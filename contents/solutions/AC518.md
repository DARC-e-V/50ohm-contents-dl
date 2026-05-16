Zunächst berechnen wir den benötigten Basisstrom:

$I_B = \frac{I_C}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere}$

Durch den Querwiderstand $R_2$ soll der zehnfache Basisstrom fließen:

$I_2 = 10 \cdot I_B = \qty{100}{\micro\ampere}$

Der Strom durch $R_1$ setzt sich aus dem Strom durch $R_2$ und dem Basisstrom zusammen:

$I_1 = I_2 + I_B = \qty{100}{\micro\ampere} + \qty{10}{\micro\ampere} = \qty{110}{\micro\ampere}$

An $R_1$ fällt die Betriebsspannung abzüglich der Basis-Emitter-Spannung ab:

$U_1 = \qty{10}{\volt} - \qty{0,6}{\volt} = \qty{9,4}{\volt}$

Damit ergibt sich:

$R_1 = \frac{U_1}{I_1} = \frac{\qty{9,4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{85,5}{\kilo\ohm}$