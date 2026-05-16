Da alle Widerstände gleich groß sind, gilt:

$ R_1 = R_2 = R_3 = \qty{10}{\kilo\ohm} $

Durch $R_3$ fließt ein Strom von:

$ I_{R_3} = \qty{1}{\milli\ampere} $

Da $R_2$ und $R_3$ parallel geschaltet sind und den gleichen Widerstand besitzen, fließt durch $R_2$ ebenfalls:

$ I_{R_2} = \qty{1}{\milli\ampere} $

Der Strom durch $R_1$ ist die Summe beider Teilströme:

$ I_{R_1} = I_{R_2} + I_{R_3} = \qty{1}{\milli\ampere} + \qty{1}{\milli\ampere} = \qty{2}{\milli\ampere} $

Nun wird zuerst der Ersatzwiderstand der Parallelschaltung aus $R_2$ und $R_3$ berechnet:

$ R_{23} = \frac{R_2 \cdot R_3}{R_2 + R_3} = \frac{\qty{10}{\kilo\ohm} \cdot \qty{10}{\kilo\ohm}}
{\qty{10}{\kilo\ohm} + \qty{10}{\kilo\ohm}} = \qty{5}{\kilo\ohm} $

Der Gesamtwiderstand der Schaltung beträgt damit:

$ R_\mathrm{ges} = R_1 + R_{23} = \qty{10}{\kilo\ohm} + \qty{5}{\kilo\ohm} = \qty{15}{\kilo\ohm} $

Mit dem Gesamtstrom ergibt sich die Gesamtspannung:

$ U = I \cdot R = \qty{2}{\milli\ampere} \cdot \qty{15}{\kilo\ohm} = \qty{30}{\volt} $