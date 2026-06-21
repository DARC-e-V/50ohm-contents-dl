## Benötigte Formeln

Zu nutzende Formeln aus den Hilfsmitteln der Bundesnetzagentur zur Berechnung des Sicherheitsabstands im Fernfeld:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E}$ 

und zum Leistungszusammenhang EIRP und ERP:

$P_\mathrm{EIRP} = P_\mathrm{ERP} \cdot 10^{\frac{g_i - a}{10}}$

## Angaben aus der Aufgabenstellung

1. Da es sich um einen Dipol handelt, gilt: $g_i = \qty{2,15}{\dBi}$ 
2. Die Kabeldämpfung beträgt: $a = \qty{0,5}{\dB}$
3. Die Leistung beträgt: $P_\mathrm{ERP} = \qty{700}{\watt}$
4. Der Grenzwert für den Personenschutzabstand ist: $E = \qty{28}{\volt\per\meter}$

## Lösungschritte

1. Berechnung von $P_\mathrm{EIRP}$:

$P_\mathrm{EIRP} = \qty{700}{\watt} \cdot 10^{\frac{2,15 - 0,5}{10}} = \qty{1023,5}{\watt}$

2. Berechnung von $d$:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{1023,5}{\watt}}}{\qty{28}{\volt\per\meter}} = \frac{\qty{175,23}{\volt}}{\qty{28}{\volt\per\meter}} \approx \qty{6,26}{\meter}$


## Interpretation

Der gesuchte Sicherheitsabstand beträgt $\qty{6,26}{\meter}$.

