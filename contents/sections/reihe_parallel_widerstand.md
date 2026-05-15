Wir stehen oft vor dem Problem, dass ein gewünschter Widerstandswert nicht in der sogenannten "Widerstands-Normreihe" enthalten ist. Es könnte auch sein, dass ein Widerstand eine große Verlustleistung umsetzen muss, die in handelsüblichen Einzelwiderständen nicht möglich ist -- um nur zwei Beispiele zu nennen. Wir werden jetzt betrachten, wie wir durch Reihenschaltung oder Parallelschaltung von Widerständen andere Widerstandswerte erhalten können.

Aus dem Ohmschen Gesetz können wir die Regeln von Reihen- und Parallelschaltungen von Widerständen herleiten:

$U=R \cdot I$

<margin>
[picture:819:e_spannungsteiler:Spannungsteiler]
</margin>

Die Abbildung [ref:e_spannungsteiler] zeigt zwei Widerstände $R_1$ und $R_2$, die hinter einander geschaltet werden. Sie vom gleichen Strom *I* durchflossen. An den Widerständen fallen dann die Spannungen

$U_1 = R_1 \cdot I$ und  $U_2 = R_2 \cdot I$ ab. 
Die Gesamtspannung $U_g$ ist einfach die Summe dieser beiden Spannungen:

$U_g = U_1 + U_2 = R_{\mathrm{ges}} \cdot {I} = R_1 \cdot I + R_2 \cdot I$

Jetzt können wir den Widerstand berechnen, der zwischen den äußeren Klemmen zu sehen ist:
$R_{\mathrm{ges}} = \frac{U_g}{I} = R_1 + R_2$, weil sich auf beiden Seiten der Gleichung der Strom $I$ rauskürzt.

Das Ganze funktioniert auch bei mehr als zwei Widerständen, wie in der Formelsammlung dargestellt:

$R_{\mathrm{ges}} = R_1 + R_2 + R_3 + R_4 + \dots$

---

Doch wie verhält es sich, wenn wir zwei Widerstände $R_1$ und $R_2$ parallel schalten wie in Abbildung [ref:e_parallelschaltung] gezeigt? 

Jetzt liegt an beiden Widerständen die selbe Spannung $U$ an, die in den Widerständen die Ströme

$I_1 = \frac{U}{R_1}$ und $I_2 = \frac{U}{R_2}$

fließen lässt. 

<margin>
[picture:945:e_parallelschaltung:In dieser Schaltung sind alle Spannungen und Ströme zu sehen.]
</margin>

Der im äußeren Stromkreis fließende Strom ist die Summe dieser beiden Ströme:

$I = I_1 + I_2 = \frac{U}{R_1} + \frac{U}{R_2}$

Wir suchen wieder einen Gesamtwiderstand $R_{\mathrm{ges}}$, für den dann gelten muss: $I=\frac{U}{R_{\mathrm{ges}}}$ und folglich:

$\dfrac{1}{R_{\mathrm{ges}}} = \dfrac{1}{R_1} + \dfrac{1}{R_2}$

---

Der Kehrwert des Gesamtwiderstands ist also die Summe der Kehrwerte der Einzelwiderstände. Eine Konsequenz ist, dass man bei einer Parallelschaltung einer Reihe gleicher Widerstände einfach den Wert des einzelnen Widerstands durch die Anzahl der Widerstände teilt.

Auch hier können wir die Berechnung für beliebig viele parallele Widerstände durchführen (vgl. Formelsammlung):

$\dfrac{1}{R_{\mathrm{ges}}} = \dfrac{1}{R_1} + \dfrac{1}{R_2} + \dfrac{1}{R_3} + \dfrac{1}{R_4} + \dots$

Den Ausdruck für zwei parallele Widerstände können wir nach den Regeln der Bruchrechnung auch schreiben als:

$R_{\mathrm{ges}} = \dfrac{R_1 \cdot R_2}{R_1 + R_2}$

<tip>
Bei der Reihenschaltung ist die Wert des Gesamtwiderstands immer größer als der größte Einzelwiderstand. Bei der Parallelschaltung ist der Gesamtwiderstand immer kleiner als der kleinste Einzelwiderstand.
</tip>

---

[question:ED104]
[question:ED105]
[question:ED106]

<tip>
Genau darauf achten, dass die in der Rechnung verwendeten Widerstände immer die selben Einheiten haben. Wir empfehlen immer, möglichst auf die Grundeinheit ($\unit{\ohm}$) zu gehen. Schalten wir z.B. einen $\qty{1}{\kilo\ohm}$- und einen $\qty{10}{\ohm}$-Widerstand in Reihe, dann rechnen wir $\qty{1000}{\ohm} + \qty{10}{\ohm} = \qty{1010}{\ohm}$.
</tip>

---

Einige der Aufgaben enthalten Widerstandsnetzwerke, in denen sowohl eine Reihen- als auch eine Parallelschaltung vorkommt. Da gehen wir so vor, dass wir erst z.B. die Parallelschaltung in einen äquivalenten Widerstand umwandeln, den wir dann mit dem in Reihe geschalteten dritten Widerstand zusammenfassen. Oder halt umgekehrt, je nach dem, was sich anhand des Schaltbildes anbietet.

<tip>
[picture:305:e_tipp_aufgabe:Beispielschaltung]

Ein wichtiges Lösungsverfahren ist die "Methode des scharfen Hinsehens" ... da gibt es zum Beispiel eine Schaltung, die einen Widerstand $R_1$ in Reihe mit zwei parallel geschalteten Widerständen $R_2$ und $R_3$ hat. Die Werte sind $R_1 = \qty{1}{\kilo\ohm}$, $R_2 = \qty{2000}{\ohm}$ und $R_3 = \qty{2}{\kilo\ohm}$. Nun sind aber $\qty{2}{\kilo\ohm} = \qty{2000}{\ohm}$. Die Parallelschaltung von $R_2$ und $R_3$ ergibt einen Widerstand, der halb so groß ist: $\qty{1000}{\ohm} = \qty{1}{\kilo\ohm}$. Den schalten wir in Reihe mit $R_1$ und erhalten das Ergebnis: $R_{\mathrm{ges}} = \qty{2}{\kilo\ohm}$.
</tip>

[question:ED111]
[question:ED110]
[question:ED112]
[question:ED113]
[question:ED108]
[question:ED109]

Bei Leistungsbetrachtungen geht man am Besten von dem bekannten Ausdruck für die Leistung aus:

$P = U \cdot I$

Bei der Reihenschaltung von z.B. drei gleichen Widerständen fließt durch alle Widerstände der gleiche Strom, aber an jedem einzelnen Widerstand fällt nur ein Drittel der äußeren Spannung ab. Bei der Parallelschaltung liegt an allen Widerständen die selbe Spannung, aber der Strom teil sich auf drei Pfade auf. In beiden Fällen verträgt also die Schaltung das dreifache der Leistung des einzelnen Widerstandes.

[question:ED107]