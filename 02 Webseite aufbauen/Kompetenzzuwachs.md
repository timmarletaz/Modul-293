# Dokumentation

<br>

## Webseitenplanung (E3)

- Ich habe, bevor ich angefangen habe meine Webseite zu programmieren, ein Konzept für die Landing Page erstellt, sodass ich anschliessend nach diesem die Webseite erstellen kann und mir keine Gedanken über das Design, etc. machen muss.

<br>

![Webseitenkonzept](/Sonstiges/imgs/mockupPhone.png)

<br>

![Webseitenkonzept](/Sonstiges/imgs/mockupLaptop.png)


- Nebst dem Aufbau widmete ich mich zudem noch den Farben, welche ich verwenden wollte. Ich entschied mich dazu, dass ich 3 Hauptfarben verweden möchte. 
Ich suchte mir, zur Inspiration, auf [Color Hunt](https://colorhunt.co/) einige Farbpaletten heraus, dessen Farben mir gefiellen.
Anschliessend entschied ich mich für 3 Farben, welche meiner Meinung nach am besten zusammenpassen.

<br>

![Farbkonzept](/Sonstiges/imgs/Farbkonzept.png)


<br>


<br>

## Formulare (E4)


<br>

### Die wichtigsten Elemente

Element         | Beschreibung          | Beispiel
----------------|-----------------------| ----
`<input>`       | `<input>` ist eine Eingabefeld, für all mögliche zeichenbasierte Datentypen. Diese können mit einem "type" Parameter spezifiziert werden.      | <input placeholder="Das ist ein Input für alle Zeichen"><input type="number" placeholder="Dies ist ein Input für Zahlen"><input type="submit">
`<textarea></textarea>`     | `<textarea>` wird verwendet um grössere Texteingaben zu ermöglichen.     | <textarea style="resize:vertical; min-height: 30px; max-height: 75px;" placeholder="Dies ist eine Textarea"></textarea>
`<label></label>`       | Mit `<label for="[element-id]">Text</label>` lässt sich ein Titel für ein Form-Element erstellten. | <label for="input1">Hallo</label><input id="input1" placeholder="klicken sie auf den Text">
`<select><option></option></select>` | Dieser Tag wird verwendet um eine Dropdown-Liste anzuzeigen. Man kann auch sogenannte `<optgroups></optgroups>` einbinden. | <select><optgroup label="1-2 Option"><option>1. Option</option><option>2. Option</option></optgroup></select>
`<datalist></datalist>` | Das `<datalist>`-Element ist ein Kompromiss zwischen input und select. | **Datalist kann in Markdown nicht angezeigt werden**<br>Beispiel: [W3schools](https://www.w3schools.com/tags/tag_datalist.asp)
`<button></button>` | Um "custom" submit-buttons zu erstellen, kann man den `<button>`-Tag verwenden und diesem einen `type="submit"` verpassen. | <button type="submit">Hier kommt dein Text</button>
`<input type="checkbox"></input>` | Checkbox wird verwendent um eine einzelne, "ankreuzbare" Option darzustellen. | <input type="checkbox">Option</checkbox>
`<input type="radio"><input>` | Radiobuttons sind ähnlich wie checkboxen, nur dass diese nicht mehr abgewählt werden können. | <label for="radio">Newsletter<label><input type="radio" id="radio">


<br>


<br>


## Medien (E5)

<br>

### Map-Tag
<br>
Eine meiner lieblings Medien-Elementen in HTML ist definitiv der Map-Tag, da dieser eine Coole Funktion mit sich bringt (Tipp: klicken Sie auf ein Logo):

<img src="https://i.ytimg.com/vi/o0wfgrL07oI/maxresdefault.jpg" alt="" usemap="#map1719346753244">
<map id="map1719346753244" name="map1719346753244"><area shape="rect" coords="114,149,443,483" title="DuckDuckGo" alt="DuckDuckGo" href="https:duckduckgo.com" target="_blank"><area shape="rect" coords="832,146,1164,481" title="Google" alt="Google" href="https:google.com" target="_blank"></map>

<div style="position:relative; height:720px; width:1280px; background:url(https://i.ytimg.com/vi/o0wfgrL07oI/maxresdefault.jpg) 0 0 no-repeat;"><a style="position:absolute; top:149px; left:114px; width:329px; height:334px;" title="DuckDuckGo" alt="DuckDuckGo" href="https://www.duckduckgo.com" target="_blank"></a><a style="position:absolute; top:146px; left:832px; width:332px; height:335px;" title="Google" alt="Google" href="https://www.google.com" target="_blank"></a></div>

<br>
<br>
<br>

**Rest Siehe Webseite**