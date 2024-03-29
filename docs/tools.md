# Tools

Dies ist eine Sammlung nützlicher Werkzeuge bzw. Tools, um die Arbeit mit MCP zu vereinfachen.

## OpenStreetMaps

[OpenStreetMap](https://www.openstreetmap.org/), auch mit OSM abgekürzt, ist ein Projekt für freies Kartenmaterial. Die Karten als auch die dazugehörigen
Daten sind frei zugänglich und werden von Nutzer bereitgestellt und gepflegt. Da das Kartenmaterial sehr ausführlich und
frei zugänglich ist, ist es eine ideale Datenquelle für MCP.

!!! info

    Das Datenmaterial von OpenStreetMaps sind offene Daten, unterliegen dennoch einer Lizenz und dem Urheberrecht. Alle
    Details dazu, wie z.B. die Namensnennung, können unter 
    [https://www.openstreetmap.org/copyright](https://www.openstreetmap.org/copyright) nachgelesen werden.

Da OpenStreetMap und Mission Control Paramedic unterschiedliche Datenformate haben, müssen die Kartendaten zuerst in das
passende Format umgewandelt werden, damit diese in Mission Control Paramedic importiert werden können. Da dieses, vor 
allem bei größeren Städten sehr aufwendig werden kann, wenn manuell gemacht, gibt es das Software-Tool `mcp_tools`. 
Diese Software kann die Daten direkt von OpenStreetMap herunterladen, konvertieren und dann als passende `*.json`-Datei
für Mission Control Paramedic bereitstellen, welche dann nur noch importiert werden muss.

[mcp_tools](https://github.com/AlexanderKaschta/MCP_Tools) ist eine quelloffene Software, welche unter der 
[MIT-Lizenz](https://github.com/AlexanderKaschta/MCP_Tools/blob/main/LICENSE) verfügbar ist.

### Installation

`mcp_tools` hat folgende Systemanforderungen:

- eine Python 3 Installation mit Version `>=3.6`
- den `pip`-Paketverwaltung
- eine aktive Internetverbindung

!!! danger "Achtung"

    Stelle sicher, dass du Python 3.6 oder höher verwendest, denn sonst wird die Software nicht funktionieren. Python 2
    wird überhaupt nicht unterstützt.


???+ tip "Tipp"
    
    Auf Linux und macOS ist Python 3 häufig schon vorinstalliert, unter Windows muss es jedoch noch instaliert werden.
    Anleitungen für die entsprechenden Plattformen können hier gefunden werden, sind jedoch auf Englisch:

    - Windows: [https://docs.python.org/3/using/windows.html](https://docs.python.org/3/using/windows.html)
    - macOS: [https://docs.python.org/3/using/mac.html](https://docs.python.org/3/using/mac.html)
    - Linux/Unix: [https://docs.python.org/3/using/unix.html](https://docs.python.org/3/using/unix.html)

Öffne ein Terminal, Kommandozeile oder Eingabeaufforderung auf, um mit der Installation zu beginnen.
Tippe nun folgenden Befehl ein

```shell
pip install git+https://github.com/AlexanderKaschta/MCP_Tools.git
```

und führe ihn aus, um `mcp_tools` zu installieren. Sobald der Befehl fertig durchgelaufen ist, ist die Installation 
abgeschlossen.

!!! info
    
    Natürlich ist auch die Installation in einem `venv` möglich. Dafür muss dieses erstellt und aktiviert sein, bevor
    der oben stehende Befehl ausgeführt wird. Mehr ist nicht zu beachten.

### Verwendung

Für die Verwendung der Software wird erneut ein Terminal, Kommandozeile oder Eingabeforderung benötigt. Dies kann die 
gleiche Instanz sein, wie sie auch für die Installation verwendet wurde, es ist aber kein muss. Dort gibst du den 
folgenden Befehl ein,

```shell
python3 -m mcp_tools
```

um die Anwendung zu starten. Da es sich um eine Konsolenanwendung handelt, wird sich alles Weitere auch im 
Konsolenfenster passieren.

Als Erstes wirst du gefragt, welche der gelisteten Aktionen du ausführen möchtest. Für den hier besprochenen Export von
OpenStreetMaps-Daten muss `OpenStreetMaps-Export` ausgewählt werden. Als Nächstes wirst du nach dem Namen der Stadt 
gefragt, für welche du Daten exportieren möchtest. Stelle dabei sicher, dass du den Namen richtig schreibst und dass es 
möglicherweise zu Fehler kommen kann, wenn ein ungültiger Name eingegeben wird. Im Hintergrund wird in den 
OpenStreetMaps-Daten nach der Stadt gesucht und alle dazugehörigen Stadtteile ermittelt. Für jeden Stadtteil erfolgt 
dann eine weitere Abfrage, um alle Straßen des Ortsteils zu ermitteln. Nun werden noch die doppelten Straßeneinträge je
Stadtteil entfernt. Die sich daraus ergebenden Daten werden dann in das passende Format für MCP abgespeichert. Die Datei
trägt den Namen `MCP-Orte-Adressen.json` und liegt in dem Ordner, in dem das Programm ausgeführt wird.

Für die Nutzung dieser Daten muss die Datei nur noch in Mission Control Paramedic importiert werden, dann stehen sie zur
Verfügung.