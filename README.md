# Algorithmen einfach erklärt
## Ich versuche pro Woche mindestens eine Erklärung zu einem Algorithmus hochzuladen.
Da ich, als ich angefangen habe, Algorithmen zu lernen, leider größtenteils auf rein englisch sprachige Tutorials gestoßen bin, was nicht unbedingt dabei geholfen hat, sie zu verstehen, dachte ich mir, so etwas müsste es in Deutsch geben.
Aus diesem Grund werde ich in diesem Repository ein paar der bekanntesten Algorithmen in Deutsch näher erklären.
Alle Algorithmen werden für ein besseres Verständnis zusätzlich zu der Erklärung noch in Python implementiert.
Ich habe mir Python ausgesucht, da diese Programmiersprache auch für Leser ohne Programmierkenntnisse leicht zu verstehen ist.
<br>
Des weiteren werden Kenntnisse über folgende Datenstrukturen vorausgesetzt, da ich auf diese nicht genauer eingehen werde.
* Array (Listen in Python)
* set
* Queue (FirstInFirstOut) / Stack (LastInFirstOut)
* Graphen


## Grundlegendes Vokabular und Erklärungen
First things first.
### Was ist ein Algorithmus? <br>
Einfach erklärt, ein Algorithmus ist eine Reihe von Anweisungen, die Schritt für Schritt ausgeführt werden, um ein bestimmtes Problem, wie beispielsweise das Sortieren einer Liste, zu lösen.
Sie helfen uns aber auch im Alltag weiter, Stichwort Google Maps.
Zu den bekanntesten gehören unter anderem die Algorithmen:
* Bubblesort
* Insertionsort
* Quicksort
* Mergesort
* Breadth First Search / Depth First Search (Breiten- und Tiefensuche)
* Dijkstras Algorithmus
* Binary Search (Binäre Suche)
* Euklidischer Algorithmus
* SHA-256 (Wird bspw. im Bitcoin Netzwerk für das Mining und zur Erstellung von Bitcoin Adressen verwendet)
* Shors Algorithmus
<br>
Wobei Letzterer für Quantencomputer und nicht für herkömmliche Computer entwickelt wurde.
<br>
Die Leser, die gerne mehr über den Shor-Algorithmus erfahren möchten, können dies hier tun:
<br>
https://de-academic.com/dic.nsf/dewiki/1283433
<br>
<br>
Einige dieser Algorithmen werde ich in diesem Repository behandeln.
<br>

### Landau-Notation (O-Notation oder auch big O notation)
Wenn du relativ neu im Thema Algorithmen bist, wirst du dir wahrscheinlich die Frage stellen, was ist die Landau-Notation und wozu brauch man sie.
Da in der Informatik das Laufzeitverhalten von Programmen eine wichtige und fundamentale Rolle spielt, muss es eine Möglichkeit geben, dieses anzugeben.<br>
Kommen wir nun zu unserem vorherigen Beispiel, dem sortieren einer Liste zurück.<br>
Da die Länge einer Liste, welche mit einem Bestimmen Algorithmus sortiert werden soll, meist variabel ist, kann man die Laufzeit des Algorithmus nicht in Sekunden oder Minuten angeben.
Hier kommt die Landau-Notaion (auch O-Notation genannt) ins Spiel.<br>
Diese ermöglicht es uns, eine allgemeine Aussage über das Laufzeitverhalten von Algorithmen zu tätigen.
<br>
Jetzt folgt eine kleine Erklärung, der häufigsten Notationen.

**O(1)**:
konstante Komplexität, die Laufzeit hängt nicht von der Datenmenge ab.
z.B. Arrayzugriff, Hashtable.
<br>
<br>
**O(n)**:
lineare Komplexität, die Laufzeit ist propertional zur Datenmenge.
z.B. Schleife über ein Array um einen Wert zu finden, Einlesen einer Treffermenge aus der Datenbank.
<br>
<br>
**O(n²)**:
quadratische Komplexität, eine doppelte Datenmenge vervierfacht die Laufzeit
z.B. Bubble-Sort.
<br>
<br>
**O(log n)**:
logarithmische Komplexität, wird die Datenmenge jeweils verdoppelt, steigt die Laufzeit linear an
z.B. Suchbäume.
<br>
<br>
**O(n log n)**:
superlineare Komplexität, liegt zwischen 𝒪(n) und 𝒪(n²). Tritt zum Beispiel auf, wenn eine Schleife über eine Baumsuche gebildet wird.
z.B. optimierte Sortieralgorithmen wie Quicksort.
<br>
<br>
**O(2ⁿ)**:
exponentielle Komplexität, die Laufzeit verdoppelt sich, wenn die Datenmenge um eine Einheit größer wird.
z.B. Bilden aller Paare einer Menge, Türme von Hanoi als rekursiver Algorithmus
<br>
<br>
**O(n!)**:
faktorielle Komplexität, die Laufzeit wächst mit der Fakultät der Datenmenge.
z.B. Problem des Handlungsreisenden.
<br>
<br>
Da es manchen bestimmt trotzdem noch schwerfällt, sich darunter was vorzustellen, habe ich hier noch mal ein Bild eingefügt, welches das soeben Beschriebene visuell darstellt.
<br>

![image](https://user-images.githubusercontent.com/83044113/151657832-9b5915d3-65ec-4f43-a859-9e8c630d81ea.png)
<br>
<br>
Zusätzlich spielt auch noch die sogenannte Space complexity (Platzkomplexität) eine wichtige Rolle.
Diese gibt an, wie viel Speicher ein Algorithmus benötigt.
Die Platzkomplexität wird ebenfalls mit der zuvor erklärten Landau-Notation angegeben.
<br>
<br>

### In-Place-Algorithmus
Wenn du dich mit Algorithmen beschäftigst, wirst du um den Begriff In-Place nicht herumkommen.
Dieser bedeutet lediglich, dass kein neuer Speicherplatz für die Ausführung des Algorithmus benötigt wird, da um wieder zu dem Beispiel einer Liste, die sortiert werden muss, zurück zukommen, die Elemente nur untereinander getauscht und keine neue Listen erstellt werden.
Ein Beispiel hierfür ist der Bubblesort Algorithmus.







<br>
<br>
Falls ich etwas vergessen habe oder sich irgendwelche Fehler eingeschlichen haben, würde ich mich freuen, wenn du mich darauf aufmerksam machst.
<br>
<br>
Quellen:<br>
https://ichi.pro/de/algorithmen-und-big-o-notation-274052038946963<br>
https://wiki.selfhtml.org/wiki/Laufzeitkomplexit%C3%A4t<br>
