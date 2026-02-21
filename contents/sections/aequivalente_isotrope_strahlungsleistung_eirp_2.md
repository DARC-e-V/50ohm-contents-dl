In der Klasse N haben wir bereits den isotropen Strahler (vgl. Abbildung [ref:e_Kugelstrahler]) kennengelernt. Der isotrope Strahler ist keine reale Antenne, er ist ein physikalisches Modell für einen Strahler, der die Energie in alle Richtungen des Raumes gleichmäßig abstrahlt. 

Die Äquivalente Isotrope Strahlungsleistung (EIRP) einer realen Antenne bezieht sich auf den isotropen Strahler. Mit anderen Worten, die Strahlungsleistung  einer realen Antenne wird mit der Strahlungsleistung des isotropen Strahlers verglichen. Für die abgestrahlte Leistung ist nur die Energie relevant, die tatsächlich an der Antenne ankommt. Durch Kabeldämpfung etc. kann die Leistung des Senders in der realen Welt nicht vollständig der Antenne zugeführt werden. Diese verlorene Leistung darf nicht in die Berechnung der Stahlungsleistung eingehen. Der Antennengewinn in der Vorzugsrichtung ist natürlich Teil der Rechnung. In Formeln bedeutet das:

$P_\text{EIRP} = (P_\text{Sender} - P_\text{Verluste}) \cdot G_\text{Antenne}$

Wobei $G$ hier den Antennengewinn darstellt. EIRP also ist das Produkt aus der Leistung, die unmittelbar der Antenne zugeführt wird, und ihrem Gewinn in einer Richtung, bezogen auf den isotropen Strahler.

<margin>
[picture:751:e_Kugelstrahler:Isotroper Strahler in der Mitte einer Kugel, der an allen Stellen der Kugeloberfläche die gleiche Strahlungsleistung erzeugt]
</margin>

<tip>
Vor der Prüfung sollte man sich gut mit seinem Taschenrechner vertraut machen. Die Berechnungen und die Formeln bei den verschiedenen Fragen sollten immer wieder geübt werden, damit man das Gerät und die Rechenschritte in der Prüfung sicher beherrscht.
</tip>

[question:EG501]

Bei der nächsten Frage ist unbedingt auf die Rechenzeichen zu achten. Die Verluste werden von der Sendeleistung *subtrahiert* und danach mit dem Gewinnfaktor ($G_{Antenne}$) *multipliziert*. Da die EIRP berechnet werden soll, muss der Bezug auf den isotropen Strahler erfolgen.

[question:EG502]

---

Im Kapitel zu Dezibel haben wir gelernt, dass es sinnvoll ist, mit dB-Werten zu rechnen, da sich viele Berechnungen dadurch deutlich vereinfachen. Verstärkungen und Dämpfungen lassen sich in Dezibel einfach addieren beziehungsweise subtrahieren. Abbildung [ref:e_verstaerkung_daempfung] zeigt eine Funkanlage mit mehreren Verstärkungs- und Dämpfungsgliedern. Die Gesamtverstärkung dieser Anlage ergibt sich durch Addition der einzelnen Beiträge zu $\qty{-2}{\dB} + \qty{6}{\dB} - \qty{3}{\dB} + \qty{2}{\dB} = \qty{3}{\dB}$, was einem Leistungsfaktor von $\num{2}$ entspricht.

<margin>
[picture:439:e_verstaerkung_daempfung:Verstärkungen und Dämpfungen in einer Funkanlage]
</margin>

---

Die folgenden Fragen erfordern die Berechnung der EIRP. Hierfür kann entweder direkt eine Formel verwendet werden, oder die Aufgaben lassen sich – mit etwas Übung – vollständig im Kopf lösen. Im Folgenden möchten wir daher meist beide Vorgehensweisen aufzeigen.

Die Formel zur Berechnung der EIRP ergibt sich aus der Formelsammlung und lautet:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}$

<indepth>
Man erhält die Formel für $P_\text{EIRP}$, indem man die Gewinnformel aus der Formelsammlung entsprechend umstellt:
  
$g = 10 \cdot \log_{10}\left(\frac{P_2}{P_1}\right) \unit{\dB}$
  
Da zusätzlich eine Dämpfung $a$ berücksichtigt werden muss, wird diese vom Antennengewinn abgezogen. Für $P_1$ setzen wir die Senderleistung $P_\text{Sender}$ ein, da sie die Eingangsleistung darstellt, und für $P_2$ entsprechend $P_\text{EIRP}$, da dies die resultierende Ausgangsleistung ist.

