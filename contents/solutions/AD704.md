Wie in der Schaltung gezeigt, gilt für die Ausgangsfrequenz des VCO im eingerasteten Zustand der PLL:

$f_{VCO} = n \cdot f_A$

Umgestellt nach dem Teilerverhältnis *n* ergibt sich:

$n = \frac{f_{VCO}}{f_A}$

Für die *untere Grenze* des gewünschten Ausgangsbereichs mit $f_{VCO} = \qty{12,000}{\mega\hertz}$ und $f_A = \qty{12,5}{\kilo\hertz}$ folgt:

$n_{min} = \frac{\qty{12000000}{\hertz}}{\qty{12500}{\hertz}} = 960$

Für die *obere Grenze* mit $f_{VCO} = \qty{14,000}{\mega\hertz}$ folgt:

$n_{max} = \frac{\qty{14000000}{\hertz}}{\qty{12500}{\hertz}} = 1120$

Das Teilerverhältnis *n* muss sich also im Bereich von *960* bis *1120* bewegen.