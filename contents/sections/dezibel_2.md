%%%%%%%%%%%%%%%%% Aus der Klasse E kopiert. TODO einarbeiten

---

Wenn wir nun den zu einem Dezibel-Wert gehörenden Verhältniswert finden wollen, rechnen wir:

$b = 10^{\frac{a/\unit{\dB}}{10}}$

Nun zurück zu unserem Verstärkungsfaktor des Kurzwellenempfängers. Der dekadische Logarithmus einer Eins mit 12 Nullen ist einfach die Anzahl der Nullen, also 12, multipliziert mit 10, ergibt den Verstärkungsfaktor von $\qty{120}{\dB}$.


In der Frage wird noch der Begriff _Leistungspegel_ verwendet. Das ist das logarithmisch ausgedrückte Verhältnis einer Leistung zu einer Referenzleistung.

So ist die Leistung *b* bezogen auf $\qty{1}{\watt}$:

$a = \qty{\left(10\cdot\lg{\frac{b}{\qty{1}{\watt}}}\right)}{\dBW}$

bzw. bezogen auf ein Milliwatt:

$a =  \qty{\left(10\cdot\lg{\frac{b}{\qty{1}{\milli\watt}}}\right)}{\dBm}$

Nun zur Lösung der Frage. Die Leistung wird verdoppelt - um wieviel $\unit{\dB}$ ändert sich der Leistungspegel? Hier ist also das Leistungsverhältnis $b=2$.

$10 \cdot \lg{2} = \qty{3,01}{\dB} \approx \qty{3}{\dB}$

Negative Dezibelwerte kennzeichnen übrigens Verhältniswerte kleiner als 1. So entspricht $\qty{-3}{\dB}$ einem Verhältniswert von $\num{0,5}$ ($\frac{1}{2}$).

%%%%%%%%%%%%%%%%%

% Dezibel II, DF2DR, 2024-08-17

Den Begriff der Logarithmus und das Dezibel ($\unit{\dB}$) als Form der logarithmischen Angabe von Leistungsverhältnissen hatten wir bereits eingeführt.

%TODO: Wie kann der Erklärungstext aus "Dezibel I" hier verlinkt werden?

Kurz zur Wiederholung: das Verhältnis *a* zweier Leistungen $P_1$ und $P_2$ in $\unit{\dB}$ ist:

$a = 10 \cdot\log\left(\frac{P_1}{P_2}\right)\unit{\dB}$

Aus dem Dezibel abgeleitet hatten wir die *Leistungspegel* als logarithmische Maße:

- Leistung bezogen auf $\qty{1}{\watt}$: $\unit{\dBW}$
- Leistung bezogen auf $\qty{1}{\milli\watt}$: $\unit{\dBm}$

Das Dezibel können wir auch verwenden, um *Spannungsverhältnisse* und *Spannungspegel* anzugeben. Dazu berücksichtigen wir, dass die Leistung proportional zum Quadrat der Spannung ist. Also können wir schreiben:

$a = 10 \cdot \log\left(\frac{P_1}{P_2}\right) = 10 \cdot \log\left(\frac{U_1^2}{U_2^2}\right)$

Der Logarithmus einer quadrierten Zahl ist aber gleich zweimal dem Logarithmus der Zahl:

$\lg(x^2)=2 \cdot \lg(x)$

Also:

$10 \cdot \log\left(\frac{U_1^2}{U_2^2}\right)=20 \cdot \lg\left(\frac{U_1}{U_2}\right)$

Daher berechnen wir ein Verhältnis *a* zweier Spannungen $U_1$ und $U_2$, indem wir den Logarithmus des Verhältnisses nicht mit dem Faktor 10, sondern mit dem Faktor 20 multiplizieren:

$a = 20 \cdot \log \left(\frac{U_1}{U_2}\right)\unit{\dB}$

<tip>
Bei der Dezibel-Berechnung immer genau beachten, ob es sich um Leistungs- oder Spannungsverhältnisse handelt!
</tip>

Zur Bestimmung von Spannungspegeln müssen wir wieder erst eine Bezugsspannung festlegen. Bei Empfangssignalen messen wir die (sehr kleinen) Spannungen am Empfängereingang gern in $\unit{\micro\volt}$. Der zugehörige Spannungspegel hat dann die Einheit $\unit{\dBuV}$. Beispiel:

$\qty{10}{\micro\volt} \rightarrow 20 \cdot \log\left(\frac{\qty{10}{\micro\volt}}{\qty{1}{\micro\volt}}\right)=\qty{20}{\dBuV}$

<tip>
*Rechnen mit Logarithmen:*
Einige einfache Rechenregeln ermöglichen die Lösung von Dezibel-Aufgaben ohne Taschenrechner.

* Der Logarithmus eines Produkts zweier Zahlen entspricht der Summe der Logarithmen: $\log(a\cdot b) = \log(a)+ \log(b)$
* Der Logarithmus einer Division zweier Zahlen entspricht der Differenz der Logarithmen: $\log(a / b) = \log(a) - \lg(b)$
* Daraus abgeleitet: um den Logarithmus einer quadrierten Zahl zu bestimmen, multiplizieren wir den Logarithmus der Zahl mit dem Faktor 2. Um den Logarithus der Quadratwurzel einer Zahl zu bestimmen, multiplizieren wir den Logarithmus der Zahl mit dem Faktor $\frac{1}{2}$. 
</tip>

<tip>
*Nützlich zu merken:*

* $\qty{0}{\dB}$ entspricht dem Faktor $1$.
* $\qty{3}{\dB}$ entsprechen einem Leistungsverhältnis von $2$
* $\qty{-3}{\dB}$ einem Leistungsverhältnis von $\frac{1}{2}$.
* $\qty{6}{\dB}$ entsprechen einem Leistungsverhältnis von $4$ und einem Spannungsverhälnis von $2$.
* $\qty{-6}{\dB}$ sind ein Leistungsverhältnis von $\frac{1}{4}$ und ein Spannungsverhältnis von $\frac{1}{2}$.
* $\qty{10}{\dB}$ entsprechen einem Leistungsverhältnis von $10$.
* $\qty{20}{\dB}$ entsprechen einem Leistungsverhältnis von $100$ und einem Spannungsverhältnis von $10$.
  
Mit diesen wenigen Werten lassen sich Lösungen in der Regel zumindest hinreichend genau abschätzen.
  
*Beispiele:*

* Welcher Faktor entspricht einem Leistungsverhältnis von $\qty{17}{\dB}$? $\qty{17}{\dB} = \qty{20}{\dB} - \qty{3}{\dB}$, also Faktor $100$ durch $2$ gleich $50$.
* Wieviel $\unit{\dB}$ entspricht ein Spannungsverhältnis von 4? $4 = 2 \cdot 2 \rightarrow \qty{6}{\dB} + \qty{6}{\dB} = \qty{12}{\dB}$
</tip>

[question:AA105]
[question:AA106]
[question:AA107]
[question:AA108]
[question:AA109]
[question:AA110]
[question:AA111]
[question:AA112]