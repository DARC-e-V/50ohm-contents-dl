Bei einem belasteten Spannungsteiler muss berücksichtigt werden, dass der Gesamtstrom steigt, wenn die Belastung erhöht wird, d.h. der Lastwiderstand $R_\text{L}$ niederohmiger wird.
Dies gilt unter der Voraussetzung, dass der Strom der Versorgungsspannung nicht einbricht, weil er limitiert ist.

Eine schwierige Frage, deshalb soll sie im Einzelnen erklärt werden!

---
[question:AD115]

Im belasteten Spannungsteiler fließen 3 Ströme:
$I_1$ fließt durch $R_1$ und verursacht dort eine Verlustleistung $P_1 = U_1 \cdot I_1 = I_2 \cdot R_1$
$I_2$ fließt durch $R_2$ und verursacht dort eine Verlustleistung $P_2 = U_2 \cdot I_2 = {I_2}^2 \cdot R_2$
$I_\text{L}$ fließt durch $R_\text{L}$ und verursacht dort eine Verlustleistung $P_\text{L} = U_2 \cdot I_\text{L} = {I_\text{L}}^2 \cdot R_\text{L}$
Der Strom $I_1$ ist die Summe von $I_2$ und $I_\text{L}$ und damit der größte Strom.

<margin>
  Zur Veranschaulichung hilft am Besten eine Rechnung mit konkreten Bauteilwerten.
Angenommen: Alle Widerstände haben einen Wert von $\qty{1}{\kilo\ohm}$ und die Gesamtspannung $U_\text{B}$ beträgt $\qty{12}{\volt}$.
  
 *unbelasteter Fall:*
 Ohne Rechnung ist sofort zu sehen: An jedem Widerstand können $\qty{6}{\volt}$ gemessen werden.
 Der Gesamtwiderstand $R_{\mathrm{ges}}$ beträgt: $\qty{2}{\kilo\ohm}$
 $\dfrac{U_\text{B}}{U_{2}} = \frac{R_{\mathrm{ges}}}{R_{2}}$
 Der Gesamtstrom $I_1$ beträgt:  $I_1 = \frac{U_\text{B}}{R_{\mathrm{ges}}}$
 $I_1 = \frac{\qty{12}{\volt}}{\qty{2}{\kilo\ohm}} = \qty{6}{\milli\ampere}$. Dieser Strom fließt auch durch $R_2$.
 Die Verlustleistung ist an beiden Widerständen gleich groß: $P_1 = P_2 = \qty{6}{\volt} \cdot \qty{6}{\milli\ampere} = \qty{36}{\milli\watt}$
 
 *belasteter Fall:*
  Die Parallelschaltung von $R_2$ und $R_\text{L}$ ergibt einen Ersatzwiderstand von $\qty{500}{\ohm}$.
  Der Gesamtwiderstand des Spannungsteilers beträgt nun $\qty{1,5}{\kilo\ohm}$. Jetzt wirkt eine Spannungsteiler mit $\qty{1}{\kilo\ohm}$ zu $\qty{500}{\ohm}$ und dementsprechend teilt sich die Gesamtspannung auf.
  $2/3$ der Gesamtspannung kann an $R_1$ und $1/3$ der Gesamtspannung kann an $\qty{500}{\ohm}$ gemessen werden.
  Formel: $\frac{U_1}{U_\text{B}} = \frac{R_{1}}{R_{\mathrm{ges}}} \Leftrightarrow U_1 = U_\text{B} \cdot \frac{R_1}{R_{\mathrm{ges}}}$
  $U_1 = \qty{12}{\volt} \cdot \frac{\qty{1}{\kilo\ohm}}{\qty{1,5}{\kilo\ohm}}$
  $U_1 = \qty{8}{\volt}$ und am $\qty{500}{\ohm}$ Ersatzwiderstand $\qty{12}{\volt} - \qty{8}{\volt} = \qty{4}{\volt}$. 
  
Nun betrachten wir die Ströme:
  $I_1 = \qty{8}{\volt} / \qty{1}{\kilo\ohm} = \qty{8}{\milli\ampere}$. Dieser Strom steigt an.
  An $R_2$ und $R_\text{L}$ liegen jetzt nur noch $\qty{4}{\volt}$ an, deshalb sinken beide Ströme auf $I_2 = \qty{4}{\volt} / \qty{1}{\kilo\ohm} = \qty{4}{\milli\ampere}$ und $I_\text{L} = \qty{4}{\volt} / \qty{1}{\kilo\ohm} = \qty{4}{\milli\ampere}$.
  
  Wie verändern sich die Verlustleistungen?
  *An $R_1$:*  
  $P_1 = U_1 \cdot I_1 = \qty{8}{\volt} \cdot \qty{8}{\milli\ampere} = \qty{64}{\milli\watt}$ gegenüber $\qty{36}{\milli\watt}$ im unbelasteten Fall.
  *An $R_2$* : 
  $P_2 = U_2 \cdot I_2 = \qty{4}{\volt} \cdot \qty{4}{\milli\ampere} = \qty{16}{\milli\watt}$ gegenüber $\qty{36}{\milli\watt}$ im unbelasteten Fall.
  *An $R_\text{L}$:*  
  $P_\text{L} = U_\text{L} \cdot I_\text{L} = \qty{4}{\volt} \cdot \qty{4}{\milli\ampere} = \qty{16}{\milli\watt}$.
</margin>

Merke: Bei der Dimensionierung eines Spannungsteiler ist die Stromstärke durch die Widerstände zu berücksichtigen. Der Strom $I_1$ steigt, wenn ein Lastwiderstand angeschlossen wird und dadurch wird $R_1$ wärmer.

% Spannungsteiler müssen eine bestimmte Belastbarkeit besitzen, die von der Stromstärke durch die Widerstände abhängt.



