



## ausführliche Beschreibung

Der Adapter admin dient der Bedienung der gesamten ioBroker-Installation. Er stellt ein Webinterface zur Verfügung. Dieses wird unter der `<IP-Adresse des Servers>:8081` aufgerufen. Dieser Adapter wird direkt bei der Installation von ioBroker angelegt.

Über das vom Adapter zur Verfügung gestellte GUI können u.a. folgenden Funktionen abgerufen werden:

*   Installation weiterer Adapter
*   Zugriff auf Objektübersicht
*   Zugriff auf die Zustandsübersicht der Objekte
*   Zugriff auf Benutzer und Gruppen Administration
*   Zugriff auf das Logfile
*   Verwaltung der Hosts

* * *

## Installation

Dieser Adapter wird direkt bei der Installation von ioBroker angelegt eine manuelle Installation ist nicht notwendig

* * *

## Konfiguration

[![adapter_admin_konfiguration](http://www.iobroker.net/wp-content/uploads/adapter_admin_konfiguration.png)](http://www.iobroker.net/wp-content/uploads//adapter_admin_konfiguration.png)

#### IP

Hier wird die IP-Adresse unter der der Adapter erreichbar ist eingegeben. Verschiedene Ipv4 und Ipv6 Möglichkeiten stehen zur Auswahl. <span style="color: #ff0000;">**Default ist 0.0.0.0\. Dies darf nicht verändert werden!**</span>

#### Port

Hier wird der Port, unter der der Administrator aufgerufen werden kann eingestellt. Falls auf dem Server mehrere Webserver laufen muss dieser Port angepasst werden, damit es nicht zu Problemen wegen doppelter Portvergabe kommt.

#### Verschlüsselung

Soll das sichere Protokoll https verwendet werden ist hier ein Haken zu setzen.

#### Authentifikation

Soll eine Authentifizierung erfolgen ist hier ein Haken zu setzen.

* * *

## Bedienung

Über den Webbrowser die folgende Seite aufrufen: `<IP-Adresse des Servers>:8081`

* * *

## Reiter

Die Hauptseite des Administrators besteht aus mehreren Reitern. In der Grundinstallation werden die Reiter wie in der Abbildung angezeigt. Über das Bleistift-Icon rechts oben (1) können nach der Installation zusätzlicher Adapter weitere Reiter hinzugefügt werden. Dort können auch Reiter deaktiviert werden um eine besser Übersicht zu erhalten.

[![iobroker_adapter_admin_001a](img/ioBroker_Adapter_Admin_001a.jpg)](img/ioBroker_Adapter_Admin_001a.jpg)

Ausführliche Informationen sind in den Seiten hinterlegt, die über die Überschriften verlinkt sind.

### [Adapter](http://www.iobroker.net/?page_id=5379&lang=de)

Hier werden die verfügbaren und installierten Adapter angezeigt und verwaltet.

### [Instanzen](http://www.iobroker.net/?page_id=5474&lang=de)

Hier werden die bereits über den Reiter Adapter installierten Instanzen aufgelistet und können entsprechend konfiguriert werden.

### [Objekte](http://www.iobroker.net/?page_id=5495&lang=de)

Die verwalteten Objekte (z.B. die Geräte/Variablen/Programme der CCU). Hier können Objekte angelegt und gelöscht werden. Über die _Pfeil hoch_ und _Pfeil runter_ Knöpfe können ganze Objektstrukturen hoch- oder runtergeladen werden. Ein weiterer Knopf ermöglicht die Anzeige der Expertenansicht.

Werden Werte in roter Schrift angezeigt, sind sie noch nicht bestätigt (`ack = false`).

### [Zustände](http://www.iobroker.net/?page_id=5526&lang=de)

Die aktuellen Zustände der Objekte.

### [Ereignisse](http://www.iobroker.net/?page_id=5579&lang=de)

Eine Liste der laufenden Aktualisierung der Zustände.

### [Gruppen](http://www.iobroker.net/?page_id=5549&lang=de)

Hier werden die angelegten Usergruppen angelegt und die Rechte verwaltet

### [Benutzer](http://www.iobroker.net/?page_id=5746&lang=de)

Hier können Benutzer angelegt und zu den bestehenden Gruppen hinzugefügt werden.

### [Aufzählungen](http://www.iobroker.net/?page_id=5755&lang=de)

Hier werden die Favoriten, Gewerke und Räume aus der Homematic-CCU aufgelistet.

### [hosts](http://www.iobroker.net/?page_id=5590&lang=de)

Informationen über den Rechner, auf dem ioBroker installiert ist. Hier kann die aktuelle Version des js-Controllers upgedated werden. Liegt eine neue Version vor, erscheint die Beschriftung des Reiters in grüner Farbe.

### [Log](http://www.iobroker.net/?page_id=5604&lang=de)

Hier wird das log angezeigt

Im Reiter Instanzen kann bei den einzelnen Instanzen der zu loggende Loglevel eingestellt werden. In dem Auswahlmenü wird der anzuzeigende Mindest-Loglevel ausgewählt. Sollte ein Error auftreten, erscheint die Beschriftung des Reiters in roter Farbe.

Nach der Installation zusätzlicher Adapter können noch weitere Reiter über das Bleistift-Icon oben rechts (1) aktiviert werden. Die Beschreibung dieser Reiter befindet sich bei dem entsprechenden Adapter.

### [Systemeinstellungen](http://www.iobroker.net/?page_id=6227&lang=de)

In dem sich hier öffnenden Menü werden Einstellungen wie Sprache, Zeit- und Datumsformat sowie weitere systemweite Einstellungen getätigt. [caption id="attachment_3212" align="aligncenter" width="803"][![](img/Systemeinstellungen.jpg)](img/Systemeinstellungen.jpg) Admin Systemeinstellungen[/caption] Auch die Repositorien und Sicherheitseinstellungen können hier eingestellt werden. Eine tiefergehende Beschreibung ist über den Link in dem Titel dieses Abschnitts zu erreichen.