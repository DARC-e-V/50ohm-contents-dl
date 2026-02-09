An vielen Stellen der Hochfrequenztechnik spielen Leistungsverhältnisse eine wichtige Rolle, etwa beim Gewinn einer Antenne oder eines Verstärkers, oder bei der Dämpfung eines Kabels. In der Klasse N haben wir diese Zusammenhänge noch in Form einfacher Faktoren kennengelernt, zum Beispiel: „Die Antenne hat einen Gewinn von Faktor 2“.

Diese Verhältnisse können sehr große oder sehr kleine Zahlenwerte annehmen. So besitzt beispielsweise ein Kurzwellenempfänger einen Gesamtverstärkungsfaktor von 1 000 000 000 000, also eine Eins mit zwölf Nullen. Mit solchen Zahlen wird das Rechnen schnell unübersichtlich, und man beginnt unweigerlich, die Nullen zu zählen.

Vereinfacht gesagt gibt es jedoch ein mathematisches Hilfsmittel für dieses „Zählen von Nullen“: die Logarithmen. Mit ihrer Hilfe lassen sich außerdem Multiplikationen in Additionen und Divisionen in Subtraktionen umwandeln. Das macht das Rechnen mit Großen Zahlen sehr einfach. 

---

Es hat sich daher eingebürgert, Leistungsverhältnisse auf einer logarithmischen Skala anzugeben.
Das Logarithmieren ist die Umkehroperation des Potenzierens. Im Amateurfunk nutzen wir in der Regel den dekadischen Logarithmus ("Zehnerlogarithmen") zur Basis 10:

---

$a =\log_{10} (b)$, falls $b=10^{a}$

Der Logarithmus von 100 beträgt $\log_{10}(100)=2$, da $10^2 = 100$ ist. Anders ausgedrückt: Die Zahl 100 besitzt zwei Nullen.

<warning>
Ein technisch-wissenschaftlicher Taschenrechner bietet neben dem dekadischen Logarithmus (Beschriftung lg oder log) auch den natürlichen Logarithmus *ln* an, der als Basis die Eulersche Zahl *e=2,7182818…* hat. Nicht verwechseln!
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

$10 \cdot \lg(b) = \qty{a}{\dB}$

---

Die Formelsammlung gibt für das Umrechnen eines Leistungsverhältnisses folgende Formel an:

$g = 10\cdot \log_{10}\left(\frac{P_2}{P_1}\right)\unit{\dB}$

Wobei $P_1$ der Eingangsleistung entspricht und $P_2$ der Ausgangsleistung. Nehmen wir nun an, wir haben einen Verstärker der die Eingangsleistung $P_1=\qty{50}{\watt}$ auf $P_2=\qty{100}{\watt}$ verstärkt, also verdoppelt. So ergibt sich nach unserer Formel folgender Verstärkungsfaktor in $\unit{\dB}$:

$g = 10\cdot \log_{10}\left(\frac{\qty{100}{\watt}}{\qty{50}{\watt}}\right)\unit{\dB} = 10\cdot \log_{10}\left(2\right)\unit{\dB} = 10\cdot 0.301 \unit{\dB} \approx 3 \unit{\dB} $

Für die Klasse E ist es zunächst ausreichend, den Dezibelwert für den Leistungsfaktor 2 zu kennen. Die Formelsammlung enthält dazu eine Tabelle, die auch in Tabelle [ref:e_dezibel_leistungsfaktoren] dargestellt ist. Daraus lässt sich ablesen, dass ein Leistungsfaktor von 2 einem Dezibelwert von $\qty{3}{\dB}$ entspricht. Das ausführliche Rechnen mit Dezibelwerten wird erst in der Klasse A behandelt.

%TODO: ^--- Prüfen ob Formeln in der Klasse E gebraucht werden! (DL9MJ)

<tip>
Ganz ohne Taschenrechner lassen sich Dezibelwerte  abschätzen, die auf "0" enden .. einfach die letzte Null zuhalten, die Ziffer gibt dann die Anzahl der Nullen des Verhältnisfaktors an. Beispiel: $\qty{30}{\dB} \rightarrow 3 \rightarrow \text{3 Nullen} \rightarrow \text{Verhältnisfaktor 1000}$!
</tip>

[question:EA107]

Neben der Einheit $\unit{dB}$ begegnet man in der Praxis häufig auch Angaben wie $\unit{\dBi}$, $\unit{\dBm}$, $\unit{\dBW}$ oder $\unit{\dBu}$. Diese Zusätze geben an, auf welche Bezugsgröße sich der jeweilige Dezibelwert bezieht.

Das Bel ($\unit{\bel}$) beziehungsweise das Dezibel ($\unit{\dB}$) beschreibt grundsätzlich ein dimensionsloses Verhältnis, etwa von Leistungen oder Spannungen. Deshalb wird $\unit{\dB}$ vor allem zur Angabe von Verstärkungen und Dämpfungen verwendet. In diesen Fällen ist kein weiterer Zusatz notwendig, da lediglich das Verhältnis zweier Größen angegeben wird.

