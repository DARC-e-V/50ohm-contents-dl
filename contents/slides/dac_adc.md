## A/D- und D/A-Umsetzung

* *A/D-Umsetzer* wandeln analoge Signale in digitale Werte um
* *D/A-Umsetzer* wandeln digitale Werte wieder in analoge Signale um
* Beide besitzen nur eine endliche Anzahl möglicher Werte
* Eine wichtige Eigenschaft ist daher ihre *Auflösung*

<note>
A/D- und D/A-Umsetzer bilden die Schnittstelle zwischen der analogen und der digitalen Welt.

Der A/D-Umsetzer erzeugt aus einem analogen Eingangssignal digitale Samples. Der D/A-Umsetzer führt den umgekehrten Vorgang aus und erzeugt aus digitalen Werten wieder analoge Spannungswerte.
</note>

---
## Quantisierung im A/D-Umsetzer

* Der A/D-Umsetzer kann nur eine begrenzte Anzahl digitaler Werte erzeugen
* Analoge Eingangswerte werden daher festen Stufen zugeordnet
* Zwischenwerte können nicht exakt dargestellt werden
* Dadurch entsteht ein *Quantisierungsfehler*

<note>
Die Quantisierung haben wir bereits kennengelernt.

Ein tatsächlich gemessener analoger Wert liegt häufig zwischen zwei möglichen digitalen Stufen. Der A/D-Umsetzer muss ihn einer dieser Stufen zuordnen.

Die dabei entstehende Abweichung zwischen dem tatsächlichen und dem dargestellten Wert bezeichnet man als Quantisierungsfehler.
</note>

---

[question:AF607]

---
## Auflösung eines A/D-Umsetzers

* Die Auflösung gibt die Anzahl der unterscheidbaren digitalen Werte an
* Sie wird üblicherweise in *Bit* angegeben
* $\qty{8}{\bit}$ → $\num{256}$ mögliche Werte
* $\qty{16}{\bit}$ → $\num{65536}$ mögliche Werte
* Mehr Bit ermöglichen eine feinere Darstellung der Signalamplitude

---
## Einfluss der Auflösung

<left>
[picture:300:a_adc_4bit:Sinussignal digitalisiert durch einen 4-Bit-A/D-Umsetzer und anschließende D/A-Umsetzung]
</left>
<right>
[picture:299:a_adc_12bit:Sinussignal digitalisiert durch einen 12-Bit-A/D-Umsetzer und anschließende D/A-Umsetzung]
</right>

* $\qty{4}{\bit}$ → $\num{16}$ mögliche Werte
* $\qty{12}{\bit}$ → $\num{4096}$ mögliche Werte
* Höhere Auflösung → kleinere Quantisierungsstufen

<note>
Hier lässt sich der Einfluss der Auflösung direkt vergleichen.

Bei 4 Bit stehen nur 16 mögliche Werte zur Verfügung. Die Abstufung ist im rekonstruierten Signal deutlich zu erkennen.

Bei 12 Bit stehen bereits 4096 mögliche Werte zur Verfügung. Das rekonstruierte Signal kommt dem ursprünglichen Sinussignal daher wesentlich näher.

Durch die zusätzlichen 8 Bit steigt die Anzahl der möglichen Stufen um den Faktor 256.
</note>

---

[question:AF608]

---
## Jitter

* Die Samples sollten zu exakt festgelegten Zeitpunkten aufgenommen werden
* In der Praxis können die tatsächlichen Abtastzeitpunkte geringfügig schwanken
* Diese zeitlichen Abweichungen bezeichnet man als *Jitter*
* Jitter kann zusätzliches Rauschen im digitalisierten Signal verursachen

<note>
Nicht nur die Genauigkeit der gemessenen Amplitude ist wichtig, sondern auch die Genauigkeit des Abtastzeitpunktes.

Dazu benötigt der A/D-Umsetzer einen möglichst stabilen Takt. Kleine zeitliche Schwankungen dieses Taktes führen dazu, dass die Samples nicht exakt zu den vorgesehenen Zeitpunkten aufgenommen werden.

Diese Schwankungen werden als Jitter bezeichnet.
</note>

---

[question:AF621]

---
## D/A-Umsetzer

