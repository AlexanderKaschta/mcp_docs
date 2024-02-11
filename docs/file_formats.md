# Technische Dokumentation

## Dateiformate

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