%Um die Feldstärke einer Antenne im Fernfeld ($d>\frac \lambda {2 \pi}$) zu berechnen gibt es die folgende Näherungsformel:

%$E=\frac{\sqrt{\qty{30}{\ohm} \cdot P_\text{A} \cdot G_\text{i}}} {d}=\frac {\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}} d$

%mit der Leistung an der Antenne $P_\text{A}$, dem Gewinnfaktor bezogen auf den Isotropen Strahler %$G_\text{i}$, und dem Abstand $d$

%Für den Gewinnfaktor von Antennen ist gegeben:

%$G_\text{i}=G_\text{d} \cdot 1,64$ 

%bzw.

%$g_\text{i} = g_\text{d}+2,15\text{ dB}$

%Es ist in der Prüfung der Grenzwert für den Personenschutzabstand angegeben. Um den Personenschutzabstand dann zu berechnen, muss daher die Formel umgestellt werden zu

%$d=\frac{\sqrt{\qty{30}{\ohm} \cdot P_\text{A} \cdot G_\text{i}}} {E}$

%Jedoch ist meist nicht die Leistung an der Antenne angegeben, und genauso wenig der Gewinn gegenüber einem Isotropen Strahler. Entsprechend muss dies mit berücksichtigt werden. Dies ergibt dann:

%$d=\dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{Transceiver} \cdot G_\text{Kabel} \cdot G_\text{d} \cdot 1,64}} {E}$

%Mit der Leistung am Transceiver $P_\text{Transceiver}$, dem "Gewinn" des Kabels $G_\text{Kabel}$ (hier entsprechend mit negativem Vorzeichen einsetzen) und dem Gewinn gegenüber dem Dipol $G_\text{d}$.

%Der "Gewinn" des Kabels kann z.B. berechnet werden für ein Kabel mit einer Dämpfung von $2 \text{ dB}$:
%$G_\text{Kabel} = 10^{\frac {-2 \text{ dB}} {10 \text{ dB}}} = 10^{-0,2}= 0,631$

% DD4UQ
Bei der Anzeige einer ortsfesten Amateurfunkanlage können die Sicherheitsabstände nach verschiedenen Verfahren ermittelt werden. Eine davon ist die Fernfeldberechnung. 
Für die Berechnung braucht man die Sendeleistung ($P_\text{S}$), den Gewinnfaktor der Antenne bezogen auf den isotropen Strahler ($G_i = 1,64$) und den Grenzwert für die Feldstärke $(E = \qty{28}{\volt\per\meter})$ im Fernfeld einer Antenne. Die Wellenlänge ($\qty{10}{\meter}$) ist nur angebeben um den Beginn des Fernfeldes zu ermitteln.

$\begin{split} d &=\dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{A} \cdot G_\text{i}}}{E}\\ d &=\dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{100}{\watt} \cdot 1,64}}{\qty{28}{\volt\per\meter}}\\ d &\approx \qty{2,50}{\meter}\end{split}$

Ist der Abstand im Fernfeld (strahlenden Nahfeld)?

 $\begin{split}d &= \dfrac{\lambda}{2 \cdot \pi}\\ d &= \dfrac{\qty{10}{\meter}}{2 \cdot \pi}\\ d &\approx \qty{1,59}{\meter}\end{split}$
 
 Der Sicherheitsabstand von $\qty{2,50}{\meter}$ liegt deutlich im Fernfeld (strahlenden Nahfeld) und ist damit gültig.

[question:AK106]

Die Frage AK108  ähnelt der vorherigen Frage. Hier muss zusätzlich die Kabeldämpfung beachtet werden. 

Hier bietet sich an, erst die ERIP zu berechnen.

