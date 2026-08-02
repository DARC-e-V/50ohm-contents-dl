In der Klasse E haben wir bereits das Dezibel als Werkzeug zum Beschreiben von Verhältnissen kennengelernt und gesehen, dass eine Leistungsänderung von $\qty{3}{\dB}$ einem Leistungsfaktor von $\num{2}$ entspricht. In der Formelsammlung finden wir die Tabelle [ref:a_dezibel_leistungsfaktoren], welche weitere wichtige Entsprechungen beinhaltet. 

<margin>
| c:dB | c:≈ Leistungsfaktor |
| $-20$ | $\num{0,01}$ |
| $-10$ | $\num{0,1}$ |
| $-6$ | $\num{0,25}$ |
| $-3$ | $\num{0,5}$ |
| $-1$ | $\num{0,79}$ |
| $0$ | $\num{1}$ |
| $1,5$ | $\sqrt{2} = \num{1,41}$ |
| $2,15$ | $\num{1,64}$ |
| $3$ | $\num{2}$ |
| $5$ | $\sqrt{10} = \num{3,16}$ |
| $6$ | $\num{4}$ |
| $10$ | $\num{10}$ |
| $20$ | $\num{100}$ |
[table:a_dezibel_leistungsfaktoren:Wichtige Leistungsfaktoren in $\unit{\dB}$]
</margin>

Die Formelsammlung gibt für das Umrechnen eines Leistungsverhältnisses in $\unit{\dB}$ folgende Formel an, welche wir auch schonmal in der Klasse E kennen gelernt haben. Das Verhältnis $g$ zweier Leistungen $P_1$ und $P_2$ in $\unit{\dB}$ ist:

$g = 10\cdot \log_{10}\left(\frac{P_2}{P_1}\right)\unit{\dB}$

[question:AD428]

Möchte man aus einem $\unit{\dB}$-Wert einen Verhältnisfaktor ermitteln, so muss die Formel umgestellt werden: 

$\begin{align*} g &= 10 \cdot \log_{10}\left( x \right) \unit{\dB} & \quad\quad\quad &|: \qty{10}{\dB} \\ \frac{g}{\qty{10}{\dB}} &= \log_{10}\left( x \right) &~&| \quad 10^{x}\\ x &= 10^{\frac{g}{\qty{10}{\dB}}} &~&~\end{align*}$

Mit diesen beiden Formeln können wir also leicht zwischen $\unit{\dB}$-Angaben und Verhältnisfaktoren umrechnen. Versuche nun die drei folgenden Fragen zu berechnen: 

---

[question:AA105]
[question:AA106]
[question:AD426]

<tip>
In der Klasse E haben wir bereits folgenden Trick kennengelernt: Ganz ohne Taschenrechner lassen sich Dezibelwerte abschätzen, die auf "$0$" enden: Einfach die letzte Null zuhalten, die Ziffer gibt dann die Anzahl der Nullen des Verhältnisfaktors an. Beispiel: $\qty{30}{\dB} \rightarrow 3 \rightarrow 3~\text{Nullen} \rightarrow \text{Verhältnisfaktor}~1000$!

Auch anders herum lässt es sich leicht berechnen: Eins mit $12$ Nullen ($\num{1000000000000}$) in $\unit{\dB}$ ist einfach die Anzahl der Nullen, also $12$, multipliziert mit $10$. Es ergibt sich so ein Verstärkungsfaktor von $\qty{120}{\dB}$.

Aber auch für $\unit{\dB}$-Werte die nicht auf $0$ enden kann man durch Zerlegung den entsprechenden Faktor ermitteln:

* Man kann $\qty{9}{\dB}$ in $\qty{6}{\dB} + \qty{3}{\dB}$ zerlegen, was einer Multiplikation von $4\cdot 2 = 8$ entspricht. 
* Welcher Faktor entspricht einem Leistungsverhältnis von $\qty{17}{\dB}$? $\qty{17}{\dB} = \qty{20}{\dB} - \qty{3}{\dB}$, also Faktor $100$ durch $2$ gleich $50$.
</tip>

Das Dezibel ($\unit{\dB}$) beschreibt grundsätzlich ein dimensionsloses Verhältnis, etwa von Leistungen oder Spannungen. Deshalb wird $\unit{\dB}$ vor allem zur Angabe von Verstärkungen und Dämpfungen verwendet. In diesen Fällen ist kein weiterer Zusatz notwendig, da lediglich das Verhältnis zweier Größen angegeben wird. Negative Dezibelwerte kennzeichnen übrigens Verhältniswerte kleiner als $1$. So entspricht $\qty{-3}{\dB}$ einem Verhältniswert von $\frac{1}{2} = \num{0,5}$.

Man kann aber auch Dezibelwerte nutzen, um einen absoluten Pegel anzugeben. Dafür ist allerdings eine feste Bezugsgröße $P_0$ erforderlich:

$p = 10\cdot \log_{10}\left(\frac{P}{P_0}\right)\unit{\dB}$

---

