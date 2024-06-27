
# Fortgeschrittene Styling Techniken (E6)


### SCSS

> Ich verwendete SCSS für mein Projekt, da ich dies aufgrund seiner Übersichtlichkeit und Abwärtskompabilität am meisten mag.<br>
Ich musste mich am Anfang allerdings nochmals darüber informieren.


<br>

### Das wichtigste in Kürze

> SCSS steht für "Sassy CSS" und ist eine erweiterte Syntax für Cascading Style Sheets (CSS). Es bietet zusätzliche Funktionen wie Variablen, Verschachtelung von Selektoren, Mixins (für wiederverwendbare Stile) und importierbare Teildateien. SCSS-Dateien werden in der Regel in normale CSS-Dateien kompiliert, die von Webbrowsern interpretiert werden können, wobei alle Vorteile der erweiterten Funktionen erhalten bleiben. Entwickler verwenden SCSS, um den Prozess der CSS-Erstellung effizienter und strukturierter zu gestalten.

Definition durch [ChatGPT](https://chatgpt.com/share/68127b32-9bc0-41f4-829f-6ab38ecbca32)


<br>
<br>

#### **Man kann unten die Unterschiede zwischen CSS, SASS und SCSS erkennen.**

![Vergleichstabelle](/Sonstiges/imgs/SCSS.png)
<br>
Bild von [Lightweb](https://lightweb-media.de/webentwicklung/unterschied-css-less-scss-sass/#:~:text=SCSS%20(Sassy%20CSS)%20ist%20eine,zu%20organisieren%20und%20zu%20verwalten)

<br>

<br>




### CSS VS SCSS

<br>

#### CSS:

    :root {
        --primary: #f1f1f1;
        --secondary: #ffffff;
    }


    body {
        background-color: var(primary);
    }

    
    body h1{
        color: var(secondary);
    }



<br>
<br>


#### SCSS

    $primary: #f1f1f1;
    $secondary: #ffffff;

    body {
        background-color: $primary;

        h1 {
            color: $secondary;
        }

    }


<br>
<br>

> Mehr kann man im [Style](https://github.com/timmarletaz/M293-V3) meiner Website sehen.

> Wie man oben erkennen kann, erlaubt einem SCSS das verschachtelte Stylen, während dies in CSS nicht möglich ist.

<br>
<br>

### Was bietet SCSS für Vorteile?

<br>

    @mixin preset1{
        display: flex;
        justify-content: center;
        align-items: center;
    }

    body{
        background-color: #f1f1f1;
        @include preset1();
    }

<br>

> SCSS lässt einem "Mixins" erstellen, was nichts anderes als vordefinierte Zeilen sind. Diese kann man anschliessend in Elemente einbinden und so viele Zeilen sparen.


<br>
<br>
<br>

# Responsives Layout (E7)

<br>

Eine Responsiven Wesbeite kann man mit folgendem Mittel umgesetzt werden.

<br>

### Breakpoints (@media query)

<br>

CSS Breakpoints sind bestimmte Punkte in einer Website oder Anwendung, bei denen das Layout und Design an verschiedene Bildschirmgrößen und Gerätetypen angepasst werden. Diese werden durch Media Queries definiert, die Bedingungen festlegen, wann bestimmte CSS-Regeln angewendet werden sollen, um ein responsives Design zu gewährleisten.

<br>

### Code

    body{
        background-color: blue;
    }

    @media screen and (max-width: 500px){
        background-color: red;
    }

> Im oben steheneden Code hat der Body der Webseite die Hintergrundfarbe rot.
Wenn nun von einem Gerät mit kleinerer Viewport-Width als 500px auf die Webseite zugegriffen wird ändert sich die Hintergrundfarbe zu blau.

<br>

### Ergebnis

![MediaQuery](/Sonstiges/imgs/mediaQuery.gif)



<br>
<br>
<br>





# Was habe ich in diesem Kompetenzband gelernt?
<br>

- In diesem Kompetenzband habe ich mich erneut zum Thema [SCSS](#scss) schlau gemacht, da ich dies sehr lange nicht mehr benutzt habe. Ich konnte somit nochmals das Wichtigste dazu aufnehmen.

- Der Inhalt zu [Responsives Layout](#responsives-layout) ist als Zusammenfassung für mich selbst gedacht und zählt nicht zu meinem Lernfortschritt.