$P_\text{EIRP} = P_S \cdot {10^\dfrac{g_d  −  a  +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}$
Bei einer Richtantenne muss der Wert für $g_d$ angegeben werden. Ein einfacher Dipol hat nur einen Gewinn in Bezug auf einen isotropen Strahler. Hier ist  $g_d = \qty{0}{\dBd}$.
$\begin{split}P_\text{EIRP} &= \qty{300}{\watt}\cdot {10^\dfrac{\qty{0}{\dBd} −  \qty{0,5}{\dB} +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{300}{\watt}\cdot {10^\dfrac{\qty{1,65}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{300}{\watt}\cdot {10^{0,165}}\\ P_\text{EIRP} &\approx \qty{438,65}{\watt}\end{split}$

Nun kann der Sicherheitsabstand berechnet werden.

$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{438,65}{\watt}}} {\qty{28}{\volt\per\meter}}\\ d &\approx \qty{4,10}{\meter}\end{split}$

Ist der Abstand im Fernfeld (strahlenden Nahfeld)?

 $\begin{split} d &= \dfrac{\lambda}{2 \cdot \pi}\\ d &= \dfrac{\qty{20}{\meter}}{2 \cdot \pi}\\ d &\approx \qty{3,18}{\meter}\end{split}$
 
 Der Sicherheitsabstand von $\qty{4,10}{\meter}$ liegt auch hier im Fernfeld (strahlenden Nahfeld) und ist damit gültig.

[question:AK108]

Hier kann geauso vorgegangen werden, wie bei der vorherigen Frage.
$\begin{split} P_\text{EIRP} &= P_S \cdot {10^\dfrac{g_d  −  a  +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{700}{\watt}\cdot {10^\dfrac{\qty{0}{\dBd} −  \qty{0,5}{\dB} +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{700}{\watt}\cdot {10^\dfrac{\qty{1,65}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{700}{\watt}\cdot {10^{0,165}}\\ P_\text{EIRP} &\approx \qty{1023,52}{\watt}\end{split}$

$\begin{split} d & =\dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{1023,52}{\watt}}} {\qty{28}{\volt\per\meter}}\\ d &\approx \qty{6,26}{\meter}\end{split}$

[question:AK109]

Bei der nächsten Frage muss der Sicherheitsabstand für ein Richtantenne berechnet werden. Der Gewinn $g_d = \qty{11,5}{\dBd}$.

$\begin{split} P_\text{EIRP} &= P_S \cdot {10^\dfrac{g_d  −  a  +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{75}{\watt}\cdot {10^\dfrac{\qty{11,5}{\dB} −  \qty{1,5}{\dB} +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{75}{\watt}\cdot {10^\dfrac{\qty{12,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{75}{\watt}\cdot {10^{1,215}}\\ P_\text{EIRP} &\approx \qty{1230,44}{\watt}\end{split}$

$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{1230,44}{\watt}}} {\qty{28}{\volt\per\meter}}\\ d &\approx \qty{6,86}{\meter}\end{split}$

 Ist der Abstand im Fernfeld (strahlenden Nahfeld)?

 $\begin{split} d &= \dfrac{\lambda}{2 \cdot \pi}\\ d &= \dfrac{\qty{2}{\meter}}{2 \cdot \pi}\\ d &\approx \qty{0,32}{\meter}\end{split}$
 
 Der Sicherheitsabstand von $\qty{6,86}{\meter}$ liegt auch hier im Fernfeld (strahlenden Nahfeld) und ist damit gültig.

[question:AK110]

Die Vorgehensweise ist analog der, der vorhergehenden Frage.

$\begin{split} P_\text{EIRP} &= P_S \cdot {10^\dfrac{g_d  −  a  +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{100}{\watt}\cdot {10^\dfrac{\qty{10,5}{\dBd} −  \qty{1,5}{\dB} +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{100}{\watt}\cdot {10^\dfrac{\qty{11,15}{\dBd}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{100}{\watt}\cdot {10^{1,115}}\\ P_\text{EIRP} &\approx \qty{1303,17}{\watt}\end{split}$

$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{1303,17}{\watt}}} {\qty{28}{\volt\per\meter}}\\ d &\approx \qty{7,1}{\meter}\end{split}$

Der Sicherheitsabstand von $\qty{7,1}{\meter}$ liegt auch hier im Fernfeld (strahlenden Nahfeld).

[question:AK111]

Das $\qty{13}{\centi\meter}$-Band reicht von $\qtyrange{2320}{2450}{\mega\hertz}$. Für den Frequenzbereich $\qtyrange{2000}{300000}{\mega\hertz}$ ist der Grenzwert für die elektrische Feldstärke $\qty{61}{\volt\per\meter}$.

$\begin{split} P_\text{EIRP} &= P_S \cdot {10^\dfrac{g_d  −  a  +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{40}{\watt}\cdot {10^\dfrac{\qty{18}{\dBd} −  \qty{2}{\dB} +  \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{40}{\watt}\cdot {10^\dfrac{\qty{18,15}{\dB}}{\qty{10}{\dB}}}\\ P_\text{EIRP} &= \qty{40}{\watt}\cdot {10^{1,815}}\\ P_\text{EIRP} &\approx \qty{2612,52}{\watt}\end{split}$

$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_\text{EIRP}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{2612,52}{\watt}}} {\qty{61}{\volt\per\meter}}\\ d &\approx \qty{4,6}{\meter}\end{split}$

Ist der Abstand im Fernfeld (strahlenden Nahfeld)?

$\begin{split} d &= \dfrac{\lambda}{2 \cdot \pi}\\ d &= \dfrac{\qty{0,13}{\meter}}{2 \cdot \pi}\\ d &\approx \qty{0,02}{\meter}\end{split}$

Der Sicherheitsabstand von $\qty{4,6}{\meter}$ liegt deutlich im Fernfeld (strahlenden Nahfeld).

[question:AK112]

<indepth>
Warum wird in den Fragen in diesem Abschnitt auf Modulationsverfahren RTTY und FM hingewiesen?
Bei der Anzeige einer ortsfesten Amateurfunkanlage (nach § 9, BEMFV) ist bei der Konfiguration der Umrechnungsfaktor $\textrm{Faktor}_\textrm{FmodPers}$ einzutragen.
Mit dem Faktor wird die angegebene Spitzenleistung (PEP) in die mittlere Leistung P umgerechnet. Die so korrigierte Leistung kann in die Fernfeldformel zur Berechnung des Sicherheitsabstandes Personenschutz eingesetzt werden. 

RTTY und FM haben den Faktor $\num{1}$, so wie die meisten Modulationsverfahren.
</indepth>