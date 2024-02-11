# Einführung

## Was ist MCP?

Mission Control Paramedic, kurz MCP, ist eine Einsatzleitsoftware für die Führung und Organisation von Sanitätsdiensten.
Fokus der Software ist es, intuitiv und übersichtlich zu sein, sodass in jeder Situation der Überblick behalten werden 
kann.

Die Software ist im Rahmen der Initiative "Coding for Charity" von [inovex](https://www.inovex.de/) in Kooperation mit 
dem Deutschen Roten Kreuz entstanden.

Zu den weiteren Vorteilen der Software gehört, dass diese kostenfrei ist und nicht nur unter Windows läuft, sondern auch
anderen Plattformen wie z.B. macOS unterstützt.

## Wann verwende ich MCP?

MCP wird dir auf einem kleinen Sanitätsdienst mit zwei Personen auf einer Sportveranstaltung recht wahrscheinlich nicht 
begegnen, denn recht wahrscheinlich habt ihr keinen Computer dabei und euch wird euch keinen wirklichen Mehrwert 
bringen.

Eine Einsatzleitsoftware ist erst hilfreich, sobald ihr einen Einsatz oder Sanitätsdienst mit Führungskräften habt. 
Dabei ist es egal, ob dies ein kleiner Dienst mit einfach nur drei Fußteams ist oder doch so große Veranstaltung, wie 
z.B. Fußballspiele der ersten und zweiten Fußballliga oder Festivals. Erst in dieser Situation haben eure Führungskräfte
die Möglichkeit, die gesamte Situation mit einer Einsatzleitsoftware im Überblick zu behalten und zu koordinieren, 
während die Teams an Hilfskräften einfach ihren Aufgaben nachgehen können.

## MCP starten

Als Helferin oder Helfer kommt man schnell in die Situation auf einem Dienst, Mission Control Paramedic zu verwenden. In
diesen Fällen ist häufig die entsprechende Infrastruktur und Geräte, wie z.B. Internet und ein Computer, bereits 
vorhanden, aufgebaut und eingerichtet ist.

!!! note "Notiz"

    In diesem Abschnitt wird sich auf die Benutzung von MCP für eine Helferin oder einen Helfer konzentriert. 
    Anleitungen für die Installation und Einrichtung von Mission Control Paramedic (MCP) als die Anleitung für das
    Führungspersonal kann in den entsprechenden Abschnitten gefunden werden.

Zuallererst müsst ihr euren Computer bereit machen, also ihn einschalten und euch anmelden. Für die weitere Anleitung 
wird angenommen, dass ihr erfolgreich euren Computer gestartet und angemeldet habt.

Um Mission Control Paramedic (MCP) verwenden zu können, müsst ihr die gleichnamige Anwendung auf dem entsprechenden 
Computer starten. Dies könnt ihr z.B. mit einem Doppelklick auf die auf dem Desktop hinterlegte Verknüpfung zu MCP 
machen oder einen passenden Eintrag im Startmenü nutzen.

## Verbindungsaufbau

Nach dem Start der Anwendung werdet ihr mit folgendem Fenster begrüßt.

![Startbildschirm von Mission Control Paramedic](assets/Startbildschirm.png)

Nun hat man zwei Optionen zur Auswahl, wie man MCP verwenden kann. Mit der ersten Option kann man die lokale MCP-Instanz
verwenden, wo dann die Daten auch auf dem Computer gespeichert werden. Gleichzeitig stellt man die eigene MCP-Instanz 
auch im lokalen Netzwerk bereit, sodass sich andere MCP-Instanzen damit verbinden können, wenn das Netzwerk entsprechend
freigeschaltet ist.

Alternativ kann man sich mit einer anderen MCP-Instanz verbinden, wo dann die Daten für MCP nutzt, die auf einem anderen
Computer gespeichert werden. Damit ihr euch mit einer anderen MCP-Instanz verbinden könnt, benötigt ihr die IP-Adresse
des anderen Computers, um die Verbindung aufzubauen. MCP speichert außerdem immer die letzte Adresse, mit der man sich
verbunden hat.

Im Regelfall wird die MCP-Instanz von der Einsatzleitung bzw. den Führungskräften bereitgestellt, sodass du dich als 
Helfer mit dieser Remote-Instanz nur verbinden musst. Da dies meist schon vorbereitet ist und auch getestet wurde, ist
es recht wahrscheinlich, dass dort schon die richtige Adresse steht. Sollte dort nichts stehen, du dir unsicher sein 
oder keine Verbindung mit der dort stehenden Instanz möglich sein, dann wende dich bitte an deine zuständige 
Führungskraft.

!!! bug "Bug"

    Achte beim Verbinden mit Remote-Rechnern auf die Adresse bzw. Url, welche im Feld steht. Sollte dort 
    `https://127.0.0.1:443` stehen, dann wurde sich beim letzten Mal mit der lokalen Instanz verbunden und nicht mit 
    einer Remote-Instanz.

## Anmeldung

Sobald du dich erfolgreich mit einer MCP-Instanz verbunden hast, wirst du nach gültigen Zugangsdaten für die jeweilige
MCP-Instanz gefragt. Diese Authentifizierung ist notwendig, da mit besonders schützenwerten persönlichen Daten 
gearbeitet wird und diese vor unberechtigtem Zugriff geschützt werden müssen. Die Anmeldemaske sieht wie folgt aus.

![Anmeldemaske von Mission Control Paramedic](assets/Anmeldebildschirm.png)

Ihr solltet die Anmeldedaten von eurer Führungskraft erhalten, solltet ihr sie sonst nicht schon kennen. Falls dies 
nicht der Fall ist, fragt bei deiner Führungskraft einfach nach.

Nach einer erfolgreichen Anmeldung landet ihr dann auf der Startseite.

!!! note "Anmerkung"

    Die Wiederherstellung des Zugangs eines Kontos mit verlorenen Zugangsdaten ist möglich. Details zur Einrichtung 
    davon werden im Abschnitt zur Installation behandelt. Die Wiederherstellung selbst wird im Fortgeschrittenen Bereich
    erklärt.

## Startseite

![Startseite von Mission Control Paramedic](assets/Startseite.png)

## Verwaltung von Sanitätsdiensten

![Sanitätsdienstverwaltung](assets/Sandienst_Verwaltung.png)

## Dashboard eines Sanitätsdienstes

![Dashboard eines Sanitätsdienstes](assets/Dashboard.png)

## Patientenübersicht

![Patientenübersicht](assets/Patientenuebersicht.png)