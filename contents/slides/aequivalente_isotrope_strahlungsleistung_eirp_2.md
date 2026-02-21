
* Bei der Berechnung nur die Energie berücksichtigen, die an der Antenne ankommt
* Verluste $a$ durch Kabel, Stecker oder andere Bauteile abziehen
* Erst dann mit dem Gewinnfaktor multiplizieren
* Es folgen diverse allgemeine Formeln für ERP und EIRP

---
### ERP

Aus Klasse N bekannt:

$P_{\mathrm{ERP}} = (P_{\mathrm{Sender}} - P_{\mathrm{Verluste}}) \cdot G_{\mathrm{Antenne}}$

<fragment>
Bei der Rechnung mit $\unit{\dB}$ zu verwenden:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} - a + g_d$
</fragment>

<fragment>
Aus der Formelsammlung mit Umwandlung von $\unit{\dB}$ in Leistungsfaktor:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a}{\qty{10}{\dB}}}$
</fragment>

---
### EIRP

Umrechnung ERP zu EIRP:

$P_{\mathrm{EIRP}} = P_{\mathrm{ERP}} + \qty{2,15}{\dB}$

<fragment>
Aus der Formelsammlung mit Umwandlung von $\unit{\dB}$ in Leistungsfaktor:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + \qty{2,15}{\dB}}{\qty{10}{\dB}}}$
</fragment>

<fragment>
Wenn der Gewinn in $\unit{\dBi}$ angegeben ist:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}$
</fragment>

---
[question:EG501]
---
[question:EG502]
---
## Ortsfeste Amateurfunkanlage

Eine ortsfeste Amateurfunkanlage ist nach § 9 BEMFV bei der BNetzA anzuzeigen, wenn eine Strahlungsleistung von $\qty{10}{\watt}$ EIRP überschritten wird.
---
[question:EG503]
--- style="font-size: smaller;"
### Lösungsweg

* gegeben: $P_{\mathrm{Sender}} = \qty{250}{\milli\watt}$
* gegeben: $g_i = \qty{26}{\dBi}$
* gegeben: $a = \qty{0}{\dB}$
* gesucht: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}\\ &= \qty{250}{\milli\watt} \cdot 10^{\frac{\qty{26}{\dBi}}{\qty{10}{\dB}}}\\ &= \qty{250}{\milli\watt} \cdot 398\\ &\approx \qty{100}{\watt} \end{split}$
</fragment>

---
[question:EG504]

<note>
* Lösungsweg gleich wie vorher
</note>
---
[question:EG511]
--- style="font-size: smaller;"
### Lösungsweg

* gegeben: $P_{\mathrm{EIRP}} = \qty{10}{\watt}$
* gegeben: $g_i = \qty{5,15}{\dBi}$
* gegeben: $a = \qty{0}{\dB}$
* gesucht: $P_{\mathrm{Sender}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{\qty{10}{\dB}}}\\ \Rightarrow P_{\mathrm{Sender}} &= \dfrac{P_{\mathrm{EIRP}}}{10^{\frac{g_i - a}{\qty{10}{\dB}}}}\\ &= \dfrac{\qty{10}{\watt}}{10^{\frac{\qty{5,15}{\dBi}}{\qty{10}{\dB}}}}\\ &\approx \frac{\qty{10}{\watt}}{3,27} \approx \qty{3}{\watt} \end{split}$
</fragment>

<note>
Es führen mehrere Wege zum Ziel.  So kann auch mit Logarithmen direkt gerechnet werden.
</note>
---
[question:EG505]

<note>
Gewinn: $\qty{10}{\dB}$, also auch Faktor $\num{10}$
</note>
---
[question:EG507]

<note>
* $\qty{10}{\dB}$ Verlust ist Faktor $\num{10}$, also kommen an der Antenne $\qty{10}{\watt}$ ERP an
* Faktor ERP zu EIRP ist $\num{1,64}$
</note>
---
[question:EG506]

<note>
* Der Gewinn des Dipols von $\qty{2,15}{\dBi}$ gleicht die Kabelverluste exakt aus
</note>
---

* Ist der Antennengewinn bezogen auf den Dipol angegeben, müssen wir den Gewinn des Dipols noch zusätzlich berücksichtigen, wenn nach der EIRP gefragt ist.

---
[question:EG508]
---
### Lösungsweg

* gegeben: $P_{\mathrm{Sender}} = \qty{5}{\watt}$
* gegeben: $g_d = \qty{5}{\dBd}$
* gegeben: $a = \qty{2}{\dB}$
* gesucht: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{5}{\watt} \cdot 10^{\frac{\qty{5}{\dBd} - \qty{2}{\dB} + \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{5}{\watt} \cdot 3,27\\ &\approx \qty{16,4}{\watt} \end{split}$
</fragment>

---
[question:EG509]

<note>
Lösungsweg gleich wie vorher
</note>
---
[question:EG510]

<note>
Lösungsweg gleich wie vorher
</note>