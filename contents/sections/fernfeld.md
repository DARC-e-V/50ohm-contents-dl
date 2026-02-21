%Im Nahfeld einer Antenne weißen die elektrische Feldstärke und die magnetische Feldstärke keine konstante Phasenbeziehung zueinander auf. Das ändert sich erst im Fernfeld einer Antenne. Der Übergang zwischen den beiden Bereichen ist fließend, und wird auch als Übergangsfeld bezeichnet.

%Grundsätzlich ist der Übergang zwischen dem Nahfeld und dem Fernfeld abhängig von der berücksichtigten Wellenlänge. Es ist angegeben als

%$d > \dfrac {\lambda} {2 \cdot \pi}$

%Bei einer Wellenlänge von z.B. $\qty{20}{\meter}$ ist der Übergang also in etwa in einem Abstand von $d = \frac {\qty{20}{\meter}} {2 \cdot \pi} \approx \qty{3,18}{\meter}$.

%Bei Antennen, die geometrisch klein im Verhältnis zu ihrer Wellenlänge sind, kann sich das Fernfeld jedoch auch erst noch später ausbilden.

%Für die Berechnung von den Personenschutzabständen ist im Fernfeld eine Näherungformel möglich. Dies erspart einem ggf. aufwendige Messungen oder Simulation.

% ************

Das Fernfeld einer Strahlungsquelle, ist der Bereich, in dem die Vektoren der elektrischen Feldstärke (E), der magnetischen Feldstärke (H) sowie die Ausbreitungsrichtung senkrecht aufeinander stehen und keine Phasendifferenzen aufweisen. Zusätzlich muss der Feldwellenwiderstand dem des freien Raums entsprechen. 

Die Grenze zwischen Fernfeld und Nahfeld ist in erster Linie abhängig von der Wellenlänge. Jedoch spielt die Art der verwendeten Antenne und deren Umgebung durch aus eine Rolle. Bei den im Amateurfunk überwiegend verwendeten Drahtantennen (z.B. Dipole) bildet sich das Fernfeld in einem Abstand von etwa $4\cdot\lambda$ aus. 

Das Nahfeld unterteilt sich in das reaktive und das strahlende Nahfeld. Praktisch ist, dass im strahlenden Nahfeld trotzdem die Formel für das Fernfeld verwendet werden kann. Das liegt daran, dass die Näherungsformel hier sehr konservative Abschätzungen liefert, das heißt die tatsächlichen Feldstärken sind geringer als die errechneten. Man ist auf der sicheren Seite. Dies gilt aber nicht für magnetische Antennen und Antennen, die sehr kurz im Verhältnis zur Wellenlänge sind. In diesen Fällen muss auf andere Verfahren zurück gegriffen werden z.B. Nahfeldberechnungsprogramme.

Der Übergang zwischen dem reaktiven Nahfeld und dem strahlenden Nahfeld ist abhängig von der Wellenlänge. 

$d > \dfrac {\lambda} {2 \cdot \pi}$

Die Berechnung mit der Näherungformel erspart einem ggf. aufwendige Messungen oder Simulationen.

Die Formel $d = \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_{\textrm{EIRP}}}}{E}$ gilt für die meisten Antennenformen, wenn der berechnete Sicherheitsabstand im strahlenden Nahfeld oder im Fernfeld liegt.

<indepth>
In den [Erläuterung der Bewertungsverfahren nach BEMFV](https://50ohm.de/bemfv)  hat die BNetzA die Begriffe und Verfahren für die Ermittlung der Sicherheitsabstände erläutert.
% Bild von DL4HR
[photo:80:n_Bewertungsverfahren:In diesem Dokument sind die Bewertungsverfahren beschrieben.]
</indepth>