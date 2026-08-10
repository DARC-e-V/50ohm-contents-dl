Diese Schaltung arbeitet als Spannungsverdoppler beziehungsweise Spitze-Spitze-Detektor. Die positive und die negative Spitze des HF-Signals werden erfasst, sodass am Ausgang näherungsweise die Spitze-Spitze-Spannung abzüglich der Durchlassspannungen beider Dioden zur Verfügung steht.

$U_{\mathrm{SS}} = \qty{15,3}{\volt} + 2 \cdot \qty{0,23}{\volt} = \qty{15,76}{\volt}$

Aus

$U_{\mathrm{SS}} = 2 \cdot \hat{U}$

folgt für den Spitzenwert der HF-Spannung an der $\qty{5}{\ohm}$-Anzapfung:

$\hat{U} = \frac{U_{\mathrm{SS}}}{2} = \qty{7,88}{\volt}$

Die Spannung wird an einer $\qty{5}{\ohm}$-Anzapfung der insgesamt $\qty{50}{\ohm}$ großen Dummyload gemessen. Da durch die gesamte Dummyload derselbe Strom fließt, verhalten sich die Spannungen wie die Widerstände. Die HF-Spitzenspannung über der gesamten Dummyload beträgt daher:

$\hat{U}_{\mathrm{Sender}} = \frac{\qty{50}{\ohm}}{\qty{5}{\ohm}} \cdot \hat{U} = 10 \cdot \qty{7,88}{\volt} = \qty{78,8}{\volt}$

Mit

$\hat{U} = U_{\mathrm{eff}} \cdot \sqrt{2}$

und

$P = \frac{U_{\mathrm{eff}}^2}{R}$

ergibt sich:

$P = \frac{\hat{U}_{\mathrm{Sender}}^2}{2R} = \frac{(\qty{78,8}{\volt})^2}{2 \cdot \qty{50}{\ohm}} \approx \qty{62}{\watt}$

Die HF-Leistung des Senders beträgt somit ungefähr $\qty{60}{\watt}$.