$g-a = 10 \cdot \log_{10}\left(\frac{P_\text{EIRP}}{P_{Sender}}\right) \unit{\dB} \quad\quad\quad | : \qty{10}{\dB}$
  
Wir teilen auf beiden Seiten durch $\qty{10}{\dB}$:
  
$\frac{g-a}{\qty{10}{\dB}} = \log_{10}\left(\frac{P_\text{EIRP}}{P_{Sender}}\right) \quad\quad\quad | 10^x$
  
Danach wenden wir auf beiden Seiten $10^x$ an um den Logarithmus aufzulösen:
  
$10^{\frac{g-a}{\qty{10}{\dB}}} = \frac{P_\text{EIRP}}{P_{Sender}} \quad\quad\quad | \cdot P_{Sender}$
  
Durch Multiplikation von P_{Sender} ergibt sich die benötigte Formel:
  
$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}$
</indepth>

Dabei ist $g_i$ der Antennengewinn bezogen auf den isotropen Strahler, während $a$ die Dämpfung durch Kabel und Anpassgeräte beschreibt.

[question:EG503]

Der erste Rechenweg nutz die oben angesprochene Formel. Da es keine Leistungsverluste gibt ist die Dämpfung $a=0$ und die Formel vereinfacht sich zu: 

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}}= \qty{250}{\milli\watt} \cdot 10^{\frac{\qty{26}{dBi}}{\qty{10}{\dB}}}= \qty{250}{\milli\watt} \cdot 398 \approx \qty{100}{\watt}$

---

Der zweite mögliche Rechenweg nutzt die Tatsache, dass man dB-Werte "zerlegen" kann. In der Frage beträgt der Antennengewinn $g = \qty{26}{\dBi}$. In der Formelsammlung findet sich in Tabelle [ref:e_dezibel_leistungsfaktoren] eine Übersicht über Leistungsfaktoren für wichtige dB-Werte. Für $\qty{26}{\dB}$ gibt es dort keinen direkten Eintrag. Da sich Pegel in Dezibel jedoch addieren lassen, kann man den Wert sinnvoll aufteilen:

$\qty{26}{\dBi} = \qty{20}{\dBi} + \qty{6}{\dB}$

<margin>
| c:dB | c:≈ Leistungsfaktor |
| $\num{0}$ | $\num{1}$ |
| $\num{1,5}$ | $\sqrt{2} = 1,41$ |
| $\num{2,15}$ | $\num{1,64}$ |
| $\num{3}$ | $\num{2}$ |
| $\num{5}$ | $\sqrt{10} = 3,16$ |
| $\num{6}$ | $\num{4}$ |
| $\num{10}$ | $\num{10}$ |
| $\num{20}$ | $\num{100}$ |
[table:e_dezibel_leistungsfaktoren:Wichtige Leistungsfaktoren in dB]
</margin>

Für $\qty{20}{\dB}$ ist in der Tabelle ein Leistungsfaktor von $\num{100}$ angegeben, für $\qty{6}{\dB}$ ein Faktor von $\num{4}$. Damit lässt sich die äquivalente isotrope Strahlungsleistung sehr einfach berechnen:

$P_\text{EIRP} = \qty{250}{\milli\watt} \cdot 100 \cdot 4 = \qty{100}{\watt}$

Die richtige Antwort ist also $\qty{100}{\watt}$ EIRP.

Bei der nächsten Frage können wir genauso vorgehen wie bei der vorhergehenden Frage. 

[question:EG504]

---

Für viele Funkamateure ist es schwierig den notwendigen Sicherheitsabstand bei einer Sendeleistung von z.B. $\qty{100}{\watt}$ einzuhalten. Der QRP-Betrieb ist in diesen Fällen eine Lösung. Bleibt man mit der Strahlungsleistung unter der $\qty{10}{\watt}$-EIRP-Grenze, kann die Anzeige einer ortsfesten Amateurfunkanlage nach § 9 BEMFV entfallen. Auch bei einem nicht-QRP-Gerät kann man die Ausgangsleistung auf einen bestimmten Wert reduzieren, wie in Abbildung [ref:e_ausgangsleistung_ic] dargestellt.