Sollen Dezibelwerte jedoch als absolute Pegel angegeben werden, ist eine feste Bezugsgröße erforderlich. Diese Bezugsgröße kann zum Beispiel eine Leistung von $\qty{1}{\milli\watt}$, eine Leistung von $\qty{1}{\watt}$ oder eine Spannung von $\qty{0,775}{\volt}$ sein. Entsprechend wird der Dezibelwert mit einem Zusatz versehen: Bezieht sich der Pegel beispielsweise auf $\qty{1}{\milli\watt}$, spricht man von $\unit{\dBm}$. Auf diese Weise wird eindeutig festgelegt, welcher absolute Wert dem Dezibelpegel zugrunde liegt.

Findet man eine Angabe wie „Der Sender hat eine Ausgangsleistung von $\qty{20}{\dBm}$“, lässt sich dieser Wert leicht in Milliwatt umrechnen. Ein Pegel von $\qty{20}{\dB}$ entspricht einem Leistungsfaktor von 100 (also zwei Nullen). Dieser Faktor wird mit der Bezugsgröße von $\qty{1}{\milli\watt}$ multipliziert:

$ P = 100 \cdot \qty{1}{\milli\watt} = \qty{100}{\milli\watt}$

Weitere Beispiele sind, $\qty{0}{\dBm} \equiv \qty{1}{\milli\watt}$, oder $\qty{50}{\dBm} \equiv \qty{100}{\watt}$

%TODO: ggf die Umrechnung in die andere Richtung hinzufügen falls das in der Klasse E gebraucht wird. (DL9MJ)

---

Warum macht man das Ganze? Wie bereits angedeutet, dient die Verwendung von Dezibel vor allem dazu, Rechnungen zu vereinfachen. Durch die Darstellung von Verstärkungen und Dämpfungen in Dezibel lassen sich komplette Signalketten sehr einfach durch Addition und Subtraktion überschlagen, ohne auf umständliche Multiplikationen und Divisionen zurückgreifen zu müssen.

Abbildung [ref:e_signalkette] zeigt eine solche Signalkette mit drei Verstärkerstufen. Das Eingangssignal besitzt eine Leistung von $\qty{1}{\milli\watt}$, was $\qty{0}{\dBm}$ entspricht. Durch die drei Verstärkerstufen wird das Signal insgesamt auf $\qty{60}{\dBm}$ verstärkt (also $1000000\cdot \qty{1}{\milli\watt}$), was einer Leistung von $\qty{1000}{\watt}$ entspricht.

Abbildung [ref:e_signalkette_2] zeigt ein weiteres Beispiel einer Signalkette, bei der zusätzlich ein Dämpfungsglied mit einer Dämpfung von $\qty{20}{\dB}$ eingesetzt wird, was einer negativen Verstärkung von $\qty{-20}{\dB}$ entspricht. Das Eingangssignal besitzt eine Leistung von $\qty{1}{\milli\watt}$, also $\qty{0}{\dBm}$. Durch die erste Verstärkerstufe wird das Signal auf $\qty{10}{\dBm}$ angehoben. Anschließend wird es durch das Dämpfungsglied auf $\qty{-10}{\dBm}$ abgeschwächt und schließlich durch die zweite Verstärkerstufe wieder auf $\qty{0}{\dBm}$ verstärkt.

<margin>
[picture:877:e_signalkette:Signalkette mit drei Verstärken]
[picture:1053:e_signalkette_2:Signalkette mit zwei Verstärken und einem Dämpfungsglied]
</margin>

<indepth>
Wieso ist es zulässig vom Pegel $\qty{9}{\dBm}$ eine Dämpfung von $\qty{3}{\dB}$ abzuziehen? Beide Werte haben doch unterschiedliche Maßeinheiten!
Bei der Einheit Bel ($\unit{\bel}$) bzw. Dezibel ($\unit{\dB}$) handelt es sich um eine Hilfsmaßeinheit (auch Pseudoeinheit).
Im Prinzip könnte der Zahlenwert auch ohne  die Einheit $\unit{\dB}$ geschrieben werden, aber mit dem Zusatz $\unit{\dB}$ wird deutlich, dass es um ein logarithmisches Verhältnis von zwei Größen geht. Ohne diese Einheit müsste man verbal beschreiben welche Bedeutung der Zahlenwert hat.
</indepth>
  
Zusätzlich gibt es die Zusätze $\unit{\dBd}$ und $\unit{\dBi}$, die bei der Angabe von Antennengewinnen verwendet werden. In diesem Fall bezieht sich der Dezibelwert nicht auf eine Leistung oder Spannung, sondern auf einen bestimmten Referenzstrahler. Üblich sind dabei $\unit{\dBi}$, bezogen auf den isotropen Kugelstrahler, sowie $\unit{\dBd}$, bezogen auf den Halbwellendipol. Dieses Wissen werden wir benötigen, wenn wir uns später mit Antennen beschäftigen.
