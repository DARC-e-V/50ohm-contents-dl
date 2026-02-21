% In Bearbeitung! Um was geht es denn hier???
% Das habe ich mir alles aus den Fingern gezogen!

In der Formelsammlung findet man unter Punkt  6.2, Formelzeichen, Konstanten und Tabellen, auch die Formel für $Z_{F0}$ den Feldwellenwiderstand des freien Raumes (Vakuum).
$Z_{F0} = \sqrt{\dfrac{\mu_0}{\varepsilon_0}}$

$\mu_0$ die magnetische Feldkonstante, $\varepsilon_0$ die elektrische Feldkonstante

Die in der Frage angesprochene **magnetischen Feldstärke** wird mit Hilfe magnetische Feldkonstante, der magnetischen Flussdichte und der Magnetisierung berechnet. Deutlich komplexer ist der Zusammenhang der elektrischen Feldkonstante und der **elektrischen Feldstärke**.

In einem Medium (z.B. Luft) ist der Wellenwiderstand  $Z_{F}$ von $\mu$, der magnetische Feldkonstante und $\varepsilon$, der elektrische Feldkonstante des Mediums abhängig.

$Z_{F} = \sqrt{\dfrac{\mu}{\varepsilon}}$

Es gibt eine Abhängigkeit von Feldwellenwiderstand, elektrischer und magnetischer Feldstärke. Damit ist auch die elektrische und magnetische Feldstärke von dem Wellenwiderstand des Mediums abhängig.


[question:AK102]

% Wie errechnen Sie die Leistung am Einspeisepunkt der Antenne (Antenneneingangsleistung) bei bekannter Senderausgangsleistung?

Die Leistung am Speisepunkt der Antenne ergibt sich aus der Senderausgangsleistung und der Dämpfung der Speiseleitung. Jede Dämpfung kann in einen Dämpfungsfaktor übertragen werden. Zum Beispiel, bei $\qty{10}{\dB}$ Dämpfung ist der Faktor $\num{0,1}$.
Die Berechnung ist einfach: $P_{Ant} = D \cdot P_{Sender}$ (D steht für Dämpfungsfaktor)

[question:AK104]
% In Bearbeitung!
 Im § 8, BEMFV ist u.a. festgelegt, dass der standortbezogene Sicherheitsabstand innerhalb des kontrollierbaren Bereichs liegen muss. Oft ist dieser Abstand durch die örtlichen Gegebenheiten festgelegt und kann nicht verändert werden. In diesen Fällen muss die maximale Sendeleistung angepasst werden.
 
In die Strahlungsleistung geht neben der Sendeleistung der Antennengewinn in $\unit{\dBi}$ ein. Angegeben sind $\qty{6}{\dBd}$. Bezogen auf den isotropen Strahler sind dies $\qty{6}{\dBd} + \qty{2,15}{\dB}$. Das ergibt einen Gewinnfaktor von $G_i = 4 \cdot 1,64 = 6,56$.

Jetzt kann die maximale Sendeleistung ermittelt werden. Dazu muss die Formel für die Feldstärke im Fernfeld einer Antenne umgestellt werden:
 $\begin{split}E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_A\cdot G_i}}{d}\\ E \cdot d &= \sqrt{\qty{30}{\ohm}\cdot P_A\cdot G_i}\\ E^2 \cdot d^2 &= \qty{30}{\ohm}\cdot P_A\cdot G_i\\ \dfrac{E^2 \cdot d^2}{\qty{30}{\ohm}\cdot G_i} &= P_A\\ P_A &= \dfrac{E^2 \cdot d^2}{\qty{30}{\ohm}\cdot G_i}\\ P_A &= \qty{\dfrac{28^2 \cdot 5^2}{30 \cdot 6,56}}{\watt}\\ P_A &\approx \qty{99,59}{\watt}\end{split}$
