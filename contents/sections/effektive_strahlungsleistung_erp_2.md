In der Klasse N haben wir bereits die *effektive Strahlungsleistung* (ERP) kennengelernt. Im Gegensatz zur EIRP bezieht sie sich nicht auf einen isotropen Strahler, sondern auf einen Halbwellendipol. Für die Berechnung ist nur die Leistung maßgeblich, die tatsächlich am Speisepunkt der Antenne ankommt. Verluste in der Speiseleitung, beispielsweise durch Kabeldämpfung, müssen daher von der Senderausgangsleistung abgezogen werden.

Die effektive Strahlungsleistung ergibt sich aus der der Antenne zugeführten Leistung und dem Antennengewinn in der betrachteten Richtung:

$P_\mathrm{ERP}=P_\mathrm{Ant}\cdot G_\mathrm{d}$

Dabei ist $G_\mathrm{d}$ der auf einen Halbwellendipol bezogene Antennengewinn als linearer Faktor.

[question:AG501]

Die Leistung am Speisepunkt der Antenne lässt sich aus der Senderausgangsleistung und der Dämpfung der Speiseleitung bestimmen. Dazu wird die Dämpfung in einen linearen Dämpfungsfaktor $D$ umgerechnet. Bei einer Dämpfung von beispielsweise $\qty{10}{\dB}$ beträgt dieser Faktor $\num{0,1}$, sodass nur noch ein Zehntel der Senderleistung an der Antenne ankommt:

$P_\mathrm{Ant}=D\cdot P_\mathrm{Sender}$

Erst diese tatsächlich zugeführte Leistung wird anschließend mit dem Antennengewinn multipliziert, um die ERP zu berechnen.

[question:AK104]

In der Klasse N haben wir die effektiven Strahlungsleistung (ERP) bereits kennen gelernt. Sie bezieht sich im gegensatz zur EIRP auf den Halbwellendipol und nicht auf den isotropen Strahler. Bei der Strahlungsleistung ist nur die Energie relevant, die tatsächlich an der Antenne ankommt. Durch Kabeldämpfung etc. kann die Leistung des Senders in der realen Welt nicht vollständig der Antenne zugeführt werden. Diese verlorene Leistung darf nicht in die Berechnung der Strahlungsleistung eingehen. Der Antennengewinn in der Vorzugsrichtung ist natürlich Teil der Rechnung. ERP ist das Produkt aus zugeführter Leistung und dem Antennengewinn.

[question:AG501]

Die Leistung am Speisepunkt der Antenne ergibt sich aus der Senderausgangsleistung und der Dämpfung der Speiseleitung. Jede Dämpfung kann in einen Dämpfungsfaktor übertragen werden. Zum Beispiel, bei $\qty{10}{\dB}$ Dämpfung ist der Faktor $\num{0,1}$.
Die Berechnung ist einfach: $P_{Ant} = D \cdot P_{Sender}$ (D steht für Dämpfungsfaktor)

[question:AK104]

Bei der nächsten Frage ist unbedingt auf die Rechenzeichen zu achten. Die Verluste werden von der Sendeleistung subtrahiert und danach mit dem Gewinnfaktor ($G_{Antenne}$) multipliziert.
Da die ERP berechnet werden soll, muss der Bezug auf einen Halbwellendipol erfolgen.

[question:AG502]

Einen Hinweis auf die richtige Lösung der nächsten Frage gibt schon die [Anlage 1 der AFUV](https://50ohm.de/a1). Dort ist als maximale Leistung für das $\qty{630}{\meter}$-Band $\qty{1}{\watt}$ ERP vorgegeben. Ein Halbwellendipol für diese Frequenz hätte eine Länge von etwa $\qty{315}{\meter}$ und ist daher für die meisten Funkamateure kaum realisierbar. In der Praxis kommen deshalb meist stark verkürzte Antennen zum Einsatz, deren Wirkungsgrad deutlich geringer ist als der eines unverkürzten Halbwellendipols. Ein Antennengewinn von $\qty{-20}{\dBd}$ ist daher durchaus plausibel. Da das verwendete Koaxialkabel nur eine geringe Länge hat, kann dessen Dämpfung in diesem Frequenzbereich vernachlässigt werden. Versuche nun die folgende Frage zu lösen. 

[question:AG503]