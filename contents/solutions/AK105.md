## Teil 1 des Lösungsansatzes
Der Formelsammlung in den Hilfsmitteln der Bundesnetzagentur kann im Kapitel "Pegel" entnommen werden, dass $\qty{-6}{\dB}$-Dämpfung im Leistungsverhältnis dem Faktor 0,25 entspricht.

In Formeln ausgedrückt:

$P_{\qty{40}{^\circ}} = 0{,}25 \cdot P_\mathrm{EIRP}$

## Teil 2 des Lösungsansatzes
Der Formelsammlung in den Hilfsmitteln der Bundesnetzagentur kann im Kapitel "Strahlungsleistung und Gewinn" von Antennen die folgende Formel entnommen werden:

$E = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{d}$

Da ein Sicherheitsabstand ermittelt werden soll, muss die Formel nach $d$ umgestellt werden:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E}$

## Einsetzen

$d_{\qty{40}{^\circ}} = \frac{\sqrt{\qty{30}{\ohm} \cdot P_{\qty{40}{^\circ}}}}{E} = \frac{\sqrt{\qty{30}{\ohm} \cdot 0,25 \cdot P_\mathrm{EIRP}}}{E} = \frac{\sqrt{0,25} \cdot \sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E} = \sqrt{0,25} \cdot \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E} = 0,5 \cdot \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E} = 0,5 \cdot d$

## Interpretation der Formel

Der Sicherheitsabstand bei $\qty{40}{^\circ}$ halbiert sich im Vergleich zum Sicherheitsabstand in Hauptstrahlrichtung. 
Er verringert sich damit vom vorgegeben Wert $\qty{20}{\meter}$ auf den gesuchten Wert von $\qty{10}{\meter}$.
