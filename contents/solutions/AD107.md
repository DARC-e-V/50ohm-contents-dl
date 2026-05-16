Gegeben sind:

$ U = \qty{15}{\volt} $

und

$ R_1 = R_2 = R_3 = \qty{10}{\kilo\ohm} $

Zuerst wird der Ersatzwiderstand der Parallelschaltung aus $R_2$ und $R_3$ berechnet:

$ R_{23} = \frac{R_2 \cdot R_3}{R_2 + R_3} $

Da beide Widerstände gleich groß sind, ergibt sich:

$ R_{23} = \qty{5}{\kilo\ohm} $

Der Gesamtwiderstand der Schaltung beträgt damit:

$ R_\mathrm{ges} = R_1 + R_{23} = \qty{10}{\kilo\ohm} + \qty{5}{\kilo\ohm} = \qty{15}{\kilo\ohm} $

Nun kann der Gesamtstrom berechnet werden:

$ I_\mathrm{ges} = \frac{U}{R_\mathrm{ges}} = \frac{\qty{15}{\volt}}{\qty{15}{\kilo\ohm}} = \qty{1}{\milli\ampere} $

Dieser Strom fließt zunächst durch $R_1$ und teilt sich danach auf die beiden gleich großen Widerstände $R_2$ und $R_3$ auf.

Da beide Widerstände gleich groß sind, fließt durch jeden Zweig genau die Hälfte des Gesamtstroms:

$ I_3 = \frac{I_\mathrm{ges}}{2} = \frac{\qty{1}{\milli\ampere}}{2} = \qty{0,5}{\milli\ampere} $