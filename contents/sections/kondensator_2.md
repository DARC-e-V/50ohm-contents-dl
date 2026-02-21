Das Verhalten eines Kondensators an einer Wechselspnnnung soll nun genauer betrachtet werden.

Die Strom- und Spannungsmessung an einem Kondensator mit Hilfe eines Zweikanal-Oszilloskops zeigt ein überraschendes Ergebnis, denn man sieht eine Phasenverschiebung von 90 Grad, wobei der Strom der Spannung vorauseilt.
MERKE: Kondensatooor, Strom eilt vooor!

---
[question:AC101]
<margin>
[photo:268:a_I eilt vor:Phasenverschiebung am Kondensator zwischen Spannung und Strom]
</margin>

[picture:943:a_Blindleistung Kondensator:Das Produkt von $U \cdot I$ ergibt die grüne Leistungskurve]
Die Phasenverschiebung zwischen Spannung und Strom beträgt 90 Grad, wobei der Strom voreilend ist.
Daraus ergibt sich eine Leistungskurve, die um die Nulllinie symmetrisch schwankt. Der Mittelwert ergibt Null, d.h. es wird keine Wirkleistung aufgenommen.
Wir sprechen deshalb auch bei einem verlustfreien Kondensator von Blindleistung und Blindwiderstand.

% entfernt photo:258:a_Blindleistung:Blindleistung siehe grüne Sinuskurve

[question:AC111]
Bei dieser Frage gibt es nichts zu rechnen!
Reine Wirkleistung nimmt nur ein ohmscher Widerstand auf, denn bei ihm sind Spannung und Strom immer in Phase, d.h. es gibt keine Phasenverschiebung zwischen Spannung und Strom. Ein Blindwiderstand nimmt keine Wirkenergie auf und deshalb wird er im Idealfall auch nicht warm. Sollte ein Kondensator bei Hochfrequenzanwendungen warm werden, dann hat er Verluste und muss durch einen Kondensator mit geringeren Verlusten ersetzt werden.

[question:AC103]

Wird ein Kondensator an Wechselspannung angeschlossen, dann fließt ein Wechselstrom, denn der Kondensator wird ständig geladen und entladen. Um diese Eigenschaft zu beschreiben sagen wir, der Kondensator hat einen Wechselstromwiderstand und nennen diesen Widerstand kapazitiver Blindwiderstand $X_C$.

1. Wenn die Frequenz der Wechselspannung an einem Kondesator erhöht wird, dann fließt mehr Strom, dies bedeutet, der kapazitive Blindwiderstand ist kleiner geworden. 
2. Wenn die Kapazität des Kondensators erhöht wird, dann steigt auch der Strom, d.h. der Blindwiderstand wird auch kleiner. 
Daraus ergibt sich die Berechnungsformel:
$X_C = \frac{1}{\omega \cdot C} = \frac{1}{{2\pi \cdot f \cdot C}}$

(siehe Formelsammlung Seite 236 links unten:  Stichwort: Kapazitiver Blindwiderstand)
Moderne, kostengünstige Messgeräte, die  Funkamateure heutzutage gerne einsetzen, sind Antennenanalyzer oder vektoriellen Network Analyzer (VNA). Sie messen die Veränderung des Blindwiderstandes $X_C$ in Abhängigkeit der Frequenz und können das Messergebnis auch grafisch darstellen.

[photo:248:a_kapazitiver Blindwiderstand:Kapazitiver Blindwiderstand $X_C$]
Das Abbildung [ref:a_kapazitiver Blindwiderstand] zeigt die Veränderung des kapazitiven Blindwiderstandes (blaue Linie) eines $\qty{1500}{\pico\farad}$ Styroflexkondensators im Frequenzbereich von $\qtyrange{1}{4,5}{\mega\hertz}$. Die rote Linie stellt die Phasenlage des kapazitiven Blindwiderstandes bei nahezu konstanten $\qty{-90}{\degree}$ dar.

[question:AC102]
Die blaue Linie von Abbildung [ref:a_kapazitiver Blindwiderstand] hilft zur Lösung.

---

<tip>
Kennt man den kapazitiven Blindwiderstand und die Frequenz der Wechselspannung, dann kann auch die Kapazität des Kondensators berechnet werden. 
Betrachten wir das Beispiel genauer und verwenden die Formel:
$X_C = \frac{1}{\omega \cdot C} = \frac{1}{{2\pi \cdot f \cdot C}}$
umgestellt nach C:
$C =\frac{1}{{2\pi \cdot f \cdot X_C}}$
mit eingesetzten Werten aus der Abbildung [ref:a_kapazitiver Blindwiderstand]: 

$X_C = \qty{50}{\ohm} \text{ bei } \qty{2}{\mega\hertz}$
$C = \frac{1}{6,28 \cdot 2 \cdot 10^6 \cdot 50}$
Bei der Berechnung mit dem Taschenrechner ist die Zehnerpotenz für Megahertz einzugeben.
Das Ergebnis lautet: $\qty{0,000000001592}{\farad}$
$C = \qty{1592}{\pico\farad}$
</tip>

