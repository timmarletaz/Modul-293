# Kompetenzzuwachs

<br>

## Fortgeschrittene Styling Techniken (E6)


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

> Wie man oben erkennen kann, erlaubt einem SCSS das verschachtelte Stylen, während dies in CSS nicht möglich ist.

