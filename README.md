
<b style="font-size:18px">Aufgabe starten: <a href="https://blockly2java.de">blockly2java.de</a></b>

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 60%; text-align: center; vertical-align: middle; padding: 5px;">Token-URL kopieren</th>
      <th style="width: 15%; text-align: center; vertical-align: middle; padding: 5px;">Klonen</th>
      <th style="width: 30%; text-align: center; vertical-align: middle; padding: 5px;">URL einfügen</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="width: 60%; text-align: center; vertical-align: middle; padding: 10px;">
        <img src="https://github.com/Blockly2Java/Template/blob/main/shared_resources/b2j_img_1.png?raw=true" style="width: 100%; height: auto; display: block; margin: 0 auto;">
      </td>
      <td style="width: 15%; text-align: center; vertical-align: middle; padding: 10px;">
        <img src="https://github.com/Blockly2Java/Template/blob/main/shared_resources/b2j_img_2.png?raw=true" style="width: 100%; height: auto; display: block; margin: 0 auto;">
      </td>
      <td style="width: 30%; text-align: center; vertical-align: middle; padding: 10px;">
        <img src="https://github.com/Blockly2Java/Template/blob/main/shared_resources/b2j_img_3.png?raw=true" style="width: 100%; height: auto; display: block; margin: 0 auto;">
      </td>
    </tr>
  </tbody>
</table>


---

## Aufgabe: Gassi gehen - Mensch und Hund in Bewegung

In dieser Aufgabe programmieren wir einen Spaziergang zwischen Mensch und Hund. Der Hund soll seinem Herrchen beim Gassi gehen folgen, wenn er gerufen wird (Bei Fuß!).

Der Code für beide Klassen ist bereits vorhanden. Sie haben bereits ein Erscheinungsbild (aus geometrischen Formen). Deine Aufgabe ist es, die Bewegungslogik und die Interaktion zwischen Mensch und Hund zu implementieren.

---

## Klassendiagramm

[//]: #[task][](structStructural[all])

![CD](http://www.plantuml.com/plantuml/proxy?cache=no&fmt=svg&src=https://raw.githubusercontent.com/Blockly2Java/Gassi/main/shared_resources/cd.puml)







---

## Beschreibung - Vorlage

- Die Main-Methode enthält bereits etwas Code, damit du deine Änderungen direkt siehst, wenn du startest. Hieran musst du nichts ändern.
- Die Konstruktoren von Mensch und Hund erzeugen alle benötigten Grafik-Objekte. Du musst sie nicht verändern. Es wird jeweils eine Grafik-Gruppe erzeugt (siehe Klassendiagramm) mit der du das ganze Objekt auf einmal bewegen kannst. Wichtig ist, dass diese Gruppe immer alle Grafiken enthält. Das genaue Aussehen kannst du anpassen, wenn du möchtest.
- Der Hund hat bereits Getter-Methoden für die Koordinaten.
- Der Hund hat bereits eine Methode `zuPositionLaufen(x,y)`, mit deren Hilfe er sich ungefährt zu einer bestimmten Koordinate bewegt. Sie ist zwar nicht super-genau, aber das sind Hunde in Wirklichkeit ja auch nicht. Für unsere Zwecke ist das aber völlig ausreichend. Wenn du sie verbessern möchtest, kannst du das natürlich tun.


---

## TODO - Der Spaziergang

[//]: #[task][](testMenschGetX(),testMenschGetY()) 
- `Mensch.getX()`, `Mensch.getY()`: Damit der Hund später nachschauen kann, wo der Mensch ist, brauchen wir Getter-Methoden für die Koordinaten des Menschen. Tipp: Nutze die Koordinaten der `grafikGruppe`.

[//]: #[task][](testBeiFuss()) 
- `Hund.beiFuss(Mensch herrchen)` — soll den Hund veranlassen, zur Position des Mensch-Objekts zu laufen, das als Parameter übergeben wird (Tipp: Nutze `zuPositionLaufen(double x, double y)`).

[//]: #[task][](testGassiGehen()) 
- `Mensch.gassiGehen()` — soll den Menschen zu einem zufälligen Punkt bewegen (Empfehlung: zufällige Bewegung zwischen 300 und 800 Einheiten pro Koordinaten-Richtung vom Startpunkt aus) und anschließend den Hund rufen.

[//]: #[task][](testHundRufen()) 
- `Mensch.hundRufen()` — soll den Hund zum Menschen rufen (nutze `beiFuss` und übergib ein geeignetes Mensch-Objekt als Parameter).




---