* Der D/A-Umsetzer ist der Gegenspieler des A/D-Umsetzers
* Er erzeugt aus digitalen Samples analoge Spannungswerte
* Auch ein D/A-Umsetzer besitzt nur eine endliche Anzahl möglicher Ausgangswerte
* Seine Auflösung wird ebenfalls in Bit angegeben

<note>
Beim D/A-Umsetzer läuft der Vorgang in umgekehrter Richtung.

Ein digitaler Zahlenwert wird einem bestimmten analogen Ausgangswert zugeordnet. Auch hier bestimmt die Auflösung, wie viele unterschiedliche Werte erzeugt werden können.
</note>

---

[question:AF609]

---
## Spannungsbereich und Auflösung

* Ein D/A-Umsetzer besitzt einen festgelegten Spannungsbereich
* Beispiel: $\qty{0}{\volt}$ bis $\qty{1}{\volt}$
* Bei $\qty{4}{\bit}$ stehen $\num{2^4}=\num{16}$ mögliche Stufen zur Verfügung
* Bei einem linearen D/A-Umsetzer sind diese gleichmäßig über den Spannungsbereich verteilt

---
## Schrittweite

Bei $\num{16}$ Stufen gibt es $\num{15}$ Abstände zwischen den Stufen.

Für einen Spannungsbereich von $\qty{0}{\volt}$ bis $\qty{1}{\volt}$ ergibt sich:

$\frac{\qty{1}{\volt}}{16-1}\approx\qty{67}{\milli\volt}$

<fragment>
Die Schrittweite beträgt somit etwa $\qty{67}{\milli\volt}$.
</fragment>

<note>
Hier muss man beachten, dass zwischen 16 möglichen Spannungswerten nur 15 Abstände liegen.

Das entspricht dem bekannten Zaunpfahlproblem: Zwischen 10 Zaunpfählen befinden sich nur 9 Zwischenräume.

Deshalb wird bei diesem Beispiel der Spannungsbereich durch 15 und nicht durch 16 geteilt.
</note>

---

[question:AF611]

---

[question:AF610]

---
## A/D- und D/A-Umsetzer im SDR

* A/D-Umsetzer digitalisieren analoge Eingangssignale
* Anschließend können die Samples digital verarbeitet werden
* D/A-Umsetzer erzeugen daraus bei Bedarf wieder analoge Signale
* Dieses Prinzip wird an vielen Stellen in SDR-Empfängern und Transceivern eingesetzt

<note>
Ein SDR ist ein typisches Beispiel für das Zusammenspiel von A/D-Umsetzung, digitaler Signalverarbeitung und D/A-Umsetzung.

Das analoge Signal wird zunächst digitalisiert. Danach können beispielsweise Filterung, Demodulation oder Modulation digital erfolgen. Soll anschließend wieder ein analoges Signal entstehen, kommt ein D/A-Umsetzer zum Einsatz.
</note>

---
## Nutzung des Wertebereichs

* Ein kleines Eingangssignal nutzt nur einen Teil der verfügbaren Stufen
* Ein zu großes Eingangssignal überschreitet den darstellbaren Wertebereich
* Werte oberhalb des Maximums können nicht mehr korrekt dargestellt werden
* Das Signal wird an dieser Stelle abgeschnitten

<fragment>
Diesen Effekt bezeichnet man als *Clipping*.
</fragment>

<note>
Für eine möglichst gute Digitalisierung sollte der verfügbare Wertebereich sinnvoll ausgenutzt werden.

Ist das Signal sehr klein, werden nur wenige der verfügbaren Stufen genutzt.

Ist das Signal dagegen zu groß, erreicht der A/D-Umsetzer seinen maximal darstellbaren Wert. Noch größere Eingangswerte können nicht mehr unterschieden werden. Die Spitzen des Signals erscheinen dadurch abgeschnitten.

Auch ein D/A-Umsetzer kann keine Ausgangsspannung außerhalb seines vorgesehenen Wertebereichs erzeugen.
</note>

---
## Einfluss der Auflösung

* Hohe Auflösung → viele mögliche Amplitudenwerte
* Niedrige Auflösung → wenige mögliche Amplitudenwerte
* Mehr Stufen ermöglichen eine genauere Digitalisierung und Rekonstruktion
* Der verfügbare Wertebereich sollte möglichst gut genutzt werden

---

[question:AF613]

---

[question:AF612]

---

[question:AF614]