## Benötigte Formeln

Zu nutzende Formeln aus den Hilfsmitteln der Bundesnetzagentur zur Berechnung des Sicherheitsabstands im Fernfeld:

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E}$ 

und zum Leistungszusammenhang EIRP und ERP:

$P_\mathrm{EIRP} = P_\mathrm{ERP} \cdot 10^{\frac{g_d + 2{,}15 - a}{10}}$

## Umstellung der Formel

$d = \frac{\sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}}{E}$ 
$d \cdot E = \sqrt{\qty{30}{\ohm} \cdot P_\mathrm{EIRP}}$
$(d \cdot E)^2 = \qty{30}{\ohm} \cdot P_\mathrm{EIRP}$
$\frac{(d \cdot E)^2}{\qty{30}{\ohm}} = P_\mathrm{EIRP}$
$P_\mathrm{EIRP} = \frac{(d \cdot E)^2}{\qty{30}{\ohm}}$

## Angaben aus der Aufgabenstellung

1. Der angegebene Antennengewinn gegenüber dem Dipol: $g_d = \qty{6}{\dBd}$ 
2. Die Kabeldämpfung ist zu vernachlässigen: $a = \qty{0}{\dB}$
3. Der Sicherheitsabstand beträgt: $d = \qty{5}{\meter}$
4. Der Grenzwert für den Personenschutzabstand ist: $E = \qty{28}{\volt\per\meter}$


## Lösungschritte

1. Berechnung von $P_\mathrm{EIRP}$:

$P_\mathrm{EIRP} = \frac{(\qty{5}{\meter} \cdot \qty{28}{\volt\per\meter})^2}{\qty{30}{\ohm}} = \qty{653,33}{\watt}$

2. Berechnung von $P_\mathrm{ERP}$:

$P_\mathrm{ERP} = \frac{P_\mathrm{EIRP}}{10^{\frac{g_d + 2{,}15 -a}{10}}} = \frac{\qty{653,33}{\watt}}{10^{\frac{6 + 2{,}15 -0}{10}}} = \frac{\qty{653,33}{\watt}}{6,531} \approx \qty{100}{\watt}$

## Interpretation

Die maximale Ausgangsleistung des Senders darf ca. $\qty{100}{\watt}$ nicht übersteigen.