Die Z-Diode stabilisiert die Spannung am linken Anschluss von $R_2$ auf

$U_Z=\qty{6,2}{\volt}$

Befindet sich der Schleifer von $R_3$ am Anschlag 1, ist der Schleifer direkt mit dem oberen Anschluss von $R_3$ verbunden. Von diesem Punkt nach Masse liegen zwei Zweige parallel:

$R_4=\qty{6,8}{\kilo\ohm}$

und

$R_3+R_6=\qty{220}{\ohm}+\qty{150}{\ohm}=\qty{370}{\ohm}$

Der Ersatzwiderstand nach Masse beträgt damit:

$R_\mathrm{u}=R_4\parallel(R_3+R_6)$

$R_\mathrm{u}=\frac{\qty{6800}{\ohm}\cdot\qty{370}{\ohm}}{\qty{6800}{\ohm}+\qty{370}{\ohm}}\approx\qty{351}{\ohm}$

Nun ist auch $R_2=\qty{270}{\ohm}$ zu berücksichtigen. $R_2$ und $R_\mathrm{u}$ bilden an der stabilisierten Spannung von $\qty{6,2}{\volt}$ einen Spannungsteiler:

$U_\mathrm{G}=\qty{6,2}{\volt}\cdot\frac{\qty{351}{\ohm}}{\qty{270}{\ohm}+\qty{351}{\ohm}}\approx\qty{3,5}{\volt}$

Da die Source-Anschlüsse der Transistoren auf Masse liegen, entspricht die Gate-Spannung gleichzeitig der Gate-Source-Spannung:

$U_\mathrm{GS}\approx\qty{3,5}{\volt}$

Die Gate-Source-Spannung beträgt somit ungefähr $\qty{3,5}{\volt}$.

Übrigens: 

Der Widerstand $R_5=\qty{51}{\ohm}$ beeinflusst die Gleichspannung am Gate praktisch nicht, da in das Gate des LDMOS-Transistors nahezu kein Gleichstrom fließt. Für das HF-Signal ist $R_5$ jedoch wichtig: Er bedämpft zusammen mit der Gate-Kapazität mögliche hochfrequente Schwingungen und verbessert damit die Stabilität des Verstärkers.

Der Widerstand $R_4=\qty{6,8}{\kilo\ohm}$ sorgt dafür, dass das Gate auch bei einer Unterbrechung der Arbeitspunkteinstellung ein definiertes Potential gegen Masse besitzt. Er entlädt außerdem die Gate-Kapazität und verhindert damit, dass der Transistor durch ein frei schwebendes Gate unbeabsichtigt leitend wird. Da $R_4$ parallel zum unteren Zweig des Spannungsteilers liegt, muss er bei der genauen Berechnung der Gate-Spannung berücksichtigt werden.