# Tic Tac Toe

Tic Tac Toe kennt jeder - das Spiel muss man nicht erklären.

![tic tac toe](img/tic-tac-toe.png)

<hr>

### Ziele

Die Ziele beim Entwickeln eurer KI sind die folgenden:

  1. gewinne gegen Gegner die **zufällig** spielen

  2. gewinne gegen **Menschen** die optimal spielen

<hr>

> # ⚠️ Download Code
> 
> [Hier](ki3.zip) kannst du den vorgefertigten Code runterladen.
> 
> Entpacke das zip archiv mit Rechtsklick und nutze die vorgefertigten Dateien.
> 
> Du musst nur in die **ki_tictactoe.py** Datei gucken.

### Vorbereitungen

Das Spielfeld habe ich schon programmiert.

Das ist einfach eine Liste in einer Liste:

**leeres Feld**

    feld = [
         ['_','_','_'],
         ['_','_','_'],
         ['_','_','_']
        ]

    -->  [
         ['_','_','_'],
         ['_','_','_'],
         ['_','_','_']
        ] 

<hr>

Wenn man jetzt in **ein Feld schreiben** will, muss man zuerst die **Zeile**, dann die **Spalte** angeben.

    feld[0][1] = 'X'
    print(feld)

    -->  [
         ['_','X','_'],
         ['_','_','_'],
         ['_','_','_']
        ]
> ⚠️ **Die Nummerierung beginnt wie immer bei 0!**


<hr>

#### Das Spiel wird gestartet mit:

    spiel = TicTacToe(x=input_player, o=random_player)
    spiel.start()

Spieler x fängt immer an.

<hr>

#### Es gibt 3 Spielertypen:

  - *random_spieler*
    
    Dieser Spieler spielt zufällig. Diesen habe ich schon implementiert.

  - *input_player*

    Wenn du das auswählst kannst du selbst spielen, indem du in die Konsole die Koordinaten schreibst, z.B. 1,2

    Dieser Spieler ist auch schon implementiert.

  - **ki_player**

    Den Spieler sollst du selbst schreiben. Dieser Spieler soll dann optimal spielen und nie verlieren.

<hr >

## ki_player(field, symbol): programmieren

- Der KI-Player gibt zwei Koordinaten zurück.

    Zum Beispiel sagt er, dass in das Feld links oben geschrieben werden soll.

        return 0,0

- Der KI-Spieler bekommt das Feld und sein eigenes Symbol.

**Vorgehen zum Programmieren des KI-Spielers**

- Um zu entscheiden wohin der Ki-spieler als nächstes sein Symbol setzt:

  - gehe das Feld durch und gucke dann wohin du setzen musst
    
    z.B. wenn der Gegner zwei in einer Reihe hat, musst du in das letzte freie Feld in dieser Zeile setzen

  - bei diesem Vorgehen kannst du alle möglichen Fälle mit einer if-Abfrage einfach abtippen (Zeilen, Spalten und Diagonalen testen)

<hr>

## Testen deiner KI

#### KI vs Du

        spiel = TicTacToe(x=ki_player, o=input_player)
        spiel.start()

####  KI vs zufälliger Spieler

        test_durchlauf(x=ki_player, o=random_player, n=100)

Damit kannst du automatisch 100 Runden gegen einen zufälligen Spieler spielen und sehen wie oft deine KI verloren hat. Wenn du nie verlierst ist deine KI perfekt. 

#### Deine KI vs KI von Mitschüler

Wenn du nur eine Statistik willst, welche KI besser ist, kannst du wie folgt vorgehen:

- kopiere den Code aus ki_player von deinem Mitschüler in **ki_player2** rein

- rufe folgendes auf:
    
        test_durchlauf(x=ki_player, o=ki_player2, n=100)

- damit hast du nur eine Statistik wie oft du gewonnen hast

<hr>

Wenn du verfolgen willst, wie die KIs gegeneinander spielen gehe wie folgt vor:

- kopiere den Code aus ki_player von deinem Mitschüler in **ki_player2** rein

- rufe folgendes auf:

        spiel = TicTacToe(x=ki_player, o=ki_player2)
        spiel.start()
