Bei einem belasteten Spannungsteiler muss berücksichtigt werden, dass der Gesamtstrom steigt, wenn die Belastung erhöht wird, d.h. der Lastwiderstand $R_L$ niederohmiger wird.
Dies gilt unter der Voraussetzung, dass der Strom der Versorgungsspannung nicht einbricht, weil er limitiert ist.

Eine schwierige Frage, deshalb soll sie im Einzelnen erklärt werden!

---
[question:AD115]

Im belasteten Spannungsteiler fließen 3 Ströme:
$I_1$ fließt durch $R_1$ und verursacht dort eine Verlustleistung $P_1$ = $U_1$ * $I_1$ = $I_2$ * $R_1$
$I_2$ fließt durch $R_2$ und verursacht dort eine Verlustleistung $P_2$ = $U_2$ * $I_2$ = ${I_2}^2$ * $R_2$
$I_L$ fließt durch $R_L$ und verursacht dort eine Verlustleistung $P_L$ = $U_2$ * $I_L$ =  ${I_L}^2$ * $R_L$
Der Strom $I_1$ ist die Summe von $I_2$ und $I_L$ und damit der größte Strom.

<margin>
  Zur Veranschaulichung hilft am Besten eine Rechnung mit konkreten Bauteilwerten.
Angenommen: Alle Widerstände haben einen Wert von 1 kOhm und die Gesamtspannung $U_B$ beträgt 12 V.
  
 *unbelasteter Fall:*
 Ohne Rechnung ist sofort zu sehen: An jedem Widerstand können 6 V gemesen werden.
 Der Gesamtwiderstand $R_{ges}$ beträgt: 2 kOhm
 $\dfrac{ U_{ges1 } }{ U_{ 2 } } = \frac{R_{ges }}{R_{2}}$
 Der Gesamtstrom $I_1$ beträgt:  $I_1$ = $ \frac {U_B}{R_{ges}}$ 
 $I_1$ =$ \frac {12\ \text{V}}{2\ \text{k}\Omega}$ = 6 mA.  Dieser Strom fließt auch durch $R_2$.
 Die Verlustleistung ist an beiden Widerständen gleich groß: $P_1$ = $P_2$ = 6 V $\cdot\  6 \text{mA}$ = 36 mW
 
 *belasteter Fall:*
  Die Parallelschaltung von $R_2$ und $R_L$ ergibt einen Ersatzwiderstand von 500 Ohm.
  Der Gesamtwiderstand des Spannungsteilers beträgt nun 1, 5 kOhm. Jetzt wirkt eine Spannungsteiler mit 1 kOhm zu 500 Ohm und dementsprechend teilt sich die Gesamtspannung auf.
  2/3 der Gesamtspannung kann an $R_1$ und 1/3 der Gesamtspannung kann an 500 Ohm gemessen werden.
  Formel: $\frac {U_1}{U_{ges}} =  \frac {R_{1}}{R_{ges}}   \  \ \    U_1 = U_{ges} * \frac {R_1}{R_{ges}}$ 
  $U_1$ = 12 V  * ${\frac {1 \ \text{k}\Omega}{1,5\  \text{k}\Omega}}$
  $U_1$ = 8 V  und am 500 Ohm Ersatzwiderstand 12 V - 8 V = 4 V. 
  
Nun betrachten wir die Ströme:
  $I_1$ = 8 V / 1 kOhm = 8 mA. Dieser Strom steigt an.
  An $R_2$ und $R_L$ liegen jetzt nur noch 4 V an, deshalb sinken beide Ströme auf $I_2$ = 4 V / 1 kOhm = 4 mA und $I_L$ = 4 V / 1 kOhm = 4 mA.
  
  Wie verändern sich die Verlustleistungen?
  *An $R_1$:*  
  $P_1$ = $U_1$ * $I_1$ = 8 V * 8 mA = 64 mW gegenüber 36 mW im unbelasteten Fall.
  *An $R_2$* : 
  $P_2$ = $U_2$ * $I_2$ = 4 V * 4mA = 16 mW gegenüber 36 mW im unbelasteten Fall.
  *An $R_L$:*  
  $P_L$ = $U_L$ * $I_L$ = 4 V * 4mA = 16 mW.
</margin>

Merke: Bei der Dimensionierung eines Spannungsteiler ist die Stromstärke durch die Widerstände zu berücksichtigen. Der Strom $I_1$ steigt, wenn ein Lastwiderstand angeschlossen wird und dadurch wird $R_1$ wärmer.

% Spannungsteiler müssen eine bestimmte Belastbarkeit besitzen, die von der Stromstärke durch die Widerstände abhängt.



