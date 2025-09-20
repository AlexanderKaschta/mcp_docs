# Technische Dokumentation

## Dateiformate

!!! warning "Achtung"

    An diesem Abschnitt wird aktuell gearbeitet. Dieser kann daher gegebenenfalls nicht vollständig sein oder auch 
    Fehler enthalten.

Alle von MCP verarbeiteten Dateien müssen im [UTF-8](https://de.wikipedia.org/wiki/UTF-8) kodiert werden, damit diese
korrekt importiert werden können. Dies gilt für alle Dateiformat.

!!! bug "Inkompatibilität"

    Es muss darauf geachtet werden, dass man die Daten in UTF-8 ohne Byte-Order-Mark (BOM) speichert. Dateien, die in 
    UTF-8 mit BOM gespeichert wurden, können von nicht richtig eingelesen werden, sodass jeglicher Import dieser Dateien
    mit einem Fehler endet.

### Adressen und Objekte

**Dateityp:** `JSON`

#### Aufbau

```json title="Beispieldatei"
[
  {
    "name": "Karlsruhe-Innenstadt",
    "addresses": [
      {
        "name": "Kaiserstraße",
        "area": "Marktplatz",
        "id": 1
      },
      {
        "name": "Zirkel",
        "area": "",
        "id": 2
      },
      {
        "name": "Karl-Friedrich-Straße",
        "area": "",
        "id": 3
      }
    ],
    "objects": [
      {
        "name": "Postgalerie",
        "houseNumber": "217",
        "description": "Einkaufszentrum",
        "address": 1
      }
    ]
  }
]
```

!!! info

    Auf dem offiziellem Blog von Mission Control Paramedic gibt es auch einen Beitrag zum Import und Export von 
    Ortsdaten. Weitere Informationen zu diesem Thema können unter 
    [https://www.mission-control-paramedic.de/posts/import-und-export-von-ortsdaten](https://www.mission-control-paramedic.de/posts/import-und-export-von-ortsdaten) gefunden werden.

### Einsatzstichwörter

**Dateityp:** `CSV`

#### Aufbau

```text title="Beispieldatei"
Keyword,Synonyms
Alkoholvergiftung,"Alkohol, C2, C2-Intox"
Fraktur,Knochenbruch
Schnittverletzung,
```

### Einsatzmittel

**Dateityp:** `CSV`

#### Aufbau

```text title="Beispieldatei"
Name,Type
Auto A,KTW
Auto B,NKTW
Auto C,RTW
```

!!! warning "Achtung"

    In der Datei mit den Einsatzmitteln darf kein Name mehrfach auftauchen. Wird eine Datei importiert, die mindestens 
    einen Eintrag enthält, welcher mindestens doppelt vorkommt, so kommt es zu einer Datenverletzung mit Fehlermeldung
    und die entsprechende Datei kann nicht importiert werden.