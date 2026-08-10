Zunächst betrachten wir den Eingangswiderstand der Schaltung. Dieser sollte im Amateurfunk genau $\qty{50}{\ohm}$ betragen. Den Teil der Rechnung kann man also eigentlich überspringen. Der Vollständigkeit halber zeigen wir trotzdem, dass sich hier ingesamt $\qty{50}{\ohm}$ ergeben 

Der Spannungsteiler aus den beiden Widerständen mit jeweils $\qty{330}{\ohm}$ hat insgesamt:

$R_\mathrm{T}=\qty{330}{\ohm}+\qty{330}{\ohm}=\qty{660}{\ohm}$

Dieser liegt parallel zu $R_1=\qty{54,1}{\ohm}$:

$R_\mathrm{in}=R_1\parallel R_\mathrm{T}$

$R_\mathrm{in}=\frac{\qty{54,1}{\ohm}\cdot\qty{660}{\ohm}}{\qty{54,1}{\ohm}+\qty{660}{\ohm}}\approx\qty{50}{\ohm}$

Die Schaltung bildet somit näherungsweise einen $\qty{50}{\ohm}$-Abschluss.

Am Ausgang werden $\qty{14,9}{\volt}$ Gleichspannung gemessen. Wegen der Durchlassspannung der Siliziumdiode von $\qty{0,7}{\volt}$ muss der HF-Spitzenwert am Eingang der Diode um diesen Betrag größer sein:

$\hat U_\mathrm{D}=\qty{14,9}{\volt}+\qty{0,7}{\volt}=\qty{15,6}{\volt}$

Die Diode liegt am Mittelpunkt des Spannungsteilers aus den beiden gleichen $\qty{330}{\ohm}$-Widerständen. Dort liegt daher nur die halbe HF-Eingangsspannung an. Der Spitzenwert am Eingang beträgt somit:

$\hat U_\mathrm{in}=2\cdot\qty{15,6}{\volt}=\qty{31,2}{\volt}$

Für die Leistungsberechnung benötigen wir den Effektivwert:

$U_\mathrm{eff}=\frac{\hat U_\mathrm{in}}{\sqrt{2}}=\frac{\qty{31,2}{\volt}}{\sqrt{2}}\approx\qty{22,1}{\volt}$

Damit ergibt sich die HF-Leistung:

$P=\frac{U_\mathrm{eff}^2}{R_\mathrm{in}}=\frac{(\qty{22,1}{\volt})^2}{\qty{50}{\ohm}}\approx\qty{9,7}{\watt}$

Die HF-Eingangsleistung beträgt somit ungefähr $\qty{9,7}{\watt}$.