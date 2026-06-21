## Erklärung

### Quelle zur Berechnung des Sicherheitsabstands

Das Dokument "Erläuterung der Bewertungsverfahren nach BEMFV" der Bundesnetzagentur vom August 2013 gibt Aufschluss.

Der Abschnitt 1.2.2 (Durchführung der Fernfeldberechnung) enthält die Formel (5) zur Berechnung des Sicherheitsabstands - hier mit $r$ bezeichnet:

$r = \sqrt(\frac{Z_0}{4 \cdot \pi}) \cdot \frac{\sqrt{P \cdot G_i}}{E_g} \cdot C$

Mit $Z_0 = \qty{120\pi}{\Ohm}$ lässt sich der erste Faktor zu $\sqrt{\qty{30}{\Ohm}}$ vereinfachen. Vernachlässigt man den Verlustfaktor $C$, erhält man die in der Aufgabenstellung und den Hilfsmitteln der Bundesnetzagentur angegebene Formel zur Berechnung des Sicherheitsabstands:

$d = \frac{\sqrt{\qty{30}{\Ohm} \cdot P_\mathrm{EIRP}}}{E}$

Abschnitt 1.2.1 besagt, dass die oben angegebene Formel zur Berechnung des Sicherheitsabstands nur im Fernfeld einer Strahlungsquelle gültig ist.

Weiterhin wird dort zwischen dem *reaktiven Nahfeld* und dem *strahlenden Nahfeld* unterschieden.

### Reaktives Nahfeld

Man befindet sich im reaktiven Nahfeld einer Antenne, wenn der Abstand zur Antenne 

$d < \frac{\lambda}{2\pi}$ 

beträgt. Hier gilt:

"Innerhalb des reaktiven Nahfeldes kann es lokal zu starken Überhöhungen des elektrischen und des magnetischen Feldes kommen, die mit der Fernfeldberechnung nicht bestimmt werden können. Daher ist eine Fernfeldberechnung in diesem Bereich nicht zulässig."

### Strahlendes Nahfeld

Man befindet sich im strahlenden Nahfeld einer Antenne, wenn 

* man sich außerhalb des reaktiven Nahfeldes befindet und
* der Abstand zur Antenne weniger als $4 \lambda$ beträgt.

Hier gilt:

"Wenn die Fernfeldformel im Bereich des strahlenden Nahfeldes angewendet wird, ergeben sich für die meisten Antennenformen konservative Abschätzungen, das heißt die tatsächlichen Feldstärken sind geringer als die errechneten. Dies gilt jedoch nicht für alle Antennenarten, so erzeugt beispielsweise eine magnetische Antenne im Nahfeld stärkere Feldstärken, als die durch die Fernfeldformel vorausgesagten. Insbesondere Antennen, die geometrisch klein im Verhältnis zur Wellenlänge sind, zeigen ein solches Verhalten."

### Nahfeldberechnungen

Abschnitt 1.3 geht auf die Möglichkeit der Nahfeldberechnung durch Simulation ein:

"Durch die Verwendung numerischer Verfahren, wie sie in so genannten Nahfeldberechnungsprogrammen angewendet werden, ist es möglich, die elektrischen und magnetischen Felder exakt nach Betrag und Phase für beliebige Raumpunkte im Umfeld einer Antenne zu berechnen."

### Interpretation

Aus den Erläuterungen zum reaktiven und strahlenden Nahfeld sowie zu den Nahfeldberechnungen lässt sich die oben genannte Antwort begründen.