Diese Bezugsgröße kann zum Beispiel eine Leistung von $\qty{1}{\milli\watt}$ sein. In diesem Fall erhält der Dezibelwert einen entsprechenden Zusatz: Bezieht sich der Pegel auf $\qty{1}{\milli\watt}$, spricht man von $\unit{\dBm}$. Dadurch ist eindeutig festgelegt, auf welchen absoluten Leistungswert sich der Dezibelpegel bezieht.

Trifft man beispielsweise auf die Angabe „Der Sender hat eine Ausgangsleistung von $\qty{20}{\dBm}$“, lässt sich dieser Wert leicht in Milliwatt umrechnen. Ein Pegel von $\qty{20}{\dB}$ entspricht einem Leistungsfaktor von $100$ (also zwei Nullen). Dieser Faktor wird mit der Bezugsgröße von $\qty{1}{\milli\watt}$ multipliziert:

$ P = 100 \cdot \qty{1}{\milli\watt} = \qty{100}{\milli\watt}$

In der Tabelle [ref:a_bezugsgroessen] sind die wichtigsten Bezugsgrößen und ihre jeweiligen $\unit{\dB}$-Abkürzungen aufgelistet.

<margin>
| l: Abkürzung            | X: Bezugswert          |
| $\unit{\dBm}$           | $\qty{1}{\milli\watt}$ | 
| $\unit{\dBW}$           | $\qty{1}{\watt}$       | 
| $\unit{\dBu}$           | $\qty{0,775}{\volt}$   | 
| $\unit{\dB\micro\volt}$ | $\qty{1}{\micro\volt}$ | 
[table:a_bezugsgroessen:Wichtige Bezugsgrößen aus der Formelsammlung]
</margin>

Die folgenden Fragen lassen sich mit Hilfe der Formel aus der Formelsammlung und deren Umstellung vom Anfang dieser Lektion berechnen, wenn die richtige Bezugsgröße verwendet wird. 

[question:AA109]
[question:AA110]
[question:AA107]
[question:AA108]

---

Warum macht man das Ganze überhaupt und gibt absolute Leistungen in $\unit{\dBm}$ und $\unit{\dBW}$ an? Wie bereits in der Klasse E angedeutet, dient die Verwendung von Dezibel vor allem dazu, Rechnungen zu vereinfachen. Durch die Darstellung von Verstärkungen und Dämpfungen in Dezibel lassen sich komplette Signalketten sehr einfach durch Addition und Subtraktion überschlagen, ohne auf umständliche Multiplikationen und Divisionen zurückgreifen zu müssen.

Abbildung [ref:e_signalkette] zeigt eine solche Signalkette mit drei Verstärkerstufen. Das Eingangssignal besitzt eine Leistung von $\qty{1}{\milli\watt}$, was $\qty{0}{\dBm}$ entspricht. Durch die drei Verstärkerstufen wird das Signal insgesamt auf $\qty{60}{\dBm}$ verstärkt (also $\num{1000000}\cdot \qty{1}{\milli\watt}$), was einer Leistung von $\qty{1000}{\watt}$ entspricht.

Abbildung [ref:e_signalkette_2] zeigt ein weiteres Beispiel einer Signalkette, bei der zusätzlich ein Dämpfungsglied mit einer Dämpfung von $\qty{20}{\dB}$ eingesetzt wird, was einer Verstärkung von $\qty{-20}{\dB}$ entspricht. Das Eingangssignal besitzt eine Leistung von $\qty{1}{\milli\watt}$, also $\qty{0}{\dBm}$. Durch die erste Verstärkerstufe wird das Signal auf $\qty{10}{\dBm}$ angehoben. Anschließend wird es durch das Dämpfungsglied auf $\qty{-10}{\dBm}$ abgeschwächt und schließlich durch die zweite Verstärkerstufe wieder auf $\qty{0}{\dBm}$ verstärkt, was wiederum $\qty{1}{\milli\watt}$ entspricht.

<margin>
[picture:877:e_signalkette:Signalkette mit drei Verstärken]
[picture:1053:e_signalkette_2:Signalkette mit zwei Verstärken und einem Dämpfungsglied]
</margin>

<indepth>
Wieso ist es zulässig vom Pegel $\qty{9}{\dBm}$ eine Dämpfung von $\qty{3}{\dB}$ abzuziehen? Beide Werte haben doch unterschiedliche Maßeinheiten! Bei der Einheit Bel ($\unit{\bel}$) bzw. Dezibel ($\unit{\dB}$) handelt es sich um eine Hilfsmaßeinheit (auch Pseudoeinheit).
Im Prinzip könnte der Zahlenwert auch ohne die Einheit $\unit{\dB}$ geschrieben werden. Aber mit dem Zusatz $\unit{\dB}$ wird deutlich, dass es um ein logarithmisches Verhältnis von zwei Größen geht. Ohne diese Einheit müsste man verbal beschreiben welche Bedeutung der Zahlenwert hat.
</indepth>
  
