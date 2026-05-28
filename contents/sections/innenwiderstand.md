In der Klasse E haben wir bereits Spannungsquellen kennen gelernt. Zunächst wollen wir uns mit der Stromquelle beschäftigen, bevor wir den Innenwiderstand von Spannungs- und Stromquellen genauer betrachten.

Ähnlich wie bei der Spannungsquelle, sorgt eine Stromquelle dafür, dass diese möglichst einen konstanten Strom liefert. Abbildung [ref:a_isource_schematic] zeigt deren Ersatzschaltbild.

<margin>
[picture:1058:a_isource_schematic:Ersatzschaltbild Stromquelle $R_i$ hochohmig]
</margin>

<indepth>
Betrachtung einer Konstantstromquelle am Beispiel eines Labornetzgerätes:

[photo:298:a_Strombegrenzung:Labornetzgerät mit eingestellter Strombegrenzung auf $\qty{500}{\milli\ampere}$]

In Labornetzgeräten ist eine Strombegrenzung eingebaut, d.h. übersteigt der Laststrom eine maximale Stromstärke, wird die Klemmenspannung so abgesenkt, dass der Laststrom konstant bleibt. Dies entspricht der Funktion einer Konstantstromquelle -- Bei Kurzschluss an den Ausgangsklemmen fließt der eingestellte maximale Strom.
</indepth>

Eine ideale Konstantstromquelle liefert unabhängig von der angeschlossenen Last einen konstanten Dauerstrom. In der Theorie ist dies bei einem unendlichen Innenwiderstand möglich. In der Praxis haben Stromquellen einen sehr hohen Innenwiderstand.

<margin>
[picture:1018:a_vsource_schematic:Ersatzschaltbild Spannungsquelle]
</margin>

---

Die Abbildung [ref:a_vsource_schematic] zeigt ein Ersatzschaltbild einer Spannungsquelle. Der Innenwiderstand $R_i$ liegt in Reihe zur idealen Spannungsquelle und sollte im Ideallfall $\qty{0}{\ohm}$ betragen. In der Praxis haben Spannungsquellen einen kleinen Innenwiderstand.

[question:AB201]

Wird eine reale Spannungsquelle mit $R_L$ belastet, so sinkt die Klemmenspannung $U_k$. Grund dafür ist der vorhandene Innenwiderstand $R_i$ dieser Spannungsquelle. Durch ihn entsteht quasi ein Spannungsteiler. Da die Quellenspannung $U_q$ im Leerlauf, also ohne Belastung $U_q=U_L$ ist, nennt man diese auch Leerlaufspannung. 

Mit einem Multimeter ist der Innenwiderstand nicht messbar, man kann ihn aber rechnerisch über das Ohmsche Gesetz ermitteln (vgl. Formelsammlung):

$R_i = \frac{\Delta U}{\Delta I}$

Zur Berechnung werden zwei Belastungsfälle benötigt:
1. Leerlauf ohne Belastung: $I = \qty{0}{\ampere}$ und $U_L = U_q$
2. Belastung mit $R_L$: Wir messen $I_L$ und $U_L$

Über die Spannungsveränderung ($\Delta U = U_q~-~U_L$) an den Klemmen und die Laststromveränderung ($\Delta I = I_L~-~\qty{0}{\ampere}$), kann der Innenwiderstand nach der obigen Formel berechnet werden.

$R_i = \frac{\Delta U}{\Delta I} = \frac{U_q - U_L}{I_L-\qty{0}{\ampere}} = \frac{U_q - U_L}{I_L}$

Mit diesem Wissen können wir die folgenden Prüfungsfragen beantworten:

[question:AB205]
[question:AB206]
[question:AB207]
[question:AB208]

Wir fassen zusammen:

* Spannungsquellen sollen einen sehr niedrigen Innenwiderstand $R_i \ll R_L$ aufweisen, im Idealfall: $\qty{0}{\ohm}$, dann bleibt die Ausgangsspannung bei Belastung unverändert. Bleibt die Klemmenspannung bei Belastung konstant, dann spricht man von Spannungsanpassung.
* Stromquellen sollen einen sehr hohen Innenwiderstand $R_i \gg R_L$ aufweisen. Idealfall: $\qty{\infty}{\ohm}$, dann bleibt der Laststrom bei Änderung des Lastwiderstandes konstant, deshalb spricht man auch von Stromanpassung.