[question:AC104]
Bei den folgenden Berechnungen von $X_C$ müssen immer die Zehnerpotenzen beachtet werden.
Die Berechnungsformel lautet: $X_C = \frac{1}{\omega \cdot C} = \frac{1}{{2\pi \cdot f \cdot C}}\\ $
Folgende Werte müssen eingesetzt werden: $\qty{10}{\pico\farad} = \qty{10e-12}{\hertz}$ und $\qty{100}{\mega\hertz} = \qty{100e6}{\hertz}$
Berechnen sie schrittweise, wenn sie unsicher sind.
Beispiel:

$\begin{split} 6,28 \cdot 10 \cdot 100 &= 6280 \\ 10^{-12} \cdot 10^6 &= 10^{-6} \\ \num{6280} \cdot 10^{-6} &= \num{0,00628} \\ 1/\num{0,00628} &= \num{159} \end{split}$

Bei den folgenden Fragen verwenden sie die gleiche Formel und ändern nur die eingesetzten Werte.
[question:AC105]

[question:AC106]

[question:AC107]

Berechnung der Kapazität aus $X_C$ und der Frequenz:
Formel: $C = \frac{1}{2\pi \cdot f \cdot X_C}$
(Siehe auch das Rechenbeispiel zum Styroflexkondensator)

[question:AC108]
Zuerst muss $X_C$ berechnet werden: $X_C = \qty{16}{\volt} / \qty{32}{\milli\ampere} = \qty{500}{\ohm}$
Danach die Formel für $C$ anwenden: $C = \frac{1}{6,28 \cdot \qty{50}{\hertz} \cdot \qty{500}{\ohm}}$
Im Ergebnis taucht die Zehnerpotenz  $10^{-6}$ auf, die in eine Vorsilbe umgewandelt werden muss.

*Kondensatorverluste*
Die vielfältigen Kondensatorarten unterscheiden sich auch hinsichtlich ihrer unerwünschten Verluste bei der Belastung durch Hochfrequenzströme. Die technische Beurteilung geschieht über den Begriff der Güte $Q$ (Quality) und dem sogenannten   tan "delta".

---
[photo:259:a_tan delta:tan "delta" verschiedener Kondensatorarten]
Hohe Verluste = niedrige Güte = großer tan "delta"
Wenn man die tan "delta" Kurven der Kondensatoren betrachtet, sieht man, dass Glimmerkondensatoren die höchste Güte = niedrigste Verluste = kleinster tan "delta" besitzen.
%todo TAN Delta Kurven neu zeichnen ???

[question:AC109]

[question:AC110]

<indepth>
Erklärung des "tan Delta" mit Hilfe eines Zeigerdiagramms:

[photo:261:a_tan delta Zeigerdiagramm:Veranschaulichung des "tan Delta" an Hand des Zeigerdiagramms für einen verlustbehafteten Kondensator.]

In aktuellen Datenblättern wird statt des "tan Delta" der serielle Verlustwiderstand (ESR) des Kondensators bei einer bestimmten Betriebsfrequenz angegeben.

[photo:260:a_Kondensator Ersatzschaltbild:Ersatzschaltbild eines realen Kondensators mit einem seriellen Verlustwiderstand (ESR).]
  
In linear geregelten Netzteilen und in Schaltnetzteilen müssen Elektrolytkondensatoren mit sehr niedrigem ESR verwendet werden.
</indepth>
<margin>
|Zusammenfassung Kondensator 2|                                                           |
|*Zusammenfassung Kondensator 2*|
|*MERKE: Kondensatooor, Strom eilt vooor!*|
|Formel Seite 236| 
| $X_C = \frac{1}{\omega \cdot C} = \frac{1}{{2\pi \cdot f \cdot C}}$|
| Umgestellt nach C:|
| $C =\frac{1}{{2\pi \cdot f \cdot X_C}}$|
|Hohe Kondensatorverluste bewirken: |
|niedrige Güte; großer tan "delta"; großer ESR|
[table:a_Kondensator 2 Zusammenfassung:Zusammenfassung Kondensatorblindwiderstand und Güte]

*Zusammenfassung*:
   *MERKE: Kondensatooor, Strom eilt vooor!*
  
 Formel Seite 236
 $X_C = \frac{1}{\omega \cdot C} = \frac{1}{{2\pi \cdot f \cdot C}}$
 Umgestellt nach C:
 $C =\frac{1}{{2\pi \cdot f \cdot X_C}}$
 Hohe Kondensatorverluste = niedrige Güte = großer tan "delta" = großer ESR


  Lösungshinweise:
*AC 104:* $\qty{159}{\ohm}$
*AC 105:* $\qty{22}{\ohm}$
*AC 106:* $\qty{15,9}{\ohm}$
*AC 107:* $\qty{3,7}{\ohm}$
*AC 108:* $\qty{6,37}{\micro\farad}$
</margin>