Zusätzlich haben wir in der Klasse E bereits die Zusätze $\unit{\dBd}$ und $\unit{\dBi}$ kennen gelernt, die bei der Angabe von Antennengewinnen verwendet werden. In diesem Fall bezieht sich der Dezibelwert nicht auf eine Leistung oder Spannung, sondern auf einen bestimmten Referenzstrahler. Üblich sind dabei $\unit{\dBi}$, bezogen auf den isotropen Kugelstrahler, sowie $\unit{\dBd}$, bezogen auf den Halbwellendipol.

---

Neben den Leistungsverhältnissen können wir das Dezibel können auch verwenden, um *Spannungsverhältnisse* und *Spannungspegel* anzugeben. Dazu können wir die Formel $P = \frac{U^2}{R}$ verwenden. Also können wir schreiben:

$\begin{split}g &= 10 \cdot \log_{10}\left(\frac{P_1}{P_2}\right)\\ g &= 10 \cdot \log_{10}\left(\frac{\frac{U_1^2}{\cancel{R}}}{\frac{U_2^2}{\cancel{R}}}\right)\\ g &= 10 \cdot \log_{10}\left(\left(\frac{U_1}{U_2}\right)^2\right) \end{split}$

<tip>
*Rechnen mit Logarithmen:*
Einige einfache Rechenregeln ermöglichen die Lösung von Dezibel-Aufgaben ohne Taschenrechner.

* Der Logarithmus eines Produkts zweier Zahlen entspricht der Summe der Logarithmen: $\log_{10}(a\cdot b) = \log_{10}(a)+ \log_{10}(b)$
* Der Logarithmus einer Division zweier Zahlen entspricht der Differenz der Logarithmen: $\log_{10}(a / b) = \log_{10}(a) - \log_{10}(b)$
* Der Logarithmus einer quadrierten Zahl: $\log_{10}(x^2)= 2 \cdot \log_{10}(x)$
* Der Logarithmus einer Wurzel: $\log_{10}(\sqrt{x})= \frac{1}{2} \cdot \log_{10}(x)$
</tip>

Der Logarithmus einer quadrierten Zahl ist aber gleich zweimal dem Logarithmus der Zahl:

$\log_{10}(x^2)=2 \cdot \log_{10}(x)$

Es folgt daraus:

$\begin{split} g &= 10 \cdot \log_{10}\left(\left(\frac{U_1}{U_2}\right)^2\right)\\ g &= 10 \cdot 2 \cdot \log_{10}\left(\frac{U_1}{U_2}\right) \\ g &= 20 \cdot \log_{10}\left(\frac{U_1}{U_2}\right) \end{split}$

---

Daher berechnen wir ein Verhältnis *$a$* zweier Spannungen $U_1$ und $U_2$, indem wir den Logarithmus des Verhältnisses nicht mit dem Faktor $10$, sondern mit dem Faktor $20$ multiplizieren. Diese Formel finden wir auch in der Formelsammlung.

[question:AA111]
[question:AD427]

<attention>
Bei der Dezibel-Berechnung immer genau beachten, ob es sich um Leistungs- oder Spannungsverhältnisse handelt!
</attention>

Zur Bestimmung von Spannungspegeln müssen wir wieder erst eine Bezugsspannung festlegen (vgl. Tabelle [ref:a_bezugsgroessen]). Bei Empfangssignalen messen wir die (sehr kleinen) Spannungen am Empfängereingang gern in $\unit{\micro\volt}$. Der zugehörige Spannungspegel hat dann die Einheit $\unit{\dBuV}$. Beispiel:

$\qty{10}{\micro\volt} \rightarrow 20 \cdot \log_{10}\left(\frac{\qty{10}{\micro\volt}}{\qty{1}{\micro\volt}}\right)=\qty{20}{\dBuV}$

---

Bei der folgenden Frage ist der Bezugswert $\qty{1}{\micro\volt\per\meter}$. Versuche die Aufgabe mit deinem Wissen zu lösen.

<attention>
Achtung, hier ist $\unit{\dB(\micro\volt\per\meter)}$ gemeint und nicht $\unit{(\dB\micro\volt)/\meter}$! 
</attention>

[question:AA112]

<tip>
Auch bei Spannungen kann man vieles mithilfe der Tabelle aus der Formelsammlung im Kopf rechnen:

| c:dB | c:≈ Spannungsverhältnis |
| $-20$ | $\num{0,1}$ |
| $-10$ | $\num{0,32}$ |
| $-6$ | $\num{0,5}$ |
| $-3$ | $\num{0,71}$ |
| $-1$ | $\num{0,89}$ |
| $0$ | $\num{1}$ |
| $1$ | $\num{1,12}$ |
| $3$ | $\num{1,14}$ |
| $6$ | $2$ |
| $10$ | $3,16$ |
| $20$ | $10$ |
[table:a_spannungsverhaeltnisse:Wichtige Spannungsverhältnisse in $\unit{\dB}$]

*Beispiel:*

* Wieviel $\unit{\dB}$ entspricht ein Spannungsverhältnis von $4$? $4 = 2 \cdot 2 \rightarrow \qty{6}{\dB} + \qty{6}{\dB} = \qty{12}{\dB}$
</tip>