[question:AB203]
[question:AB204]

---

Soll eine Spannungsquelle die maximale Leistung an eine Last abgeben, spricht man von Leistungsanpassung. Dies ist beispielsweise auch bei einem Sender wichtig, der möglichst viel Leistung an eine Antenne übertragen soll.

Die maximale Leistungsübertragung wird erreicht, wenn

$R_i = R_L$

gilt, also Innenwiderstand und Lastwiderstand gleich groß sind.

In diesem Fall verteilt sich die Quellenspannung gleichmäßig auf Innenwiderstand und Last. Dadurch ergibt sich an der Last das maximale Produkt aus Spannung und Strom und somit die größtmögliche Leistung.

Die Abbildung [ref:a_Leistungsanpassung] zeigt die normierte Leistung an der Last in Abhängigkeit vom Verhältnis $R_L/R_i$. Das Maximum wird genau bei $R_L/R_i = 1$ erreicht, also dann, wenn Innenwiderstand und Lastwiderstand gleich groß sind. Allerdings beträgt der Wirkungsgrad bei der Leistungsanpassung nur $\qty{50}{\percent}$, da die gleiche Leistung sowohl an der Last als auch am Innenwiderstand umgesetzt wird.

<margin>
[picture:1077:a_Leistungsanpassung:Optimale Leistungsanpassung bei $R_i = R_L$, hier wird der Quotient $\frac{R_L}{R_i}=1$ und damit die maximale Leistung an der Last abgegeben. Der Plot ist logarithmisch.]
[picture:937:a_Leistungsanpassung:Optimale Ausgangsleistung bei $\qty{50}{\ohm}$ Lastwiderstand bei einem Innenwiderstand von $\qty{50}{\ohm}$. Der Plot ist nicht logarithmisch.]
</margin>

<indepth>
Wechselspannungsquellen, z.B. Sinusgeneratoren besitzen auch einen Innenwiderstand, der an der Ausgangsbuchse angeben ist.
[photo:292:Sinusgenerator 50 Ohm:Sinusgenerator mit 50 Ohm Innenwiderstand]
</indepth>

% GGF muss das woanders hin? 
<indepth>
Der in der Hochfrequenztechnik häufig verwendete Wert von $\qty{50}{\ohm}$ ist ein technischer Kompromiss zwischen maximaler Leistungsübertragung und möglichst geringen Verlusten in Leitungen.

Koaxialkabel mit einem Wellenwiderstand von etwa $\qty{30}{\ohm}$ können besonders hohe Leistungen übertragen, da der Strom im Kabel geringer verteilt wird. Kabel mit etwa $\qty{77}{\ohm}$ besitzen dagegen die geringsten Dämpfungsverluste und eignen sich besonders gut für eine verlustarme Signalübertragung.

Der heute weit verbreitete Wert von $\qty{50}{\ohm}$ liegt zwischen beiden Optima und stellt einen guten Kompromiss aus hoher Leistungsübertragung, moderaten Verlusten und praktikabler Kabelkonstruktion dar. Deshalb haben sich $\qty{50}{\ohm}$ in der Funktechnik als Standard etabliert.

Wird ein Sender, ein Kabel und eine Antenne jeweils auf $\qty{50}{\ohm}$ angepasst, dann wird die Leistung optimal übertragen und Reflexionen auf der Leitung werden minimiert.

[picture:1078:a_50ohm:50 Ohm als Kompromiss zwischen maximaler Leistungsübertragung und minimalen Verlusten in der Hochfrequenztechnik]

Jetzt weißt du auch, warum unsere Plattform 50ohm.de heißt: Wir wollen dir helfen, die Prüfungsfragen zu meistern und damit die optimale Leistung in der Prüfung zu erreichen 🤓
</indepth>

[question:AG401]
[question:AB202]