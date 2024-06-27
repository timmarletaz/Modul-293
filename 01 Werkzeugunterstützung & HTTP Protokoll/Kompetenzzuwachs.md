
# Technische Grundlagen (E2)
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

Hier sieht man alle Dateien die bei [Baloise.com](https://www.baloise.com) geladen werden.



<br><br>

# GET und POST

<br>

GET und POST sind HTTP Methoden, welche für die Kommunikation z.B. mit einem Server designed wurden.

<br>

## GET

<br>

GET ist aus dem englischen und heisst nichts anderes als "holen" oder "bekommen".
Das heisst mit der Methode GET wird eine Ressource vom Server/o.ä. geholt.
<br>
    
Wenn man z.B. an die URL einen Such-Parameter anhängt, z.B. ``https://www.bbzbl.ch/?s=Stundenplan``, wird dies mithilfe der GET-Methode abgerufen, da man eine Ressource vom Server erhalten möchte. Auch das Laden einer Seite erfolgt über dies.

<br>

![GET-Method](/Sonstiges/imgs/requesttype.png)


<br>

## POST

Die POST-Methode ist so ziemlich das Gegenteil der GET-Methode, denn anstatt Ressourcen vom Server zu holen, wird bei POST etwas auf den Server "geschrieben". Dies findet man z.B. bei einem Kontaktformular, da dort die Informationen auf dem Server gespeichert werden sollen, damit man sie auch auswerten kann.


<br>
<br>
<br>
<br>

# Request und Response

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
<br>
<br>


#  Header und Body

<br>

Die Nachrichten zwischen Server und Client oder anderen Komponenten, werden immer in Header und Body unterteilt.

<br>

## Header


Header sind Teil des Anfrage- und Antwortprozesses. Der Header enthält dabei z.B. Metadaten. Diese sagen etwas über den Inhalt der Nachricht aus (um was für einen Typ es sich handelt). Ein bekanntes Beispiel wäre z.B. ``CORS`` (Cross Origin Ressource Sharing).

<br>

## Body


<br>

Im Body befindet sich der eigentliche Inhalt der Nachricht. Wie bereits erwähnt wird da z.B. die Daten von einem Formular gesendet. Diese werden meistens in einem JSON-Format (Strukturiertes Format) gesendet, welches aus den Name-Attributen des HTML-Formulars gebildet wird. Der Server kann diese Daten dann einlesen.

<br>

![JSON-POST request](/Sonstiges/imgs/JSON-Request.png)


<br>
<br>
<br>
<br>

# Caching 
<br>
Als Caching bezeichnet man den Prozess, bei dem geladene Ressourcen (Dateien) im Cache, einem temporären Speicherort, abgelegt werden, dass beim nächsten Zugriff die Ressourcen schneller geladen werden können, da nicht alle Informationen beim Server abgerufen werden müssen - Die Ladezeit wird dadurch verkürzt.
Die Ressource welche im Cache abgespeichert werden, werden mit einer TTL (Time To Live) versehen, dass heisst, wie lange sie dort bleiben. 
<br>

**Ein Beispiel** wären Webserver die dynamische Webseiten generieren. Diese speichern meistens die vitalen Dateien für ein paar Stunden oder einen Tag im Cache ab, sodass sie nicht bei jedem Besuch neu generiert werden müssen.

<br>
<br>
<br>
<br>

# Cookies
<br>

![Cookies](/Sonstiges/imgs/Cookies.png)

<br>

    Jeder kennt sie, die nervigen Cookie-Nachrichten die immer aufpopen, wenn man eine Webseite öffnet, doch für was sind diese eigentlich da?

<br>

Cookies werden verwendet um verschiedene, individuelle Benutzerdaten zu speichern. Sie helfen dabei die "Experience" einer Webseite für den Benutzer zu personalisieren. Cookies setzt man ein, um z.B. Login-Informationen, Geräte und Einkaufswägen zu speichern, um sich bei einem nächsten Besuch an diese Informationen zu "errinern", sodass z.B. der User sich nicht jedes mal neu anmelden muss.
Diese Informationen werden innert einer Textdatei gespeichert und werden vom Server bei der Verbindung erstellt. Diese Daten sind mit einer für den Client-Computer eindeutigen ID gekennzeichnet. 
Die, zum Benutzer dazugehörende Textdatei wird dann auf seine ID gespeichert. Bei einem nächsten Besuch der Webseite übermittelt der Client automatisch seine ID an den Server, welcher dann genau weiss, welche Ressourcen / Informationen er speziell für den Client bereitstellen muss.

<br>

**HTTP-Cookies** sind eine für den Browser entwickelte Art von Cookies. Sie werden eingesetzt um Informationen über die einzelnen "Sitzungen" des Benutzers zu speichern. Unter einer Sitzung (eng. session) versteht man die Zeit, die man auf einer spezifischen Webseite verbringt (jede Sitzung/session erhält zudem ihre eigene, eindeutige ID, die zwischen dem Server und dem Client gegenseitig übermittelt werden).
Der Webserver, der die Daten der Website speichert, sendet einen Strom von Informationen in Form von Cookies an den Webbrowser des Clients. 
Diese Daten werden vom Webbrowser Lokal gespeichert und beim nächsten Besuch wieder an den Webserver übermittelt.


<br>


![HTTP-Cookies](/Sonstiges/imgs/HTTP-Cookies.png)
    <br>
    
Ein Beispiel für ein HTTP Cookie.<br>Weitere Informationen, welche mehr auf den technischen Aspekt dieser Cookies eingehen, findet man unter [Microsoft-Learning](https://learn.microsoft.com/de-de/aspnet/web-api/overview/advanced/http-cookies)




<br>
<br>
<br>

# Code
<br>

    <form method="POST" action="https://formcarry.com/s/vnBDu4KXI6Z" enctype="multipart/form-data">
    [ Inhalt ]
    </form>

In diesem Code aus meiner Webseite kann man sehen, dass ich die method "Post" verwendet habe, da in diesem Fall die Daten auf den Server geschrieben werden sollen.
Das action Attribut sagt, was passiert wenn das Formular abgeschickt wird. Der "enctype" (encryption type) was mir neu. Dieser bestimmt, wie die Daten abgeschickt werden sollen.
<br>
Dafür gibt es 2 Optionen:

<br>

**multipart/form-data**: 
<br>Die Daten werden in mehrere Teile aufgeteilt und zusammen mit den Metadaten für jeden Teil einzeln übermittelt. Dies ist erforderlich, wenn das Formular die input-Typen file, image oder submit enthält.

<br>

**application/x-www-form-urlencoded**: <br>
Dies ist der Standardwert. Hierbei werden die Formulardaten in der URL-codierten Zeichenfolge an den Server gesendet. Dies bedeutet, dass Leerzeichen als + und bestimmte Zeichen als %xy (hexadezimal codiert) dargestellt werden. Dies ist z.B. bei Google der Fall:

<br>

![GoogleSuche](/Sonstiges/imgs/enctype.png)
> Im Bild kann man erkennen, dass in der URL (Uniform Ressource Locator) die verschiedenen Begriffe mit + aneinandergehängt werden.



<br>
<br>
<br>
<br>

# Was habe ich in diesem Kompetenzband gelernt?
<br>

- In diesem Kompetenzband fand ich heraus, was der wesentliche Unterschied zwischen Caching und Cookies ist.
- Zudem konnte ich die Basics des Internets sowie die Unterschiede zwischen GET und POST repetieren.
- Auch das enctype-Attribut habe ich kennengelernt.


<br>
<br>
<br>