<margin>
[photo:229:e_ausgangsleistung_ic:Bei vielen Transeiver lässt sich die Ausgangsleistung stufenlos, oder wie hier beim IC-705 in kleinen Schritten einstellen.]
</margin>

[question:EG511]

Die in dieser Frage angegebene Vertikalantenne hat einen Gewinn von $g=\qty{5,15}{\dBi}$, die Kabelverluste werden vernachlässigt d.h. $a = 0$. Hätte die Antenne keinen Gewinn ($\qty{0}{\dBi}$) müsste die Sendeleistung einfach auf maximal $\qty{10}{\watt}$ beschränkt werden. Die Strahlungsleistung wäre dann nur $\qty{10}{\watt}$ EIRP. Da aber ein Antennengewinn von $\qty{5,15}{\dBi}$ vorhanden ist, muss die Sendeleistung entsprechend abgesenkt werden. Die Sendeleistung muss mindesten $\qty{5,15}{\dB}$ geringer als $\qty{10}{\watt}$ sein.

Auch hier gibt es wieder zwei mögliche Rechenwege. Beginnen wir mit dem Weg über die bekannte Formel. In dieser Aufgabe ist jedoch nicht die Strahlungsleistung $P_\text{EIRP}$ gesucht, sondern die Sendeleistung $P_\text{Sender}$. Daher müssen wir die Formel entsprechend umstellen:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a}{\qty{10}{\dB}}} \quad\quad\quad | : 10^{\frac{g_i-a}{\qty{10}{\dB}}}$

So ergibt sich:

$ P_\text{Sender} = \frac{P_\text{EIRP}}{10^{\frac{g_i-a}{\qty{10}{\dB}}}} $

Wir setzen die Werte ein:

$ P_\text{Sender} = \frac{\qty{10}{\watt}}{10^{\frac{\qty{5,15}{\dBi}}{\qty{10}{\dB}}}} = \frac{\qty{10}{\watt}}{3,27} \approx \qty{3,05}{\watt} $

Die Berechnung mit dem Taschenrechner ergibt $\qty{3,05}{\watt}$. Mit einer Begrenzung auf $\qty{3}{\watt}$ hält man den Grenzwert von kleiner $\qty{10}{\watt}$ EIRP ein.

Der Zweite Rechenweg geht wieder über die Zerlegung der dB-Werte. Schaut man sich den Wert $g=\qty{5,15}{\dBi}$ an so erkennt man, dass man diesen Wert in 

$\qty{5,15}{\dBi} = \qty{3}{\dBi} + \qty{2,15}{\dB}$

zerlegen kann. In der Tabelle [ref:e_dezibel_leistungsfaktoren] findet man den Faktor für $\qty{2,15}{\dB}$ als $\num{1,64}$. Somit ergibt sich für die maximale Sendeleistung:

$P_{Sender} = \frac{\qty{10}{\watt}}{2\cdot 1,64} = \frac{\qty{10}{\watt}}{3,28} \approx \qty{3}{\watt}$

Wie zu erwarten kommen wir hier zum gleichen Ergebnis. Mit $\qty{3}{\watt}$ ist man auf der sicheren Seite.

Die nächste Frage könnte man wieder mit der Formelsammlung lösen, in dem man für $a=\qty{1}{\dB}$ einsetzt, aber es geht ganz einfach im Kopf. 

[question:EG505]

Wie ganz am Anfang des Abschnitts beschrieben, wird für die Strahlungsleistung EIRP der Antennengewinn ($\qty{11}{\dBi}$) und die Leistung berücksichtigt, die tatsächlich an der Antenne ankommt. Die Sendeleistung wird durch das Kabel um $\qty{1}{\dB}$ gedämpft, das gesamte Antennensystem hat real einen Gewinn von $\qty{10}{\dBi}$. In unserer Tabelle [ref:e_dezibel_leistungsfaktoren] in der Formelsammlung wird für $\qty{10}{\dB}$ der Faktor $\num{10}$ angegeben. Aus der Sendeleistung von $\qty{100}{\watt}$ wird eine Strahlungsleistung von $\qty{1000}{\watt}$.

Für die nächste Frage muss man darauf achten, dass eine Dipol-Antenne verwendet wird. Auch sie kann ganz einfach im Kopf gerechnet werden.

[question:EG506]

