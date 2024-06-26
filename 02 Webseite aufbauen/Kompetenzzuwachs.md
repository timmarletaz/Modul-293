# Kompetenzzuwachs


<br>
<br>
<br>


# Webseitenplanung (E3)

- Bevor ich angefangen habe meine Webseite zu programmieren, habe ich mir Gedanken über das Aussehen meiner Webseite (Landing Page) gemacht.
Diese Gedanken fasste ich im nachfolgenden Konzept zusammen. Dies sollte mir anschliessend beim Realisieren helfen.

<br>

![Webseitenkonzept](/Sonstiges/imgs/mockupPhone.png)

<br>

![Webseitenkonzept](/Sonstiges/imgs/mockupLaptop.png)


- Nebst dem Designkonzept überlegte ich mir noch, welche Farben ich verwenden wollte.
Ich suchte mir, zur Inspiration, auf [Color Hunt](https://colorhunt.co/) einige Farbem heraus, welche mir gefielen.
Entschieden habe ich mich für folgende drei.

<br>

![Farbkonzept](/Sonstiges/imgs/Farbkonzept.png)


<br>

### Webseitenstruktur

<br>

![Struktur](/Sonstiges/imgs/structure.png)


<br>

<br>
<br>


# Formulare (E4)


<br>

### Die wichtigsten Elemente

Element         | Beschreibung          
----------------|-----------------------| 
`<input>`       | `<input>` ist eine Eingabefeld, für all mögliche zeichenbasierte Datentypen. Diese können mit einem "type" Parameter spezifiziert werden.
`<textarea></textarea>`     | `<textarea>` wird verwendet um grössere Texteingaben zu ermöglichen.
`<label></label>`       | Mit `<label for="[element-id]">Text</label>` lässt sich ein Titel für ein Form-Element erstellten. 
`<select><option></option></select>` | Dieser Tag wird verwendet um eine Dropdown-Liste anzuzeigen. Man kann auch sogenannte `<optgroups></optgroups>` einbinden. 
`<datalist></datalist>` | Das `<datalist>`-Element ist ein Kompromiss zwischen input und select.
`<button></button>` | Um "custom" submit-buttons zu erstellen, kann man den `<button>`-Tag verwenden und diesem einen `type="submit"` verpassen.
`<input type="checkbox"></input>` | Checkbox wird verwendent um eine einzelne, "ankreuzbare" Option darzustellen.
`<input type="radio"><input>` | Radiobuttons sind ähnlich wie checkboxen, nur dass diese nicht mehr abgewählt werden können.


<br>

## Code (E4)

<br>

Den Code zur gesamten Website findet man [hier](https://github.com/timmarletaz/M293-V3)

<br>

### E4

    <form method="POST" action="https://formcarry.com/s/vnBDu4KXI6Z"
                enctype="multipart/form-data">

                <div class="formContainer">

                    <label for="Vorname">Vorname</label>
                    <input id="Vorname" name="Vorname" type="text"
                        maxlength="20" required
                        title="Ihr Name muss aus einem Gross- und mind. 2 Kleinbuchstaben bestehen"
                        placeholder="Ihr Vorname...">

                    <label for="Nachname">Nachname</label>
                    <input id="Nachname" name="Nachname" type="text"
                        maxlength="30" required
                        title="Ihr Name muss aus einem Gross- und mind. 2 Kleinbuchstaben bestehen"
                        placeholder="Ihr Nachname...">

                    <label for="Land">Land</label>
                    <select id="Land" name="Land">
                        <option selected>Wählen Sie ihr Land</option>
                        <optgroup label="Nachbarländer der Schweiz">
                            <option>Schweiz</option>
                            <option>Deutschland</option>
                            <option>Österreich</option>
                            <option>Italien</option>
                            <option>Frankreich</option>
                            <option>Fürstentum Lichtenstein</option>
                        </optgroup>
                        <optgroup label="Andere europäische Länder">
                            <option>Belgien</option>
                            <option>Luxemburg</option>
                            <option>Niederlande</option>
                        </optgroup>
                    </select>

                    <label for="TelNum">Telefonnummer</label>
                    <input id="TelNum" type="tel" name="TelNum">

                    <label for="message">Nachricht</label>
                    <textarea id="message" name="message" maxlength="300"
                        required></textarea>

                    <label for="file" class="file"><i
                            class="fa-solid fa-cloud-arrow-up"></i>
                        Dateien</label>
                    <input type="file" id="file" name="file" hidden
                        accept=".doc, .docx, .txt, .pdf">
                    <span id="fileText">Keine Dateien ausgewählt</span>

                    <button type="submit" id="submit" name="submit">Senden <i
                            class="fa-solid fa-paper-plane"></i></button>

                </div>

            </form>

<br>

### Ergebnis

<br>

![Resultat](/Sonstiges/imgs/Form.png)

<br>
<br>
<br>
<br>
<br>


# Medien (E5)

<br>

### Map-Tag
<br>
Eine meiner lieblings Medien-Elementen in HTML ist definitiv der Map-Tag, da dieser eine Coole Funktion mit sich bringt (Tipp: klicken Sie auf ein Logo):

<img src="https://i.ytimg.com/vi/o0wfgrL07oI/maxresdefault.jpg" alt="" usemap="#map1719346753244">
<map id="map1719346753244" name="map1719346753244"><area shape="rect" coords="114,149,443,483" title="DuckDuckGo" alt="DuckDuckGo" href="https:duckduckgo.com" target="_blank"><area shape="rect" coords="832,146,1164,481" title="Google" alt="Google" href="https:google.com" target="_blank"></map>

<div style="position:relative; height:720px; width:1280px; background:url(https://i.ytimg.com/vi/o0wfgrL07oI/maxresdefault.jpg) 0 0 no-repeat;"><a style="position:absolute; top:149px; left:114px; width:329px; height:334px;" title="DuckDuckGo" alt="DuckDuckGo" href="https://www.duckduckgo.com" target="_blank"></a><a style="position:absolute; top:146px; left:832px; width:332px; height:335px;" title="Google" alt="Google" href="https://www.google.com" target="_blank"></a></div>

<br>
<br>

 > Weitere Informationen zu Multimedia-Tags findet man auf folgender [Webseite](https://www.almabetter.com/bytes/tutorials/html/multimedia-in-html)

<br>
<br>
<br>



# Was habe ich in diesem Kompetenzband gelernt?
<br>

- In diesem Kompetenzband lernte ich, wie wichtig es ist, einen guten Plan zu haben, bevor man eine Webseite zu realisieren beginnt.

- Der Rest, welcher im Kompetenzzuwachs erwähnt wurde, habe ich als Zusammenfassung für mich selbst geschrieben, um bei Unklarheiten nachschauen zu können.


<br>
<br>
<br>

