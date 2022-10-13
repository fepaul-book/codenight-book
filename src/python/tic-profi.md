# Profi Strategie

**Alternative Programmierung deiner KI**

> #### ⚠️ SCHWERER!  aber du kannst es für 4 Gewinnt nutzen und musst es nur wenig abändern!
 
**Version I**

1.  gehe das Feld durch und merke dir welche Felder frei sind

2. lege mit deepcopy eine Kopie des Feldes an

3. mache den ersten möglichen Zug und gucke, ob du dann gewonnen hast - wenn du gewinnst mache den Zug

4. wenn du nicht gewinnst probiere den nächsten möglichen Zug

5. gewinnst du bei keinem der Züge, mache einen Zug, bei dem du unentschieden spielst

  Gibt es keinen Zug, bei dem du gewinnst oder unentschieden spielst, dann mache einfach irgendeinen Zug

> **Damit guckst du einen Zug in die Zukunft**

<hr>

### Für dieses Vorgehen benötigst du aber auch die folgenden Funktionen:

**check_win(field, symbol):**

> ⚠️ Bei TicTacToe fehlt diese Funktion und du musst sie selbst programmieren. 
> 
> Bei 4Gewinnt ist die Funktion schon geschrieben und du kannst sie einfach aufrufen. 

Diese Funktion soll testen, ob der Spieler mit *symbol* gewonnen, verloren oder unentschieden gespielt hat und das dementsprechend returnen.
Die Funktion bekommt das Spielfeld wie oben gezeigt übergeben, sodass man die Listen durchgucken muss, ob ein Spieler gewonnen hat. 

> Beachte alle Fälle die eintreten können!

    return 0 (verloren)

    return 1 (gewonnen)

    return 2 (unentschieden)

**freie_felder(field):**

Diese Funktion soll sich in einer Liste merken, welche Felder frei sind. 

Ziel wäre zum Beispiel eine Liste die für **TicTacToe** wie folgt aussieht:

        [(1,0), (2,1)] 

Für **4Gewinnt** so: (gibt die Spalte an in die man noch werfen kann)

        [1,3,4]

<hr>

**Version II**

Wenn du mit keinem Zug gewinnen kannst, kannst du anstatt irgendeinen Zug zu machen auch gucken was der Gegner als nächstes machen könnte, wenn du gespielt hast.

Somit guckst du zwei Züge in die Zukunft.

Gehe dazu wie folgt vor:

1.  gehe das Feld durch und merke dir welche Felder frei sind

2. lege mit deepcopy eine Kopie des Feldes an

3. mache den ersten möglichen Zug und gucke, ob du dann gewonnen hast - wenn du gewinnst mache den Zug

4. wenn du nicht gewinnst mache folgendes
  
    4.1 lege eine Kopie des Spielfeldes an, wo du den ersten Zug schon gemacht hast

    4.2 merke dir alle freien Felder in diesem Feld 

    4.3 spiele mit dem Gegner Symbol den ersten möglichen Zug des Gegners

    4.4 gewinnt der Gegner dann mache deinen ersten Zug nicht und versuche einen anderen Zug

    4.5 gewinnt der Gegner mit diesem zweiten Zug nicht, soll er in ein anders freies Feld setzen und du guckst, ob er gewonnen hat - hat er gewonnen mache deinen ersten Zug nicht, usw.

    4.6 gewinnt der Gegner mit keinem seiner Züge, so kannst du den Zug machen

    4.7 hast du nur einen Zug zur Auswahl, musst du ihn machen!

> **Mit diesem Vorgehen guckst du zwei Züge in die Zukunft, deinen eigenen und den des Gegners.**  

<hr>

**Version III**

Anstatt zwei Züge in die Zukunft zu gucken kannst du 3 oder 4 Züge in die Zukunft gucken, um damit perfekt zu spielen

- Kannst du mit deinem ersten Zug gewinnen, mach ihn

- Kannst du mit dem ersten Zug nicht gewinnen guck ob der Gegner im nächsten Zug gewinnt

- Gewinnt er im nächsten Zug mache deinen ersten Zug nicht.

- Gewinnt der Gegner in keinem seiner Züge, gucke, ob du dann im dritten Zug (den Zug nach dem Gegner gewinnst)

- gewinnst du, egal welchen Zug der Gegner vorher gemacht hat, dann mache den Zug

- gewinnst du nicht bei jedem Zug, egal welchen Zug der Gegner vorher gemacht hat, dann gucke weiter in die Zukunft

- Gibt es keinen Zug bei dem du immer gewinnst, dann nimm irgendeinen Zug, bei dem der Gegner zwischendrin nicht gewinnen kann.

> **Mit diesem Vorgehen guckst du so weit in die Zukunft, bis das Spiel rum ist**


