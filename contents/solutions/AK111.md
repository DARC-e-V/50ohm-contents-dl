## Benötigte Formeln

Zu nutzende Formeln aus den Hilfsmitteln der Bundesnetzagentur zur Berechnung des Sicherheitsabstands im Fernfeld:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E}$ 

und zum Leistungszusammenhang EIRP und ERP:

$P_\mathrm{EIRP} = P_\mathrm{ERP} \cdot 10^{\frac{g_d + 2{,}15 - a}{10}}$

## Angaben aus der Aufgabenstellung

1. Da es sich um eine Yagi-Uda-Antenne handelt, gilt: $g_d = \qty{10,5}{\dBd}$ 
2. Die Kabeldämpfung beträgt: $a = \qty{1,5}{\dB}$
3. Die Leistung beträgt: $P_\mathrm{ERP} = \qty{100}{\watt}$
4. Der Grenzwert für den Personenschutzabstand ist: $E = \qty{28}{\volt\per\meter}$

## Lösungschritte

1. Berechnung von $P_\mathrm{EIRP}$:

$P_\mathrm{EIRP} = \qty{100}{\watt} \cdot 10^{\frac{10,5 + 2,15 - 1,5}{10}} = \qty{1303,17}{\watt}$

2. Berechnung des Sicherheitsabstands $d$:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{1303,17}{\watt}}}{\qty{28}{\volt\per\meter}} = \frac{\qty{197,72}{\volt}}{\qty{28}{\volt\per\meter}} = \qty{7,06}{\meter}$


## Interpretation

Der ermittelte Sicherheitsabstand beträgt $\qty{7,06}{\meter}$.

