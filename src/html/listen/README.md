# Listen und Tabellen

Es gibt verschiedene Arten von Listen.

### Unsortierte Listen

> ![Beispiel einer unsortierten Liste](img/unsortierte-liste.png)

Unsortierte Listen sind einfach Listen deren Einträge nicht durchnummeriert sind, sondern einfach nur einen Punkt zur Markierung eines neuen Listeneintrags haben. 

- **Befehl:** 

        < ul> 

        <li>  erster Punkt </li>
        
        <li> zweiter Punkt </li>

        <li> ... </li>

        <\/ul>

- Der Befehl ul steht für **unordered** List, also unsortierte Liste.

- Der Befehl li steht für list item, also für Listenelement oder einfach Eintrag.

<hr>

### Sortierte Listen

> ![Beispiel einer sortierten Liste](img/sortierte-liste.png)

Sortierte Listen sind einfach Listen deren Einträge durchnummeriert sind.


- **Befehl:**

        < ol> 

        <li>  erster Punkt </li>
        
        <li> zweiter Punkt </li>

        <li> ... </li>

        <\/ol>

- Der Befehl ol steht für **ordered** List, also unsortierte Liste.

- Der Befehl li steht für list item, also für Listenelement oder einfach Eintrag.

<hr>

### Spezielle Listen
Man kann auch *Listen in Listen* erstellen:

1. erster Punkt
    - 1.1 
    - 1.2
2. zweiter Punkt 
3. ... 

Außerdem gibt es noch *Definitionslisten*, aber die braucht man fast nie.

## Tabellen

> ![Beispiel einer einfachen Tabelle](img/tabelle.png)

Kopiere den Code unterhalb am besten in deine Website und ändere ihn nur ab, dann ersparst du dir viel Tipparbeit.

    <!-- Beginn der Tabelle-->
        <table>
    <!-- Tabellenüberschriften -->
            <thead>
                <tr>
                <!-- erste Zeile mit Spaltennamen -->               
                <th> mag ich</th> 
                <th> mag ich nicht</th>
                </tr>
            </thead>
    <!-- Tabelleninhalt -->
            <tbody>
        <!-- zweite Zeile -->
            <tr>
                <td> Antilopen</td>
                <td> Autoreifen</td>
            </tr>
        <!-- dritte Zeile -->            
            <tr>
                <td> Fleisch</td>
                <td> Pokemon</td>
            </tr>
        <!-- vierte Zeile -->
            <tr>
                <td> Hundefutter</td>
                <td> Kuscheltiere</td>
            </tr>
          </tbody>
        </table>


Eine Tabelle hat eine feste Form 

- **Tabelle - Beginn** (table)

  Markiert durch den *table* Befehl.

    Dieser Befehl zeigt, dass es sich im folgenden um eine Tabelle handelt.

- **Tabellenkopf - Beginn** (thead)

  Markiert durch den *thead* Befehl.

    Das markiert den Bereich in dem die Spaltenüberschriften definiert werden.

- **Spaltenüberschrift** (tr und th)
    
        <thead>
            <tr>
            <!-- erste Zeile mit Spaltennamen -->               
            <th> mag ich</th> 
            <th> mag ich nicht</th>
            </tr>
        </thead>

    Eine Zeile beginnt und ende mit *tr* für Table Row also Tabellenzeile.
    
    Darin sind Zeileneinträge mit *th* für Table Head also Tabellenüberschrift.

    Die Spaltenüberschriften sind also auch nur eine Zeile außer, dass deren Inhalt dick gedruckt wird, was man durch das *th* anzeigt.

- **Tabellenkopf - Ende** (thead)

    Markiert durch den *thead* Befehl.

- **Tabelleninhalt - Beginn** (tbody)

    Markiert durch den *tbody* Befehl.

    Hier wird die Tabelle jetzt mit Inhalt (Zeilen gefüllt).

- **Tabellenzeile 2** (tr und td)

    Durch *tr* (table row - Tabellenzeile) wird eine Tabellenzeile begonnen und beendet.

    Durch die *td* Befehl (td = table data, Tabellendaten) wird ein Eintrag in einer Zeile erzeugt. 
  
        <tr> 
         <td> Zeileneintrag </td>
         <td> Zeileneintrag </td>
        </tr>

- Tabellenzeile 3
            ...
- Tabellenzeile ... 
            ...
- **Tabelleninhalt - Ende** (tbody)

    Markiert durch den *tbody* Befehl.

- **Tabellen - Ende** (table)

    Markiert durch den *table* Befehl.





