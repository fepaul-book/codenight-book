# Texte formatieren

Deine Website sieht noch sehr schlecht aus. 

Im folgenden wollen wir zunächst etwas Struktur in deine Website bekommen. 
Dafür fügen wir <h1>Überschriften</h1> und

leere Zeilen ein.

Dann schreiben wir manche Textteile **dick**, *kursiv* oder <u>unterstreichen</u> sie.

Anschließend wollen wir kleine [Links](../part1/was-ist-html.md) einfügen, mit denen man von einem Bereich in der Website zu einem anderen springen kann - so kann man schneller in deiner Website navigieren. 

> Wenn du dieses Kapitel gemeistert hast, hast du die Grundzüge von HTML und Websiten verstanden und der Rest ist nur noch Übung! 

<hr>

## Generell 

Wie du bereits gesehen hast, startet jeder Befehl mit einem öffnenden Teil und einem schließenden Teil. 
Alles dazwischen wird von dem Befehl beeinflusst.

Die Struktur sieht also wie folgt aus:

**\<befehl\>** Text der beeinflusst wird **\<\/befehl\>**

> ⚠️ Achte auf den **\/**  beim schließenden Teil!

## Überschriften 

Überschriften werden wie folgt geschrieben: 

        <h1> Text der beeinflusst wird </h1> 

Du kannst dabei zwischen verschiedenen Größen wählen von h1 (groß) bis h6 (klein)

# Überschrift (h1)

## Überschrift (h2)

### Überschrift (h3)

#### Überschrift (h4)

###### Überschrift (h5)
 
###### Überschrift (h6)

Der Befehl steht für Heading, also Überschrift.

## Paragraphen und leere Zeilen

Ein Paragraph ist wie ein Absatz in einem Aufsatz den du im Deutschunterricht schreibst. In einem Absatz sind zusammengehörende Sätze. Wie du gesehen hast macht HTML keine Zeilenumbrüche auch wenn du einen in deinem Code hast. Zwischen Absätzen wollen wir aber eine leere Zeile. 
Dafür kennzeichnen wir den Beginn und das Ende eines Absatzes und HTML macht die Leerzeile automatisch. 

Der Befehl für einen Absatz ist:

        <p> Text der beeinflusst wird </p>

Der Befehl steht für Paragraph, also Absatz.

<hr>

Willst du innerhalb eines Paragraphen Text in einer neuen Zeile starten, so machst du das mit folgendem Befehl. 

        <br> Text der beeinflusst wird </br>

Der Befehl steht für line break, also Zeilenumbruch. 


## Fett und kursiv

Der Befehl um etwas <b>fett</b> zu schreiben ist:
    
        <b> Text der beeinflusst wird </b>

Der Befehl steht für bold, also dickgedruckt.

<hr>

Der Befehl um etwas <i>kursiv</i> zu schreiben ist:

        <i> Text der beeinflusst wird </i>

Der Befehl steht für italic, also kursiv.

## horizontale Linien

Der Befehl um eine horizontale Linie auf der Website einzufügen ist:

        <hr>
<hr>

> ⚠️ Dieser Befehl ist eine Ausnahme, da er nur aus einem Teil besteht!

Der Befehl steht für horizontal rule, also horizontale Linie.


## Zitate einfügen

Der Befehl um ein Zitat einzufügen ist:

        <blockquote cite="url der Quelle"> Zitat </blockquote>

<blockquote cite="https://www.myzitate.de"> 
"Ist die Codenight nicht cool?" (Felix)
</blockquote>

Der Befehl steht für Anführungszeichen, also für ein Zitat.

## Links

Ein [Link](https://de.wikipedia.org/wiki/Hyperlink) ist eine Verknüpfung zu einer anderen DAtei/Website/ einem Foto, ...

Der Befehl um einen Link zu einer anderen Website einzufügen ist:

        <a href="https://url.de"> Text der angezeigt werden soll um etwas zu verlinken </a>

Man kann auch Links innerhalb einer Website erstellen, um zum Beispiel an den Anfang der Website oder einem speziellen Absatz zu gelangen. Das lernst du aber erst später.


##  Jetzt wird erstmal das neu gelernte geübt!


