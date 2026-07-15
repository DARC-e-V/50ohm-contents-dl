Das elektromagnetische Feld einer Antenne lässt sich, wie in Abbildung [ref:a_nahfernfeld] dargestellt, in das *Nahfeld* in unmittelbarer Umgebung der Antenne und das weiter entfernte *Fernfeld* unterteilen. Das Nahfeld wird zusätzlich in das *reaktive Nahfeld* und das *strahlende Nahfeld* gegliedert.

<tip>
In den [Erläuterungen der Bewertungsverfahren nach BEMFV](https://50ohm.de/bemfv) hat die BNetzA die Begriffe und Verfahren für die Ermittlung der Sicherheitsabstände erläutert.
[photo:80:n_Bewertungsverfahren:In diesem Dokument sind die Bewertungsverfahren beschrieben.]
</tip>

[picture:1113:a_nahfernfeld:Abstandsdefinitionen für Nahfeld und Fernfeld nach der Bundesnetzagentur (BNetzA).]

---

Nach der in der Abbildung verwendeten Definition der Bundesnetzagentur (BNetzA) erstreckt sich das reaktive Nahfeld bis zu einem Abstand von

$d \le \dfrac{\lambda}{2 \cdot \pi}$

von der Antenne, wobei $\lambda$ die Wellenlänge bezeichnet. Bei größeren Abständen beginnt das strahlende Nahfeld. Der Abstand dieser Grenze ist somit von der Wellenlänge abhängig. Bei einer Wellenlänge von beispielsweise $\qty{20}{\meter}$ ergibt sich:

$d = \frac{\qty{20}{\meter}}{2 \cdot \pi} \approx \qty{3,18}{\meter}$

Das reaktive Nahfeld reicht in diesem Beispiel also bis zu einem Abstand von etwa $\qty{3,18}{\meter}$ von der Antenne.

Im reaktiven Nahfeld einer Antenne weisen die elektrische Feldstärke und die magnetische Feldstärke keine konstante Phasenbeziehung zueinander auf. Was das genau bedeutet, wird in der nebenstehenden Vertiefung genauer erklärt. 

[question:AK101]

Schaut man sich den Verlauf des elektrischen und magnetischen Feldes für eine Dipolantenne über diese Bereiche in Abbildung [ref:a_dipol_feld_e_h] an, so erkennt man, dass die beiden Feldgrößen nicht die gleichen Beträge haben. Das elektrische Feld ist wesentlich stärker als das magnetische Feld. Bei einer magnetischen Loop-Antenne in Abbildung [ref:a_loop_feld_e_h] ist es genau umgekehrt: Das magnetische Feld ist wesentlich stärker als das elektrische Feld.

<margin>
[picture:1114:a_dipol_feld_e_h:Verlauf der elektrischen und magnetischen Feldstärke einer Dipolantenne über die Bereiche Nahfeld und Fernfeld (Logarithmisch).]
[picture:1115:a_loop_feld_e_h:Verlauf der elektrischen und magnetischen Feldstärke einer Loopantenne über die Bereiche Nahfeld und Fernfeld (Logarithmisch).]
</margin>

<indepth>
Für mathematisch Interessierte, die bereits mit komplexen Zahlen vertraut sind, soll hier vereinfacht erklärt werden, warum elektrische und magnetische Feldstärke im reaktiven Nahfeld keine ortsunabhängige Phasenbeziehung zueinander besitzen.
Bei einem elektrisch kurzen Dipol setzen sich die Felder vereinfacht aus mehreren Anteilen zusammen:

$ \underline{E}(r)~=~\left( \underbrace{\frac{A}{r^3}}_{\text{quasistatisch}} + \underbrace{j\,\frac{B}{r^2}}_{\text{induktiv}} + \underbrace{\frac{C}{r}}_{\text{Strahlung}} \right) e^{-jkr}$

$ \underline{H}(r)~=~\left( \underbrace{j\,\frac{D}{r^2}}_{\text{induktiv}} + \underbrace{\frac{F}{r}}_{\text{Strahlung}} \right) e^{-jkr}. $

Die unterstrichenen Größen sind komplex und beschreiben neben der Stärke auch die Phase der jeweiligen Feldanteile. Faktoren wie $j$ oder $-j$ in den vollständigen Feldgleichungen entsprechen dabei Phasenverschiebungen von $\qty{90}{\degree}$ beziehungsweise $\qty{-90}{\degree}$.

Da die einzelnen Anteile unterschiedlich schnell mit dem Abstand $r$ abnehmen, verändert sich ihr Verhältnis zueinander. Dadurch hängt auch die Phasendifferenz zwischen elektrischer und magnetischer Feldstärke im Nahfeld vom Abstand, von der Richtung und von der Antennenform ab.

Für ein vollständiges Verständnis sind die einzelnen Vektorkomponenten der Feldgleichungen zu betrachten. Diese Zusammenhänge gehen deutlich über die Lerninhalte der Klasse A hinaus und sind für die Prüfung nicht relevant.
</indepth>

Insbesondere im reaktiven Nahfeld können aufgrund der starken, mit zunehmendem Abstand rasch abfallenden elektrischen oder magnetischen Feldanteile hohe lokale Feldstärken auftreten. Dieser Bereich wird als *reaktiv* bezeichnet, weil ein großer Teil der Feldenergie nicht dauerhaft abgestrahlt wird, sondern zwischen Antenne und Feld hin- und herpendelt und zur Antenne zurückkehrt. Genau wie bei einem Kondensator (elektrisches Feld) oder einer Spule (magnetisches Feld) wird die im reaktiven Nahfeld gespeicherte Energie nicht verbraucht, sondern phasenverschoben zur Antenne zurückgegeben – dieses Pendeln zwischen Feld und Antenne entspricht dem Blindanteil der Antennenimpedanz, während nur der Wirkanteil (Strahlungswiderstand) tatsächlich abgestrahlte Leistung beschreibt.

Im *strahlenden Nahfeld* im Bereich

$\frac{\lambda}{2\pi} < d < 4\cdot\lambda$

treten die abgestrahlten Feldanteile zunehmend in den Vordergrund. Elektrische und magnetische Feldstärke nähern sich dabei in ihrem Verhältnis immer mehr den Verhältnissen im Fernfeld an. Die Antenne strahlt allerdings nicht erst in diesem Bereich, sondern bereits grundsätzlich; lediglich die reaktiven Feldanteile verlieren mit zunehmendem Abstand an Bedeutung. Für viele vereinfachte Betrachtungen kann das strahlende Nahfeld bereits ähnlich wie das Fernfeld behandelt werden. Darauf gehen wir später noch genauer ein.

Das *Fernfeld* beginnt nach der hier verwendeten Definition bei einem Abstand von

$d \ge 4\cdot\lambda$

von der Antenne. In diesem Bereich nehmen die elektrische und die magnetische Feldstärke jeweils proportional zu $\frac{1}{d}$ ab. Außerdem stehen beide Feldkomponenten in einem festen Verhältnis zueinander und besitzen eine konstante Phasenbeziehung.

---

Das Verhältnis der Beträge von elektrischer und magnetischer Feldstärke wird als *Feldwellenwiderstand* bezeichnet:

$Z_\mathrm{F}(d)=\left|\frac{E(d)}{H(d)}\right|$

Abbildung [ref:a_feldwellenwiderstand] zeigt, wie sich der Feldwellenwiderstand mit zunehmendem Abstand von der Antenne verändert. Im reaktiven Nahfeld hängt er stark von der Antennenform, der betrachteten Richtung und dem Abstand ab. Er kann dort deutlich größer oder kleiner als der Feldwellenwiderstand des freien Raums sein.

Im strahlenden Nahfeld nähert sich das Verhältnis von elektrischer und magnetischer Feldstärke zunehmend dem Wert des freien Raums an. Im Fernfeld ist er schließlich konstant und beträgt näherungsweise:

$Z_0 = \sqrt{\dfrac{\mu_0}{\varepsilon_0}} \approx \qty{120\pi}{\ohm} \approx \qty{377}{\ohm}$

Der Feldwellenwiderstand des freien Raums verknüpft die elektrischen und magnetischen Feldgrößen miteinander. Er ist ein Maß dafür, wie stark die elektrische Feldstärke im Verhältnis zur magnetischen Feldstärke ist. 

[question:AK102]

Diesen Wert müssen wir uns merken, da wir ihn zur Herleitung der Näherungsformel benötigen. 

Wir fassen zusammen: 

* Das Fernfeld einer Strahlungsquelle ist der Bereich, in dem die Vektoren der elektrischen Feldstärke (E), der magnetischen Feldstärke (H) sowie die Ausbreitungsrichtung senkrecht aufeinander stehen und keine Phasendifferenzen aufweisen. Zusätzlich muss der Feldwellenwiderstand dem des freien Raums entsprechen. 
* Die Grenze zwischen Fernfeld und Nahfeld ist in erster Linie abhängig von der Wellenlänge. Jedoch spielt die Art der verwendeten Antenne und deren Umgebung durchaus eine Rolle. Bei den im Amateurfunk überwiegend verwendeten Drahtantennen (z.B. Dipole) bildet sich das Fernfeld in einem Abstand von etwa $4\cdot\lambda$ aus. 

<margin>
[picture:1116:a_feldwellenwiderstand:Verlauf des Feldwellenwiderstands über die Bereiche Nahfeld und Fernfeld (Logarithmisch).]
</margin>