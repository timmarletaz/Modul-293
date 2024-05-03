# Dokumentation

<br>

## Technische Grundlagen (E)
<br>

![Technische Grundlagen](/Sonstiges/imgs/TechnischeGrundlagen.jpg)

<br>

> **Erklärung zum Bild:** <br>
> - Als erstes gibt der Client in seinem Browser die  gewünschte Adresse ein (z.B. www.bbzbl.ch)
> - Danach schaut der Browser mithilfe des (meistens eingebauten) DNS (Domain Naming System) nach der IP-Adresse der eingegebenen Domain.
> - Dort sucht es zuerst nach dem Top-Level-Domain-Anbieter (z.B. ch). Dieser gibt anschliessend die dazugehörige IP-Adresse über die vorhin genannten Schritte wieder zurück.
> - Wird in der Suchleiste vom Client kein spezifischer Port angegeben, werden die Standard Ports von HTTP (80) und HTTPS (443) verwendet, auf denen der Server ausserdem am "Hören" ist.
> - Der Client schickt nun eine Anfrage an den Webserver über einen der Ports, welcher, wenn kein Dateiname mitgegeben wurde, die Standard-Datei ``index.[kürzel]`` zurücksendet.  
Es werden allerdings auch viele andere Dateien mitgegeben (z.B. stylesheets oder JS-Dateien sowie Bilder)
> - Für diese teilt der Client dem Server zuerst mit, welche Formate, etc. er unterstützt.

<br>
<br>

![Bild](/Sonstiges/imgs/baloisecom.png)
<br>
> Hier sieht man alle Dateien die bei [Baloise.com](https://www.baloise.com) geladen werden.



<br><br>

## GET und POST

<br>

GET und POST sind HTTP Methoden, welche für die Kommunikation z.B. mit einem Server designed wurden.

<br>

### GET
<hr>

<br>

GET ist aus dem englischen und heisst nichts anderes als "holen" oder "bekommen".
Das heisst mit der Methode GET wird eine Ressource vom Server/o.ä. geholt.
<br>
Wenn man z.B. an die URL einen Such-Parameter anhängt, z.B. ``https://www.bbzbl.ch/?s=Stundenplan``, wird dies mithilfe der GET-Methode abgerufen, da man eine Ressource vom Server erhalten möchte. Auch das Laden einer Seite erfolgt über dies.

<br>

![GET-Method](/Sonstiges/imgs/requesttype.png)


<br>

### POST
<hr>

Die POST-Methode ist so ziemlich das Gegenteil der GET-Methode, denn anstatt Ressourcen vom Server zu holen, wird bei POST etwas auf den Server "geschrieben". Dies findet man z.B. bei einem Kontaktformular, da dort die Informationen auf dem Server gespeichert werden sollen, damit man sie auch auswerten kann.


<br>
<br>

## Request und Response

<br>

Request und Response sind Begriffe welche man öfters hört. Deren Bedeutung ist jedoch sehr simpel und einfach zu verstehen.

<br>

### Request
<hr>

Request ist eine Anfrage-Nachricht, welche meistens von Client-Seite an die Server-Seite geschickt wird.
Darin wird etwas gefordert. Meistens handelt es sich dabei um eine Ressource. 

<br>

### Response
<hr>

Die Response ist die Antwort auf ein Request. In der Response wird dann meistens die geforderte Ressource übermittelt, oder auch eine Fehlermeldung (z.B. "keine Berechtigung"). 


<br>

<br>

## Header und Body

<br>

Die Nachrichten zwischen Server und Client oder anderen Komponenten, werden immer in Header und Body unterteilt.

<br>

### Header
<hr>

Header sind Teil des Anfrage- und Antwortprozesses. Der Header enthält dabei z.B. Metadaten. Diese sagen etwas über den Inhalt der Nachricht aus (um was für einen Typ es sich handelt). Ein bekanntes Beispiel wäre z.B. ``CORS`` (Cross Origin Ressource Sharing).

<br>

### Body
<hr>

<br>

Im Body befindet sich der eigentliche Inhalt der Nachricht. Wie bereits erwähnt wird da z.B. die Daten von einem Formular gesendet. Diese werden meistens z.B. in einem JSON-Format (Strukturiertes Format) gesendet, welches aus den Name-Attributen des HTML-Formulars z.B. gebildet wird. Der Server kann diese Daten dann einlesen.

<br>

![JSON-POST request](/Sonstiges/imgs/JSON-Request.png)


<br>
<br>

## Caching 
<br>
Als Caching bezeichnet man den Prozess, bei dem geladene Ressourcen (Dateien) im Cache, einem temporären Speicherort, abgelegt werden, dass beim nächsten Zugriff die Ressourcen schneller geladen werden können, da nicht alle Informationen beim Server abgerufen werden müssen - Die Ladezeit wird dadurch verkürzt.
Die Ressource welche im Cache abgespeichert werden, werden mit einer TTL (Time To Live) versehen, dass heisst, wie lange sie dort bleiben. 
<br>

**Ein Beispiel** wären Webserver die dynamische Webseiten generieren. Diese speichern meistens die vitalen Dateien für ein paar Stunden oder einen Tag im Cache ab, sodass sie nicht bei jedem Besuch neu generiert werden müssen.

<br>
<br>

## Cookies
<br>

![Cookies](/Sonstiges/imgs/Cookies.png)

<br>

> Jeder kennt sie, die nervigen Cookie-Nachrichten die immer aufpopen, wenn man eine Webseite öffnet, doch für was sind diese eigentlich da?

Cookies werden verwendet um verschiedene, individuelle Benutzerdaten zu speichern. ---> In Woche 3 beenden
