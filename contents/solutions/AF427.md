Gegeben sind:

$ U_\mathrm{CC} = \qty{9}{\volt} $

$ R_\text{BIAS} = \qty{470}{\ohm} $

Aus der Schaltung ist außerdem ersichtlich:

$ U_D = \qty{4}{\volt} $

Am Widerstand $R_\text{BIAS}$ fällt daher die Differenzspannung ab:

$ U_{\text{BIAS}} = U_\mathrm{CC} - U_D = \qty{9}{\volt} - \qty{4}{\volt} = \qty{5}{\volt} $

Damit ergibt sich der Strom durch $R_\text{BIAS}$ und den MMIC zu:

$ I_D = \frac{U_{\text{BIAS}}}{R_\text{BIAS}} = \frac{\qty{5}{\volt}}{\qty{470}{\ohm}} \approx \qty{10,6}{\milli\ampere} $

Die im MMIC umgesetzte Wärmeleistung beträgt:

$ P_D = U_D \cdot I_D = \qty{4}{\volt} \cdot \qty{10,6}{\milli\ampere} \approx \qty{42,6}{\milli\watt} $

Gerundet ergibt sich:

$ P_D \approx \qty{43}{\milli\watt} $
