In der Klasse E haben wir bereits den *unbelasteten* Spannungsteiler kennengelernt. In der Klasse A beschäftigen wir uns mit dem *belasteten* Spannungsteiler, bei dem die Ausgangsspannung $U_2$ durch einen Lastwiderstand $R_\mathrm{L}$ belastet wird. Das bedeutet, dass der Lastwiderstand parallel zum Widerstand $R_2$ liegt, wie es im Schaltbild der Abbildung [ref:a_spannungsteiler_belastet] zu sehen ist.

<margin>
[picture:199:a_spannungsteiler_belastet:Belasteter Spannungsteiler]
</margin>

Bei einem belasteten Spannungsteiler muss berücksichtigt werden, dass der Gesamtstrom steigt, wenn die Belastung erhöht wird, d.h. der Lastwiderstand $R_\mathrm{L}$ niederohmiger wird. Am besten erklären wir die Auswirkungen der Belastung an einem konkreten Beispiel. Angenommen die Widerstände $R_1$ und $R_2$ haben jeweils einen Wert von $\qty{1}{\kilo\ohm}$ und die Gesamtspannung $U_\mathrm{B}$ beträgt $\qty{12}{\volt}$.

Im unbelasteten Fall beträgt der Widerstand $R_\mathrm{L}=\infty$, der Widerstand exisiert also nicht und es kann kein Strom dadurch fließen. Die Spannung teilt sich gleichmäßig auf die beiden Widerstände $R_1$ und $R_2$ auf, d.h. an jedem Widerstand können $\qty{6}{\volt}$ gemessen werden. Der Gesamtwiderstand beträgt $R_{\mathrm{ges}}=\qty{2}{\kilo\ohm}$. Der Gesamtstrom beträgt $I_1 = \frac{U_\mathrm{B}}{R_{\mathrm{ges}}}=\qty{6}{\milli\ampere}$. Dieser Strom fließt auch durch $R_2$. Die Verlustleistung ist an beiden Widerständen gleich groß: $P_1 = P_2 = \qty{6}{\volt} \cdot \qty{6}{\milli\ampere} = \qty{36}{\milli\watt}$.

Im belasteten Fall soll der Lastwiderstand nun auch $R_\mathrm{L} = \qty{1}{\kilo\ohm}$ betragen. Die Parallelschaltung von $R_2$ und $R_\mathrm{L}$ ergibt einen Ersatzwiderstand von $R_\mathrm{par}=\qty{500}{\ohm}$. Der Gesamtwiderstand des Spannungsteilers beträgt nun nur noch $R_{\mathrm{ges}}=\qty{1,5}{\kilo\ohm}$. Jetzt wirkt ein Spannungsteiler mit $\qty{1}{\kilo\ohm}$ zu $\qty{500}{\ohm}$ und dementsprechend teilt sich die Gesamtspannung auf. $\frac{2}{3}$ der Gesamtspannung ($\qty{8}{\volt}$) kann an $R_1$ und $\frac{1}{3}$ der Gesamtspannung ($\qty{4}{\volt}$) kann an $R_\mathrm{par}$ gemessen werden. 

Der Strom $I_1$ beträgt jetzt $I_1 = \frac{\qty{8}{\volt}}{\qty{1}{\kilo\ohm}}= \frac{\qty{12}{\volt}}{\qty{1,5}{\kilo\ohm}} = \qty{8}{\milli\ampere}$. Dieser Strom steigt also an. 

Die Leistung an $R_1$ beträgt jetzt $P_1 = U_1 \cdot I_1 = \qty{8}{\volt} \cdot \qty{8}{\milli\ampere} = \qty{64}{\milli\watt}$ gegenüber $\qty{36}{\milli\watt}$ im unbelasteten Fall. An $R_\mathrm{par}$ beträgt die Leistung $P_\mathrm{par} = U_\mathrm{par} \cdot I_\mathrm{par} = \qty{4}{\volt} \cdot \qty{8}{\milli\ampere} = \qty{32}{\milli\watt}$ gegenüber $\qty{36}{\milli\watt}$ im unbelasteten Fall. Da sich die ${32}{\milli\watt}$ zwischen $R_2$ und $R_\mathrm{L}$ aufteilen, reduziert sich die Leistung an $R_2$ im belasteten Fall auf $P_2 = \qty{4}{\volt} \cdot \qty{4}{\milli\ampere} = \qty{16}{\milli\watt}$.

Zusammengefasst: Beim Belasten eines Spannungsteiler mit einem Widerstand steigt der Strom $I_1$ an. Dadurch wird $R_1$ wärmer und $R_2$ weniger warm. Mit diesem Wissen können wir die nächste Frage leicht lösen.

[question:AD115]

Bei der folgenden Frage müssen wir unser Wissen über den Spannungsteiler und die Parallelschaltung von Widerständen kombinieren. Dazu zerlegen wir die Aufgabe in einzelne Schritte: Zuerst wird der Ersatzwiderstand der Parallelschaltung aus $R_2$ und $R_\mathrm{L}$ bestimmt. Anschließend kann die Schaltung als einfacher Spannungsteiler betrachtet und daraus die Ausgangsspannung $U_2$ berechnet werden.

[question:AD114]
