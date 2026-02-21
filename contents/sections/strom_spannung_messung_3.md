In den Klassen N und E haben wir bereits gelernt, wie man Strom und Spannung korrekt misst und welche Eigenschaften die Innenwiderstände der Messgeräte haben. Werden die Messgeräte nicht richtig in die Schaltung eingebaut, erhält man falsche oder unsinnige Anzeigen oder kann im schlimmsten Fall das Messgerät beschädigen. In der Klasse A gibt es dazu noch zwei weitere Fragen, die die korrekte Strom- und Spannungsmessung abprüfen – allerdings in einem etwas komplexeren Kontext.

Bei der ersten Frage geht es um die Leistungsmessung eines Verstärkers (Power Amplifier, PA). Den Zusammenhang $P = U \cdot I$ kennen wir bereits: Die Leistung lässt sich bestimmen, indem man Spannung und Strom misst und anschließend beide Werte multipliziert. In Abbildung [ref:a_strom_spannung_messung] ist links die Spannungsversorgung in Form eines Netzteils angeschlossen, in der Mitte befindet sich die PA und rechts ist ein weiterer Verbraucher, der Sender (TRX), angeschlossen. Möchten wir nun die Leistung der PA ermitteln, darf ausschließlich der Strom gemessen werden, der in die PA fließt.

<margin>
[picture:1003:a_strom_spannung_messung:Messen der Leistung eines Verstärkers (PA)]
</margin>

[question:AI101]

Für die nächste Frage erinnern wir uns an die Regeln aus der Klasse E, dass Spannungsmessgeräte immer arallel und Strommessgeräte immer in Reihe geschaltet werden. Dadurch ist die Frage sehr leicht zu lösen. 

[question:AI102]

---

Im Folgenden wollen wir uns zwei Kenngrößen beim Messen ansehen, die oft verwechselt werden:

- Auflösung
- Messgenauigkeit (auch Toleranz oder Fehler genannt)

Die *Auflösung* oder bezeichnet die kleinste Änderung der Messgröße, die ein Gerät noch anzeigen kann. Beispiel: Ein Multimeter mit einer Auflösung von $\qty{0,1}{\volt}$ kann zwischen $\qty{10,5}{\volt}$ und $\qty{10,45}{\volt}$ nicht unterscheiden, wenn der Unterschied kleiner ist als die Auflösung. Ein Gerät mit $\qty{0,01}{\volt}$ Auflösung kann hingegen deutlich feiner unterscheiden. Die Auflösung wird in der Regel vom Hersteller des Messgeräts angegeben.

<tip>
Betrachten wir zunächst die *Auflösung* anhand einer Uhr. Besitzt die Uhr eine Stunden- und Minutenanzeige, so lässt sich die Zeit auf eine Minute genau angeben. Aber ob es nun 13 Uhr 3 Minuten und 10 Sekunden ist oder 13 Uhr 3 Minuten und 59 Sekunden lässt sich nicht ablesen. *Eine Minute* ist also die *kleinste Auflösung* der Uhr (entsprechend hat eine Uhr mit einem Sekundenzeiger eine kleinste Auflösung von einer Sekunde).
</tip>

Die *Messgenauigkeit* (auch Messfehler oder Toleranz) eines Geräts beschreibt, wie stark der angezeigte Wert höchstens vom tatsächlichen Wert abweichen darf – sowohl nach oben als auch nach unten, zum Beispiel $\pm\qty{5}{\percent}$. Eine einfache Faustregel lautet: Je größer der Messbereich ist, den ein Gerät abdecken soll, desto geringer ist in der Regel die Genauigkeit der Messung.

Die Messgenauigkeit hängt unter anderem vom Innenwiderstand des Messgeräts ab, da dieser das Messergebnis beeinflusst.
In der Klasse E haben wir gelernt: Ein Strommessgerät hat einen sehr geringen Innenwiderstand (ideal $\qty{0}{\ohm}$), ein Spannungsmessgerät dagegen einen sehr hohen Innenwiderstand (ideal $\qty{\infty}{\ohm}$). In der Klasse A wollen wir uns nun zusätzlich anschauen, wie genau unsere Messgeräte die tatsächlich anliegende Spannung bzw. Stromstärke erfassen können. Der angezeigte Messwert unterscheidet sich nämlich in der Regel vom tatsächlichen Wert – und das liegt an den nicht perfekten Innenwiderständen der Messgeräte, welche die Messung beeinflussen.

