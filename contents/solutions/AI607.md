Die beiden Dioden bilden eine doppelte Spitzenwertgleichrichtung. Am Ausgang werden $\qty{15,3}{\volt}$ gemessen. Zusätzlich müssen die Durchlassspannungen der beiden Schottkydioden mit jeweils $\qty{0,23}{\volt}$ berücksichtigt werden:

$U_\mathrm{SS} = \qty{15,3}{\volt} + 2 \cdot \qty{0,23}{\volt} = \qty{15,76}{\volt}$

Der Spitzenwert der HF-Spannung beträgt damit:

$\hat U = \frac{U_\mathrm{SS}}{2} = \frac{\qty{15,76}{\volt}}{2} = \qty{7,88}{\volt}$

Für die Leistungsberechnung wird der Effektivwert benötigt:

$U_\mathrm{eff} = \frac{\hat U}{\sqrt{2}} = \frac{\qty{7,88}{\volt}}{\sqrt{2}} \approx \qty{5,57}{\volt}$

Die Widerstände mit $\qty{56}{\ohm}$ und $\qty{470}{\ohm}$ liegen parallel und bilden näherungsweise einen $\qty{50}{\ohm}$-Abschluss:

$R = \qty{56}{\ohm} \parallel \qty{470}{\ohm} \approx \qty{50}{\ohm}$

Damit ergibt sich die HF-Leistung:

$P = \frac{U_\mathrm{eff}^2}{R} = \frac{(\qty{5,57}{\volt})^2}{\qty{50}{\ohm}} \approx \qty{0,62}{\watt}$

Die HF-Leistung beträgt somit ungefähr $\qty{600}{\milli\watt}$.