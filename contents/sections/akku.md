Neben den bekannten Bleiakkus (Pb) und Nickel-Metallhydrid-Akkus (NiMH) setzen wir in der Funktechnik, z. B. beim Portabelbetrieb, zunehmend auf Lithium-Eisen-Phosphat-Akkus (LiFePO4). Schauen wir uns dazu zunächst einen Akku und seine Aufschriften in Abbildung [ref:a_akku_lifepo4] an.

<margin>
[photo:175:a_akku_lifepo4:LiFePO4]
</margin>

<indepth>
* Kapazität: $\qty{4200}{\milli\ampere\hour}$
* Spannung: 4S1P / $\qty{13,2}{\volt}$
% * Entladung: 30C Constant / 40C Burst
% * Balance Stecker: JST-XH
% * Entlastung Stecker: $\qty{5,5}{\milli\meter}$ Kugel-Stecker

Die für uns wichtigsten Kenndaten sind die Nennspannung $\qty{13,2}{\volt}$ und die Verschaltung 4S1P. Das bedeutet, dass sich die Nennspannung von $\qty{13,2}{\volt}$ aus 4 in Serie bzw. Reihe und 1 mal parallel, also alle 4 in Serie geschalten sind. Üblicherweise besitzen LiFePO4 eine Zellnennspannung von $\qty{3,2}{\volt}$ bis $\qty{3,3}{\volt}$. Und somit ergibt sich $\qty{3,3}{\volt} \cdot 4 = \qty{13,2 }{\volt} \cdot 1 = \qty{13,2}{\volt}$.

Bei einem 4S2P sind insgesamt 8 Zellen verbaut. 4 in Serie und das 2 mal parallel. Dies würde dann eine Spannung von $\qty{13,2}{\volt}$ aber eine Kapazität von $\qty{8400}{\milli\ampere\hour}$ ergeben.

</indepth>

Bei dem Beispiel-Akku sind $\qty{4200}{\milli\ampere\hour}$ als Nennkapazität angegeben. Die Akku-Nennkapazität $Q$ wird auch als Ladung bezeichnet und in $\unit{\ampere\hour}$ oder $\unit{\milli\ampere\hour}$ angegeben.

Für unseren Beispiel-Akku entspricht dies $\qty{4,2}{\ampere\hour}$. Das würde theoretisch bedeuten, wir können unseren Akku $\qty{1}{\hour}$ lang mit $\qty{4,2}{\ampere}$ oder $\qty{2}{\hour}$ lang mit $\qty{2,1}{\ampere}$ usw. belasten.Beschrieben wird dies mit der Formel:

$t=\frac{Q}{I}$

$t=\frac{\qty{4,2}{\ampere\hour}}{\qty{4,2}{\ampere}} = \qty{1}{\hour}$

[question:AB210]

Nun wollen wir aber auch wissen, wie viel elektrische Energie in dem Akku gespeichert ist. Energie ($\unit{\watt\hour}$) ist die Ladung $Q$ ($\unit{\ampere\hour}$) des Akkus multipliziert mit der Gesamtspannung $U$ in Volt.

$\qty{1}{\watt\hour} = \qty{1}{\ampere\hour} \cdot \qty{1}{\volt}$

Für unser Beispiel berechnen wir $\qty{4,2}{\ampere\hour} \cdot \qty{13,2}{\volt} = \qty{55,44}{\watt\hour}$ als gespeicherte Energie.

[question:AB501]

%Die Entladung dieses Akkus kann mit einem konstanten Entladestrom von "30 C" erfolgen. Das bedeutet, dass der Akku mit 30 $\cdot$ Kapazität $Q$ entladen werden kann.
%
%Endladestrom: $I = 30 \cdot \qty{4200}{\milli\ampere} = \qty{126}{\ampere}$
%
%Das ist allerdings nur ein theoretisch möglicher Wert, da unser Akku somit innerhalb von $\qty{108}{\second}$ entladen wäre. Auch der Kabelquerschnitt ist dabei zu berücksichtigen.
%

Bei Reihen- bzw. Serienschaltung von Akkus, wie in Abbildung [ref:a_akku_4S1P] addieren sich die Spannungen und die Kapazität bleibt gleich. 
Bei der Parallelschaltung wie in Abbildung [ref:a_akku_4S2P] bleibt die Spannung gleich und die Kapazitäten addieren sich. 

<margin>
% TODO Bild Reihenschaltung liegt bei DG1HXJ als .tex
[photo:176:a_akku_4S1P:Reihenschaltung]
</margin>

<margin>
% TODO Bild Parallelschaltung liegt bei DG1HXJ als .tex
[photo:177:a_akku_4S2P:Parallelschaltung]
</margin>

<attention>
Beachte bei dem Einsatz von einem LiFePO4 als 4S1P verschalten, dass Spannungen zwischen $\qty{10}{\volt}$ bis $\qty{14,4}{\volt}$ anliegen können. Nicht jedes Funkgerät kann mit diesen Spannungen arbeiten. Wichtig ist auch, dass wir nur Zellen/ Akkus mit gleichen Daten zusammenschalten, da sich die Zellen gegenseitig beeinflussen und sonst beschädigt werden können. Insbesondere bei den aktuellen Lithium-Akkumulatoren ist es sinnvoll eine Überwachungseinrichtung (Balancer, Batteriemonitor) zu verbauen. Dieser sorgt u.a. für den notwendigen Ausgleich der Zellspannungen und für eine optimale Ladung.
</attention>

---


% In der Abb. [ref:a_akku_lifepo4_anschluss]
% TODO Bild Infobox Anschluss Akku liegt bei DG1HXJ als .tex
%<margin>
%[photo:178:a_akku_lifepo4_anschluss:LiFePO4 Anschlüsse]
%</margin>

Um die folgende Frage zu lösen, muss man wissen, dass die Gesamtspannung der Summe der Zellenspannungen entspricht. Die Gesamtladung entspricht hingegen der Ladung einer Zelle.

[question:AB209]

Für die nächste Frage muss zuerst die entnehmbare Ladungsmenge von $\qty{90}{\percent}$ ermittelt werden.
Die Entladezeit $t$ ergibt sich aus: $t=\frac{Q}{I}$

[question:AB211]