---

Schauen wir uns das Ersatzschaltbild eines realen Spannungsmessgeräts in Abbildung [ref:a_reale_spannungsmessung] zur folgenden Prüfungsfrage an. Neben dem idealen Strommesser enthält ein reales Spannungsmessgerät einen parallelgeschalteten Widerstand, z. B. von $\qty{10}{\mega\ohm}$. Wäre dieser Widerstand unendlich groß, existierte er praktisch nicht – und wir hätten ein ideales Messgerät. Das bedeutet jedoch, dass bei einer realen Spannungsmessung immer ein kleiner Strom durch diesen Widerstand fließt, der unser Messergebnis beeinflusst. Stellen wir uns beispielsweise vor, wir wollen die Spannung an einem Spannungsteiler messen: Durch den Innenwiderstand des Messgeräts wird der Spannungsteiler geringfügig belastet, sodass wir nicht exakt die Spannung messen, die ein ideales Messgerät anzeigen würde. 

<margin>
[picture:1004:a_reale_spannungsmessung:Ersatzschaltbild reales Spannungsmessgerät]
</margin>

---

Ähnlich wie beim Spannungsmessgerät verhält es sich auch beim Strommessgerät. Ein reales Strommessgerät besteht aus dem eigentlichen Strommesser und einem kleinen Widerstand, der in Reihe geschaltet ist und an dem immer eine kleine Spannung abfällt. Wäre dieser Widerstand null, würde er praktisch nicht existieren – und wir hätten wieder das ideale Messgerät.

<margin>
[picture:1007:a_reale_strommessung:Ersatzschaltbild reales Strommessgerät]
</margin>

---

[question:AI104]

<tip>
Bei dieser Frage ist der Hinweis "Kleinste Auflösung $\qty{100}{\micro\volt}$" nicht wichtig. Sie kann allein mit Hilfe des Ohmschen Gesetzes gelöst werden.
</tip>

---

Wie verhält es sich nun mit Kenngrößen, die aus Messwerten berechnet werden – etwa der Leistung in unserem Beispiel vom Anfang ($P = U \cdot I$) nach einer Strom- und Spannungsmessung? Die einzelnen Messgrößen wie Strom und Spannung weichen durch Messfehler jeweils vom tatsächlichen Wert ab, und diese Abweichungen wirken sich in der Berechnung entsprechend fort.

Schauen wir uns ein konkretes Beispiel an: Angenommen, wir möchten die Leistung bestimmen und messen dazu eine Gleichspannung und einen Gleichstrom. Beide Messgeräte zeigen Werte an, die jeweils um fünf Prozent zu niedrig sind. Man darf nun nicht den Fehler machen und die Abweichungen der Einzelmessgrößen einfach addieren. Durch die Leistungsformel wird deutlich, dass sich die Fehler in diesem Fall multiplizieren. Schauen wir uns das im Detail an:

$U_\text{Gemessen}=0,95 \cdot U_\text{Wahr}$ und $I_\text{Gemessen}=0,95 \cdot I_\text{Wahr}$

Die Leistung berechnen wir mit unserer bekannten Formel:

$P_\text{Gemessen}=U_\text{Gemessen} \cdot I_{Gemessen}$

Nun setzen wir die wahren Werte ein: 

$P_\text{Gemessen} = 0,95 \cdot U_\text{Wahr} \cdot 0,95 \cdot I_\text{Wahr} = 0,9025 \cdot U_\text{Wahr} \cdot I_\text{Wahr}$

Das heißt, die gemessene Leistung ist etwa $\qty{9,75}{\percent}$ niedriger als die tatsächliche Leistung, denn $1-0,9025 \equiv \qty{9,75}{\percent}$. Mit diesem Wissen ist die folgende Prüfungsfrage lösbar, die konkreten Werte von Strom und Spannung sind für die Lösung nicht relevant.

[question:AI103]
