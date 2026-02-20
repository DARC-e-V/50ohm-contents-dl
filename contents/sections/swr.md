Wie wir zuvor gelernt haben, verwenden Amateurfunkgeräte und im Amateurfunk gebräuchliche Übertragungsleitungen meist einen Wellenwiderstand von $\qty{50}{\ohm}$. Wir haben auch gelernt, dass es an Verbindungsstellen von Übertragungsleitungen zu unerwünschten Reflexionen kommt, wenn der Wellenwiderstand nicht übereinstimmt.

Auch Antennen haben eine dem Wellenwiderstand ähnliche Eigenschaft, die von der genauen Anordnung der Antennenelemente abhängt. Diese Eigenschaft wird als Speise- oder Fußpunktwiderstand bezeichnet. Wie bei der Verbindung von zwei Übertragungsleitungen mit unterschiedlichem Wellenwiderstand gilt auch hier: Wenn der Speisewiderstand der Antennen nicht zum Wellenwiderstand der Zuleitung passt, dann kommt es zu unerwünschten Reflexionen. Ein Teil der Sendeleistung wird zum Funkgerät zurück reflektiert und kann nicht von der Antenne abgestrahlt werden.

Wenn hingegen der Speisewiderstand der Antenne und der Wellenwiderstand der Speiseleitung übereinstimmen und somit eine optimale Übertragung der Sendeleistung in die Antenne gewährleistet ist, spricht man davon, dass *Anpassung* vorliegt.

<margin>
[photo:144:swr_meter:Ein einfaches SWR-Meter zum Bestimmen des Stehwellenverhältnisses]
</margin>

Wie gut die Antennenanpassung ist, lässt sich messen. Vereinfacht gesagt wird dafür ermittelt, wieviel Sendeleistung von der Antenne reflektiert wird. Der vom Messgerät angezeigte Messwert nennt sich *Stehwellenverhältnis*. Meist wird die vom englischen Begriff "standing wave ratio" abgeleitete Abkürzung SWR verwendet. Zur Bestimmung des SWR benutzt man ein *Stehwellenmessgerät*, kurz *SWR-Meter* genannt.

% TODO: Editionsspezifisch machen
<indepth>
Ein SWR-Meter misst gleichzeitig die vorlaufende Sendeleistung, die der Sender zur Antenne schickt, und die rücklaufende Leistung, die reflektiert wurde. Dies lässt sich gut am SWR-Meter in Abbildung [ref:swr_meter_kreuzzeiger] erkennen, das vor- und rücklaufende Leistung getrennt anzeigt. Das SWR gibt allerdings nicht direkt das Verhältnis dieser beiden Messwerte an, sondern wird etwas komplizierter als $\text{SWR} = \frac {\sqrt{P_\text{V}}+\sqrt{P_\text{R}}} { \sqrt{P_\text{V}}-\sqrt{P_\text{R}}}$ ermittelt, wobei $P_\text{V}$ die vorlaufende und $P_\text{R}$ die rücklaufende Leistung ist. Für die Prüfung der Klasse N muss man diese Formel nicht kennen.
</indepth>

<margin>
[photo:143:swr_meter_kreuzzeiger:SWR-Meter mit Kreuzzeiger, linker Zeiger für die vorlaufende und rechter Zeiger für die rücklaufende Leistung; um das SWR abzulesen, wird der grünen Linie am Schnittpunkt beider Zeiger nach unten gefolgt]
</margin>

[question:NI201]

---

<margin>
[photo:67:n_swr_display:Display eines Transceivers]
</margin>

Moderne Transceiver haben bereits ein SWR-Meter eingebaut. Die Anzeige ist meistens im Display zu finden, siehe [ref:n_swr_display].

<attention>
SWR-Meter und S-Meter klingen ähnlich, sind aber verschieden: Das SWR-Meter misst das Stehwellenverhältnis beim Senden und das S-Meter misst die Signalstärke beim Empfang.
</attention>

% TODO Big Picture: Im Bild Trx_Display "SWR" kennzeichnen
[question:NF101] 

---

Wenn im Transceiver kein SWR-Meter eingebaut ist, kann man auch ein externes SWR-Meter verwenden. Es wird dazu wie in Abbildung [ref:n_trx_kabel_swr_antenne] zwischen Funkgerät und Antenne angeschlossen. Man sagt auch: "Das SWR-Meter wird zwischen Transceiver und Antenne eingeschleift".

[question:NI202]

Ist eine Antenne perfekt an die Zuleitung (z. B. das Koaxialkabel) angepasst, so zeigt das SWR-Meter einen Wert von $\num{1}$ an. Dies ist der beste erreichbare Wert. Dann wird die gesamte Leistung von der Antenne aufgenommen. Es wird keine Leistung zurück in den Sender reflektiert.

<margin>
[picture:670:n_trx_kabel_swr_antenne:Prinzipbild SWR-Meter zwischen Transceiver  und Antenne]
</margin>

[question:NG301]
[question:NI203]

---

Ist am Transceiver gar keine Antenne angeschlossen oder ist die Übertragungsleitung entweder unterbrochen oder kurzgeschlossen, so ist der SWR-Wert nahezu unendlich ($\infty$). Ein offenes bzw. kurzgeschlossenes Kabel reflektiert nämlich die Sendeleistung komplett. Das kann im schlimmsten Fall sogar den Sender im Funkgerät zerstören.

<indepth>
Neben den beiden *SWR*-Werten $\num{1}$ und unendlich ($\infty$) sind noch die Werte $\num{2}$ und $\num{3}$ rechts markant. Bei einem SWR-Wert von $\num{2}$ werden $\qty{11}{\percent}$, bei einem SWR-Wert von $\num{3}$ werden $\qty{25}{\percent}$ der Sendeleistung zurück in den Sender reflektiert. Bei modernen Transceivern wird einer Beschädigung des Senders dadurch vorgebeugt, dass die Sendeleistung im Funkgerät automatisch reduziert wird.
</indepth>

Ein sehr schlechtes SWR, beispielsweise nahe unendlich, kann man auch erhalten, wenn eine sehr schlechte Anpassung der Antennen vorliegt oder die Übertragungsleitung beschädigt ist.

[question:NG302]
[question:NG303]

Ist an einem Funkgerät mit SWR-Meter eine Antenne mit schlechter Anpassung über ein langes Koaxialkabel angeschlossen, so kann der angezeigte SWR-Wert deutlich besser sein als es aufgrund der schlechten Anpassung zu erwarten wäre. Ursache hierfür ist eine hohe Kabeldämpfung, die nicht nur das zur Antenne laufende, sondern auch das reflektierte Signal verringert.

[question:NG208]
