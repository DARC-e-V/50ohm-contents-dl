Die Verbindung in der Mitte sorgt dafür, dass die beiden mittleren Punkte elektrisch identisch sind.

Dadurch liegen:

* $R_1$ und $R_3$ parallel zwischen a und dem Mittelpunkt
* $R_2$ und $R_4$ parallel zwischen Mittelpunkt und b

Die Schaltung besteht also aus zwei Parallelschaltungen, die anschließend in Reihe liegen.

Zuerst werden $R_1$ und $R_3$ zusammengefasst:

$ R_{13} = \frac{R_1 \cdot R_3}{R_1 + R_3} $

Da beide Widerstände gleich groß sind:

$ R_{13} = \frac{\qty{2,2}{\kilo\ohm}}{2} = \qty{1,1}{\kilo\ohm} $

Nun werden $R_2$ und $R_4$ zusammengefasst:

$ R_{24} = \frac{R_2 \cdot R_4}{R_2 + R_4} $

Auch diese Widerstände sind gleich groß:

$ R_{24} = \frac{\qty{220}{\ohm}}{2} = \qty{110}{\ohm} $

Beide Ersatzwiderstände liegen in Reihe:

$ R_\mathrm{ges} = R_{13} + R_{24} = \qty{1100}{\ohm} + \qty{110}{\ohm} = \qty{1210}{\ohm} $