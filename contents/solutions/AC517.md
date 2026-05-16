Zuerst wird der Basisstrom berechnet:

$ I_B = \frac{I_C}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere} $

Durch $R_2$ soll der zehnfache Basisstrom fließen:

$ I_2 = 10 \cdot I_B = \qty{100}{\micro\ampere} $

Der Strom durch $R_1$ ist somit:

$ I_1 = I_2 + I_B = \qty{110}{\micro\ampere} $

Am Emitterwiderstand fallen $\qty{1}{\volt}$ ab.  
Zusätzlich benötigt der Basis-Emitter-Übergang etwa $\qty{0,6}{\volt}$.

Damit liegt die Basisspannung bei:

$ U_B = \qty{1}{\volt} + \qty{0,6}{\volt} = \qty{1,6}{\volt} $

Die Spannung über $R_1$ beträgt daher:

$ U_1 = \qty{10}{\volt} - \qty{1,6}{\volt} = \qty{8,4}{\volt} $

Nun folgt mit dem Ohmschen Gesetz:

$ R_1 = \frac{U_{R_1}}{I_{R_1}} = \frac{\qty{8,4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{76,4}{\kilo\ohm} $
