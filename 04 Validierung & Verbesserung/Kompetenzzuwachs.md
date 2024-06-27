
# Validierung und Verbesserung (E8)
<br>

![Slow loading website](https://media0.giphy.com/media/cmNXhHqqK5HhTHUK4g/giphy.gif?cid=6c09b952zop92gmmjlz3une4c3h6gq3ebcgir280q2bwbq2w&ep=v1_gifs_search&rid=giphy.gif&ct=g)


> Wer kennt es nicht? Man möchte eine Webseite besuchen, doch diese lädt ewig.<br>
Meistens ist man genervt und sucht sich irgend eine andere Webseite.


**Genau das kann man als Entwickler mit folgenden Punkten vermeiden.**

<br>
<br>
<br>

# Dateiformat

- Das Ziel eines Entwickler ist es möglichst kleine Dateien mit möglichst guter Qualität in seine Webseite einzubauen, um die Ladegeschwindigkeit zu verbessern während man qualitativ hochwertige Bilder bietet.

- Es ist also wichtig zu Wissen, welche Dateiformate sich für was eignen.


<br>

### Bilder

Dateiformat | Für was eignet es sich? | Vorteile | Nachteile
------------|-------------------------|----------|-------------
jpg | Bilder mit vielen Farben | Gute Kompression bei geringer Dateigrösse | Verlustbehaftete Kompression
png | Bilder mit transparenzen | Verlusfreie Kompression | Grössere Datei als jpg
gif | Animationen und Grafiken | Unterstützt Animationen | Beschränkte Farbtiefe
webp | Bilder mit vielen Farben | Bessere Kompression als jpg und png, unterstützt transparenz | Von alten Browsern nicht unterstützt


<br>

#### Bilder lokal beziehen vs von einem Server

Art | Vorteile | Nachteile |
----|----------|-----------|
Server | Zentralisierte Verwaltung, Skalierbarkeit | Längere Ladezeiten, Sicherheitsrisiken, CORS-Probleme
Lokal | Schnellere Ladezeiten, Unabhängigkeit, Sicherheit, Kein CORS | Speicherplatz, Verwaltungsaufwand

<br>
<hr>
<br>

### Videos

Dateiformat | Für was eignet es sich? | Vorteile | Nachteile |
------------|-------------------------|----------|-------------
mp4 | Allgemeiner Einsatz von Videos | Gute Kompression, weit unterstützt | Grosse Dateigrösse
webM | Videos für das Web | Effiziente Kompression | Nicht so verbreitet wie mp4, nur für moderne Browser


<br>
<hr>
<br>

### Audio

Dateiformat | Für was eignet es sich? | Vorteile | Nachteile  |
------------|-------------------------|----------|--------------
mp3 | Allgemeiner Einsatz von Audiodateien | Weit verbreitet | Verlustbehaftete Kompression --> Beeinträchtigt Qualität
ogg | Allgemeiner Einsatz von Audiodateien | Gute Qualität --> Verlustfreie Kompression | Nicht so verbreitet wie mp3, unterstützung in älteren Browsern eher schlecht


<br>
<hr>
<br>

> Ich habe für Bilder in meiner Webseite webP als Dateiformat verwendet, da es das beste Qualität-Dateigrösse-Verhältnis bietet.
Zudem verwendete ich das eine oder andere Gif.
Den Grossteil der Ressourcen sind dabei lokal gespeichert.

<br>
<br>

<br>
<br>


# SEO

<br>

Search Engine Optimization beschreibt den Prozess seine Webseite so zu gestalten, dass sie möglichst vielen Usern zuoberst in der Suchmaschine angezeigt wird.

Es gibt mehrere Möglichkeiten, wie man dies erreichen kann:

<br>

### Meta tags
<hr>
<br>

Die Meta-Tags sind im Head der Webseite und sagen der Suchmaschine wer der Author ist, was diese Webseite für Inhalt hat und
was Such-Schlagwörter sind.

<br>

Man sollte versuchen, Schlagwörter anzugeben, welche häufig gesucht werden.
Es gibt Webseiten, welche einem dabei helfen solche Wörter zu finden.

Eine davon ist [Ubersuggest](https://neilöatel.com/ubersuggest)

<br>

Im unteren Bild kann man erkenenn wie oft "Informatik" gesucht wurde.

![Ubersuggest](/Sonstiges/imgs/SEO.png)

<br>


#### Code
    <head>
        <meta name="keywords" content="Tim Marletaz, Tim, Modul 293, eportfolio, Informatiker, HTML, CSS, Javascript">
        <meta name="description" content="Ein Eportfolio von Tim Marlétaz">
        <meta name="author" content="Tim Marlétaz">
        <meta name="theme-color" content="#bed4f7">
    </head>


<br>
<br>


### Google Ads
<hr>
<br>

Neben den Media-Tags kann man sich auch bei [Google Ads](https://ads.google.com) "Plätze" in der Suchmaschine kaufen. 
Die Regel dabei lautet:<br>
> Je mehr Geld man für Ads ausgibt, desto höher ist das "Ranking" der Webseite.

Zudem kann man auf Google Ads die "Keywords" für die Webseite definieren. 


<br>

![Google Ads](/Sonstiges/imgs/GoogleKeywords.png)


<br>
<br>

### Lighthouse
<hr>
<br>

Eine gratis Methode um seine Webseite zu verbessern ist Lighthouse. Lighthouse ist êin, von Google entwickeltes, Werkzeug zur Messung der Qualität einer Webseite. Man findet es in den Entwicklertools von Chrome.<br>
Es gibt einem Feedback über die Webseite und listet auf, was man noch verbessern sollte.


Als ich Lighthouse das erste Mal über meine Webseite laufen liess, war das Ergebnis ziemlich schlecht.

![Lighhouse-Ranking](/Sonstiges/imgs/beforeLighthouse.png)



<br>
<br>

Als ich es jedoch nach Fertigstellung der Webseite nochmals durchgeführt habe, sah es so aus:

![Lighthouse-Ranking 2](/Sonstiges/imgs/Lighthouse.png)


<br>
<br>
<br>

# Validatoren
<br>

Es gibt verschiedene HTML und CSS Validatoren. <br>
Hier sind einige davon:

<br>

### HTML
<hr>
<br>

[JSON-Formatter](https://jsonformatter.org/html-validator#google_vignette)<br><br>
[W3C-Validator](https://validator.w3.org/)<br><br>
[NU-HTML-Validator](https://validator.nu/)

<br>

### CSS
<hr>
<br>

[CSS Validator](https://css-validator.org)
<br>
<br>

[Code Beautify](https://codebeautify.org/cssvalidate)
<br>
<br>

[CSS-Portal](https://www.cssportal.com/css-validator/)


<br>
<br>
<br>
<br>

# Was habe ich in diesem Kompetenzband gelernt
<br>

- Ich habe in diesem Kompetenzband gelernt, wie wichtig es ist, die richtigen Dateiformate zu verwenden, da dies einen grossen Unterschied machen kann.

- Zudem habe ich gelernt wie man richtig SEO betreibt und was man dabei beachten sollte. Ich habe zwar die Meta-Tags gekennt, jedoch nicht gewusst, dass diese so einen grossen Einfluss haben können.