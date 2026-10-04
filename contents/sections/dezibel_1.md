An vielen Stellen der Hochfrequenztechnik spielen Leistungsverhältnisse eine wichtige Rolle, etwa beim Gewinn einer Antenne oder eines Verstärkers, oder bei der Dämpfung eines Kabels. In der Klasse N haben wir diese Zusammenhänge noch in Form einfacher Faktoren kennengelernt, zum Beispiel: „Die Antenne hat einen Gewinn von Faktor $2$“.

Diese Verhältnisse können sehr große oder sehr kleine Zahlenwerte annehmen. So besitzt beispielsweise ein Kurzwellenempfänger einen Gesamtverstärkungsfaktor von $\num{1000000000000}$, also eine Eins mit zwölf Nullen. Mit solchen Zahlen wird das Rechnen schnell unübersichtlich, und man beginnt unweigerlich, die Nullen zu zählen.

Vereinfacht gesagt gibt es jedoch ein mathematisches Hilfsmittel für dieses „Zählen von Nullen“: die Logarithmen. Mit ihrer Hilfe lassen sich außerdem Multiplikationen in Additionen und Divisionen in Subtraktionen umwandeln. Das macht das Rechnen mit großen Zahlen sehr einfach. 

---

Es hat sich daher eingebürgert, Leistungsverhältnisse auf einer logarithmischen Skala anzugeben.
Das Logarithmieren ist die Umkehroperation des Potenzierens. Im Amateurfunk nutzen wir in der Regel den dekadischen Logarithmus ("Zehnerlogarithmen") zur Basis $10$:

---

$a =\log_{10} (b)$, falls $b=10^{a}$

Der Logarithmus von $100$ beträgt $\log_{10}(100)=2$, da $10^2 = 100$ ist. Anders ausgedrückt: Die Zahl $100$ besitzt zwei Nullen.

<warning>
Ein technisch-wissenschaftlicher Taschenrechner bietet neben dem dekadischen Logarithmus (Beschriftung $\lg$ oder $\log$) auch den natürlichen Logarithmus *$\ln$* an, der als Basis die Eulersche Zahl *$e=\num{2,7182818}\dots$* hat. Nicht verwechseln!
</warning>	

<margin>
| c:dB | c:≈ Leistungsfaktor |
| $0$ | $1$ |
| $1,5$ | $\sqrt{2} = 1,41$ |
| $2,15$ | $1,64$ |
| $3$ | $2$ |
| $5$ | $\sqrt{10} = 3,16$ |
| $6$ | $4$ |
| $10$ | $10$ |
| $20$ | $100$ |
[table:e_dezibel_leistungsfaktoren:Wichtige Leistungsfaktoren in $\unit{\dB}$]
</margin>

Vom dekadischen Logarithmus ist das *Bel* ($\unit{\bel}$) abgeleitet. Der Name ehrt den amerikanischen Gehörlosenlehrer und Telefonpionier, *Alexander Graham Bell*. Im obigen Beispiel hätten wir auch schreiben können:

$\log_{10}(b)=\qty{a}{\bel}$

In der Regel wird statt des Bels das *Dezibel* (Einheitenzeichen $\unit{\dB}$) verwendet, also der zehnte Teil eines Bels:

$10 \cdot \log_{10}(b) = \qty{a}{\dB}$

---

Die Formelsammlung gibt für das Umrechnen eines Leistungsverhältnisses folgende Formel an:

$g = 10\cdot \log_{10}\left(\frac{P_2}{P_1}\right)\unit{\dB}$

Wobei $P_1$ der Eingangsleistung entspricht und $P_2$ der Ausgangsleistung. Nehmen wir nun an, wir haben einen Verstärker der die Eingangsleistung $P_1=\qty{50}{\watt}$ auf $P_2=\qty{100}{\watt}$ verstärkt, also verdoppelt. So ergibt sich nach unserer Formel folgender Verstärkungsfaktor in $\unit{\dB}$:

$g = 10\cdot \log_{10}\left(\frac{\qty{100}{\watt}}{\qty{50}{\watt}}\right)\unit{\dB} = 10\cdot \log_{10}\left(2\right)\unit{\dB} = 10\cdot \qty{0,301}{\dB} \approx \qty{3}{\dB} $

Für die Klasse E ist es zunächst ausreichend, den Dezibelwert für den Leistungsfaktor $2$ zu kennen. Die Formelsammlung enthält dazu eine Tabelle, die auch in Tabelle [ref:e_dezibel_leistungsfaktoren] dargestellt ist. Daraus lässt sich ablesen, dass ein Leistungsfaktor von $2$ einem Dezibelwert von $\qty{3}{\dB}$ entspricht. Das ausführliche Rechnen mit Dezibelwerten wird erst in der Klasse A behandelt.

<tip>
Ganz ohne Taschenrechner lassen sich Dezibelwerte abschätzen, die auf "$0$" enden: Einfach die letzte Null zuhalten, die Ziffer gibt dann die Anzahl der Nullen des Verhältnisfaktors an. Beispiel: $\qty{30}{\dB} \rightarrow 3 \rightarrow 3~\text{Nullen} \rightarrow \text{Verhältnisfaktor}~1000$!
</tip>

[question:EA107]

Neben der Einheit $\unit{dB}$ begegnet man in der Praxis häufig auch Angaben wie $\unit{\dBi}$, $\unit{\dBm}$, $\unit{\dBW}$ oder $\unit{\dBu}$. Diese Zusätze geben an, auf welche Bezugsgröße sich der jeweilige Dezibelwert bezieht. In der Klasse E werden uns insbesondere bei Antennen die Angaben $\unit{\dBi}$ und $\unit{\dBd}$ im Antennenkapitel begegnen. Die anderen Größen wie $\unit{\dBm}$ und $\unit{\dBW}$ werden erst für die Klasse A benötigt.