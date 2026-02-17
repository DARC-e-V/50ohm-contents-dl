%Bei der Berechnung der effektiven Strahlungsleistung (ERP) ist nur die Energie zu berücksichtigen, die auch tatsächlich der Antenne zugeführt wird, d. h. möglicherweise vorhandene Kabelverluste können abgezogen werden, bevor mit dem Gewinnfaktor multipliziert wird.

Die effektiven Strahlungsleistung (ERP) einer Antenne bezieht sich auf den Halbwellendipol. Bei der Strahlungsleistung ist nur die Energie relevant, die tatsächlich an der Antenne ankommt. Durch Kabeldämpfung etc. kann die Leistung des Senders in der realen Welt nicht vollständig der Antenne zugeführt werden. Diese verlorene Leistung darf nicht in die Berechnung der Stahlungsleistung eingehen. Der Antennengewinn in der Vorzugsrichtung ist natürlich Teil der Rechnung. ERP ist das Produkt aus zugeführter Leistung und dem Antennengewinn.

[question:AG501]

Bei der nächsten Frage ist unbedingt auf die Rechenzeichen zu achten. Die Verluste werden von der Sendeleistung subtrahiert und danach mit dem Gewinnfaktor ($G_{Antenne}$) multipliziert.
Da die ERP berechnet werden soll, muss der Bezug auf einen Halbwellendipol erfolgen.

[question:AG502]

---

Einen Hinweis auf die richtige Lösung gibt schon der Frequenzplan für den Amateurfunkdienst. Dort ist als maximale Leistung für das $\qty{630}{\meter}$-Band $\qty{1}{\watt}$ ERP vorgegeben.

Ein Halbwellendipol hätte eine Länge von $\qty{315}{\meter}$. Das ist für die meisten Funkamateure nicht realisierbar. Zwangsläufig kommen stark verkürzte Antenne zum Einsatz. Verkürzte Antenne haben leider einen schlechteren Wirkungsgrad als ein Halbwellendipol in voller Länge. Ein "Antennengewinn" von $\qty{-20}{\dBd}$ ist also nicht überraschend. Da das Koaxialkabel kurz ist kann dessen Dämpfung in diesem Frequenzbereich vernachlässigt werden.

Zu Lösung der Frage AG503 kann auf die Tabelle mit den Leistungsverhältnissen in der Formelsammlung zurückgreifen. Dort ist für $\qty{-20}{\dB}$ der Faktor $\num{0,01}$ angegeben.

$\qty{50}{\watt}\cdot 0,01 = \qty{0,5}{\watt}$

Die richtige Lösung ist $\qty{0,5}{\watt}$.

%Ein Sender für das $\qty{630}{\meter}$-Band mit $\qty{50}{\watt}$ Ausgangsleistung ist mittels eines kurzen Koaxialkabels an eine Antenne mit $\qty{20}{\dBd}$ Verlust angeschlossen. Welche ERP wird von der Antenne abgestrahlt?

[question:AG503]

<tip>
 Diese Tabelle ist in der Formelsammlung enthalten und steht während der Prüfung zur Verfügung.
  
| r:   | r: Leistungsverhältnis | r: Spannungsverhältnis |
| $\qty{-20}{\dB}$ | $\num{0,01}$ | $\num{0,1}$ |
| $\qty{-10}{\dB}$ | $\num{0,1}$ | $\num{0,32}$ |
| $\qty{-6}{\dB}$ | $\num{0,25}$ | $\num{0,5}$ |
| $\qty{-3}{\dB}$ | $\num{0,5}$ | $\num{0,71}$ |
| $\qty{-1}{\dB}$ | $\num{0,79}$ | $\num{0,89}$ |
| $\qty{0}{\dB}$ | $\num{1}$ | $\num{1}$ |
| $\qty{1}{\dB}$ | $\num{1,26}$ | $\num{1,12}$ |
| $\qty{3}{\dB}$ | $\num{2}$ | $\num{1,41}$ |
| $\qty{6}{\dB}$ | $\num{4}$ | $\num{2}$ |
| $\qty{10}{\dB}$ | $\num{10}$  | $\num{3,16}$ |
| $\qty{20}{\dB}$ | $\num{100}$ | $\num{10}$ |
[table:Pegel_Verhältnis:Leistungs- und Spannungsverhältnisse für wichtige Dämpfungs- und Verstärkungswerte]

</tip>