Die Sendeleistung muss auf ca. $\qty{100}{\watt}$ beschränkt werden.
  
  Nur zur Sicherheit die Einheitengleichung. Das Ergebnis hat die Einheit Watt.
 $\begin{split} \unit{\watt} &= \dfrac{\left(\unit{\volt\per\meter}\right)^2 \cdot \unit{m\squared}}{\unit{\volt\per\ampere}}\\ \unit{\watt} &= \dfrac{\unit{\volt} \cdot \unit{\volt} \cdot \unit{m\squared} \cdot A}{\unit{\volt} \cdot \unit{m\squared}}\\ \unit{\watt} &= \unit{\volt} \cdot \unit{\ampere}\\ \unit{\watt} &= \unit{\watt}\end{split}$
 
 Die Formel für die Feldstärke gilt nur für das Fernfeld. Ob das bei den vorgegeben $\qty{5}{\meter}$ erfüllt ist, kann schnell überprüft werden.

$\begin{split}d &> \dfrac{\lambda}{2 \cdot \pi}\\ d &= \dfrac{\qty{2,06}{\meter}}{2 \cdot \pi}\\ d &\approx \qty{0,33}{\meter}\end{split}$
Der Sicherheitsabstand von $d=\qty{5}{\meter}$ ist deutlich im Fernfeld.

[question:AK107]

Bei den drei nächsten Fragen ist die Vorgehensweise mehr oder weniger gleich.
Für die Berechnung der elektrischen Feldstärke wird Leistung am Speisepunkt der Antenne, der Gewinnfaktor und die Entfernung gebraucht.

$P_A$, Leistung am Speisepunkt: $\qty{250}{\watt}$ (kein Kabel, direkte Einspeisung)

$G_i$, Gewinnfaktor: $\qty{12,15}{\dBi}$ oder $\qty{10}{\dBi}$ und $\qty{2,15}{\dBi}$, das entspricht den Faktoren $10 \cdot 1,64 = 16,4$

$d$, Entfernung: $\qty{30}{\meter}$

Die Formel gilt nur für das Fernfeld. Dies kann mit $d > \dfrac{\lambda}{2 \cdot \pi}$ überprüft werden.
$\begin{split}E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_A\cdot G_i}}{d}\\ E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot \qty{250}{\watt}\cdot 16,4}}{\qty{30}{\meter}}\\ E &\approx \qty{11,7}{\volt\per\meter}\end{split}$

[question:AK113]

$P_A$, Leistung am Speisepunkt: $\qty{10}{\watt}$ (kein Kabel, direkte Einspeisung)

$G_i$, Gewinnfaktor: $\qty{2,15}{\dBi}$, das entspricht dem Faktor $\num{1,64}$ (Dipol als Antenne)

$d$, Entfernung: $\qty{10}{\meter}$

Die Formel gilt nur für das Fernfeld. Dies kann mit $ d > \dfrac{\lambda}{2 \cdot \pi}$ überprüft werden.
$\begin{split}E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_A\cdot G_i}}{d}\\ E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot \qty{10}{\watt}\cdot 1,64}}{\qty{10}{\meter}}\\ E &\approx \qty{2,2}{\volt\per\meter}\end{split}$

[question:AK114]
% AK115: Eine Amateurfunkstelle sendet in FM mit einer äquivalenten Strahlungsleistung (ERP) von 100 W. Wie groß ist die Feldstärke im freien Raum in einer Entfernung von 100 m?

$P_A$, Leistung am Speisepunkt: $\qty{100}{\watt}$ (Strahlungsleistung in ERP)

$G_i$, Gewinnfaktor: $\qty{2,15}{\dBi}$, das entspricht dem Faktor $\num{1,64}$ (Strahlungsleistung in ERP, Faktor für EIRP)

$d$, Entfernung: $\qty{100}{\meter}$

Die Formel gilt nur für das Fernfeld. Dies kann mit $ d > \dfrac{\lambda}{2 \cdot \pi}$ überprüft werden.
$\begin{split}E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_A\cdot G_i}}{d}\\ E &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot \qty{100}{\watt}\cdot 1,64}}{\qty{100}{\meter}}\\ E &\approx \qty{0,7}{\volt\per\meter}\end{split}$

[question:AK115]