Der Gewinn einer Dipol-Antenne gegenüber dem Kugelstrahler beträgt $\qty{2,15}{\dB}$. Dies entspricht dem Faktor von $\num{1,64}$. Dies steht auch in der Formelsammlung:

$P_{EIRP} = P_{ERP} + \qty{2,15}{\dB}$

bzw. als Faktor:

$P_{EIRP} = P_{ERP}  \cdot 1,64$

Wobei $P_{ERP}$ die Strahlungsleistung bezogen auf den Dipol darstellt. 

Der Gewinn des Dipols beträgt $\qty{2,15}{\dBi}$, das entspricht hier exakt der Kabeldämpfung in der Frage. Beiden gleichen sich damit aus. Die Dipolantenne strahlt $\qty{75}{\watt}$ EIRP ab.

In der nächsten Frage ist auch wieder ein Dipol als Antenne vorgegeben. 

[question:EG507]

Gesucht ist die äquivalente isotrope Strahlungsleistung $P_\text{EIRP}$. Zunächst muss die Kabeldämpfung berücksichtigt werden. Eine Dämpfung von $\qty{10}{\dB}$ entspricht einem Leistungsverhältnis von $\num{0,1}$. Mit diesem Dämpfungsfaktor sowie dem Antennengewinnfaktor des Dipols von $\num{1,64}$ lässt sich die Strahlungsleistung anschließend berechnen.

$P_\text{EIRP} = \qty{100}{\watt} \cdot 0,1 \cdot 1,64 = \qty{16,4}{\watt}$


Für die nächste Frage findet sich in der Formelsammlung auch direkt eine Anwendbare Formel. Da wir eine Richtantenne haben deren Gewinn auf den Dipol angegeben ist (ERP) muss für die Berechung von $P_{EIRP}$  noch $\qty{2,15}{\dB}$ addiert werden:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a+\qty{2,15}{\dB}}{\qty{10}{\dB}}}$

[question:EG508]

---

Durch Einsetzen in die Formel kann man die Frage schnell lösen. Es geht aber auch hier im Kopf. Rechnen wir den Gesamtgewinn des Systems aus und zerlegen das wieder entsprechend:

$\qty{-2}{\dB} + \qty{5}{\dB} + \qty{2,15}{\dB} = \qty{3}{\dB} + \qty{2,15}{\dB}$ 

Nun können wir die Faktoren wieder aus der Tabelle ablesen:

$P_\text{EIRP} = \qty{5}{\watt} \cdot 2 \cdot 1,64 = \qty{16,4}{\watt}$

Auch die nächste Frage kann genauso gelöst werden. Man muss nur darauf achten, dass der Gewinn bezogen auf den Dipol gegeben ist. 

[question:EG509]

Wir rechnen wieder den Gesamtgewinn aus und zerlegen:

$\qty{-1}{\dB} + \qty{11}{\dB} + \qty{2,15}{\dB} = \qty{10}{\dB} + \qty{2,15}{\dB}$ 

Nun können wir die Faktoren wieder aus der Tabelle ablesen:

$P_\text{EIRP} = \qty{0,6}{\watt} \cdot 10 \cdot 1,64 = \qty{9,8}{\watt}$

In der nächsten Frage ist eine Antenne mit einem Gewinn von $\qty{0}{\dB}$ auf den Dipol bezogen angegeben. Das bedeutet nichts anderes als, dass es sich bei dieser Antenne um einen Dipol handelt. 

[question:EG510]

Hier kann wieder die Folmel aus der Formelsammlung verwendet werden:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a+\qty{2,15}{\dB}}{\qty{10}{\dB}}} = \qty{8,5}{\watt} \cdot 10^{\frac{\qty{0}{\dB}-\qty{1,5}{\dB}+\qty{2,15}{\dB}}{\qty{10}{\dB}}} = \qty{9,9}{\watt}$

Im Kopf kann man es auch überschlagen: Rechnet man wieder den Gesamtgewinn des Systems aus, so beträgt dieser nur $\qty{0,65}{\dB}$, also nicht einmal $\qty{1}{\dB}$. $\qty{1}{\dB}$ entspricht, laut unserer Tabelle [ref:e_dezibel_leistungsfaktoren], einem Faktor von $\num{1,26}$. Der Zielwert muss also zwischen $\qty{8,5}{\watt}$ und $\qty{10,71}{\watt}$ liegen. Nur die $\qty{9,9}{\watt}$ kommen also in Frage.