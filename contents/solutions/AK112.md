## Benötigte Formeln

Zu nutzende Formeln aus den Hilfsmitteln der Bundesnetzagentur zur Berechnung des Sicherheitsabstands im Fernfeld:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{E}$ 

und zum Leistungszusammenhang EIRP und ERP:

$P_{EIRP} = P_{ERP} \cdot 10^{\frac{g_d + 2,15 - a}{10}}$

## Angaben aus der Aufgabenstellung

1. Da es sich um einen Parabolspiegel handelt, gilt: $g_d = \qty{18}{\dBd}$ 
2. Die Kabeldämpfung beträgt: $a = \qty{2}{\dB}$
3. Die Leistung beträgt: $P_{ERP} = \qty{40}{\watt}$
4. Der Grenzwert für den Personenschutzabstand ist: $E = \qty{61}{\volt\per\meter}$

## Lösungschritte

1. Berechnung von $P_{EIRP}$:

$P_{EIRP} = \qty{40}{\watt} \cdot 10^{\frac{18 + 2,15 - 2}{10}} = \qty{2612,52}{\watt}$

2. Berechnung des Sicherheitsabstands $d$:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{2612,52}{\watt}}}{\qty{61}{\volt\per\meter}} = \frac{\qty{279,96}{\volt}}{\qty{61}{\volt\per\meter}} \approx \qty{4,6}{\meter}$


## Interpretation

Der Sicherheitsabstand beträgt $\qty{4,6}{\meter}$.

