Wir haben nun den Widerstand und seine Einheit $\unit{\ohm}$ (Ohm) kennengelernt. In der Praxis wird auf Widerständen allerdings meistens nicht der Zahlenwert aufgedruckt. Stattdessen werden Farbringe verwendet. Diese Farbringe kodieren den Wert des Widerstandes.

<margin>
[picture:665:n_widerstandsfarbcodes: Ein Widerstand mit 4 Farbringen]
</margin>

Die Abbildung [ref:n_widerstandsfarbcodes] zeigt einen Widerstand mit vier Farbringen. Jede Farbe entspricht dabei einem Zahlenwert, wie in der Tabelle [ref:n_widerstandsfarbcodes_tabelle] in der Spalte *Wert* gezeigt:
* Der erste Farbring entspricht der ersten Ziffer, in diesem Fall *gelb*, also vier.
* Der zweite Farbring entspricht der zweiten Ziffer, in unserem Beispiel also *violett*, also sieben.
* Der dritte Farbring ist der sogenannte Multiplikator (siehe Tabelle [ref:n_widerstandsfarbcodes_tabelle], in unserem Fall *orange*, also der Wert 1000.

<webmargin>
| X:Farbe | l:Wert | l:Multiplikator | l:Toleranz |
| Silber | - | $\num{0,01}$ | $\qty{\pm 10}{\percent}$ |
| Gold | - | $\num{0,1}$ | $\qty{\pm 5}{\percent}$ |
| Schwarz | 0 | $\num{1}$ | - |
| Braun | 1 | $\num{10}$ | $\qty{\pm 1}{\percent}$ |
| Rot | 2 | $\num{100}$ | $\qty{\pm 2}{\percent}$ |
| Orange| 3 | $\num{1000}$ | - |
| Gelb | 4 | $\num{10000}$ | - |
| Grün | 5 | $\num{100000}$ | - |
| Blau | 6 | $\num{1000000}$ | $\qty{\pm 0,25}{\percent}$ |
| Violett | 7 | $\num{10000000}$ | $\qty{\pm 0,1}{\percent}$ |
| Grau | 8 | $\num{100000000}$ | - |
| Weiß | 9 | $\num{1000000000}$ | - |
| Keine | - | - | $\qty{\pm 20}{\percent}$ |
[table:n_widerstandsfarbcodes_tabelle:Widerstandsfarbcodes Tabelle]
</webmargin>

Der erste und der zweite Ring zusammen ergeben die Zahl 47. Wenn man diese Zahl mit dem Multiplikator multipliziert, kann man den Wert des Widerstandes berechnen:

$ 47 \cdot \qty{1000}{\ohm} = \qty{47000}{\ohm} = \qty{47}{\kilo\ohm} $

---

Es bleibt noch ein vierter Farbring übrig. Dieser steht für die sogenannte Toleranz, die angibt, wie stark der tatsächliche Widerstandswert vom dem aufgedruckten Wert abweichen darf.
Weitere Details dazu folgen in der Klasse E. 

<indepth>
*Vertiefung:* In unserem Beispiel ist der letzte Ring *silber*, was eine Toleranz von $\qty{\pm 10}{\percent}$ bedeutet. Der wahre Wert des Widerstandes kann $\qty{10}{\percent} \cdot \qty{47}{\kilo\ohm} = \qty{4,7}{\kilo\ohm}$ mehr oder weniger als der angegebene Wert sein. Er kann also zwischen $\qty{42,3}{\kilo\ohm}$ und $\qty{51,7}{\kilo\ohm}$ liegen.
</indepth>

---

Die Tabelle mit den Farbcodes muss man nicht auswendig lernen. Sie liegt als Teil der Formelsammlung bei der Prüfung als Hilfsmittel bereit. Man sollte sich allerdings die Anordnung der Ringe und ihre Bedeutung merken. Zur Übung können die folgenden Fragen mithilfe des Farbcode gelöst werden, um Routine zu bekommen.

<indepth>
*Vertiefung:* Es gibt auch Widerstände mit mehr als nur vier Farbringen. Diese sind aber für die Prüfung nicht relevant. Auch andere Bauteile werden oftmals mit Farbringen gekennzeichnet.
</indepth>

[question:NC107]
[question:NC105]
[question:NC106]
[question:NC104]
[question:NC103]
[question:NC102]
[question:NC108]
[question:NC109]
[question:NC110]
