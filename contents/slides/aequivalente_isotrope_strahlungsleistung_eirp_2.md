
* Bei der Berechnung nur die Energie berücksichtigen, die an der Antenne ankommt
* Verluste $a$ durch Kabel, Stecker oder andere Bauteile abziehen
* Erst dann mit dem Gewinnfaktor multiplizieren
* Es folgen diverse allgemeine Formeln für ERP und EIRP

---
### ERP

Aus Klasse N bekannt:

$P_{\mathrm{ERP}} = (P_{\mathrm{Sender}} - P_{\mathrm{Verluste}}) \cdot G_{\mathrm{Antenne}}$

<fragment>
Bei der Rechnung mit dB zu verwenden:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} - a + g_d$
</fragment>

<fragment>
Aus der Formelsammlung mit Umwandlung von dB in Leistungsfaktor:

$P_{\mathrm{ERP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a}{10\mathrm{dB}}}$
</fragment>

---
### EIRP

Umrechnung ERP zu EIRP:

$P_{\mathrm{EIRP}} = P_{\mathrm{ERP}} + 2,15 \mathrm{dB}$

<fragment>
Aus der Formelsammlung mit Umwandlung von dB in Leistungsfaktor:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + 2,15\mathrm{dB}}{10\mathrm{dB}}}$
</fragment>

<fragment>
Wenn der Gewinn in dBi angegeben ist:

$P_{\mathrm{EIRP}} = P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{10\mathrm{dB}}}$
</fragment>

---
[question:EG501]
---
[question:EG502]
---
## Ortsfeste Amateurfunkanlage

Eine ortsfeste Amateurfunkanlage ist nach § 9 BEMFV bei der BNetzA anzuzeigen, wenn eine Strahlungsleistung von 10 W EIRP überschritten wird.
---
[question:EG503]
--- style="font-size: smaller;"
### Lösungsweg

* gegeben: $P_{\mathrm{Sender}} = 250mW$
* gegeben: $g_i = 26\mathrm{dB}$
* gegeben: $a = 0$
* gesucht: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{10\mathrm{dB}}}\\ &= 250mW \cdot 10^{\frac{26\mathrm{dB}}{10\mathrm{dB}}}\\ &= 250mW \cdot 398\\ &\approx 100W \end{split}$
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

* gegeben: $P_{\mathrm{EIRP}} = 10W$
* gegeben: $g_i = 5,15\mathrm{dB}$
* gegeben: $a = 0$
* gesucht: $P_{\mathrm{Sender}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_i - a}{10\mathrm{dB}}}\\ \Rightarrow P_{\mathrm{Sender}} &= \dfrac{P_{\mathrm{EIRP}}}{10^{\frac{g_i - a}{10\mathrm{dB}}}}\\ &= \dfrac{10W}{10^{\frac{5,15\mathrm{dB}}{10\mathrm{dB}}}}\\ &\approx \frac{10W}{3,27} \approx 3W \end{split}$
</fragment>

<note>
Es führen mehrere Wege zum Ziel.  So kann auch mit Logarithmen direkt gerechnet werden.
</note>
---
[question:EG505]

<note>
Gewinn: 10dB, also auch Faktor 10
</note>
---
[question:EG507]

<note>
* 10 dB Verlust ist Faktor 10, also kommen an der Antenne 10 W ERP an
* Faktor ERP zu EIRP ist 1,64
</note>
---
[question:EG506]

<note>
* Der Gewinn des Dipols von 2,15 dB gleicht die Kabelverluste exakt aus
</note>
---

* Ist der Antennengewinn bezogen auf den Dipol angegeben, müssen wir den Gewinn des Dipols noch zusätzlich berücksichtigen, wenn nach der EIRP gefragt ist.

---
[question:EG508]
---
### Lösungsweg

* gegeben: $P_{\mathrm{Sender}} = 5W$
* gegeben: $g_d = 5\mathrm{dB}$
* gegeben: $a = 2\mathrm{dB}$
* gesucht: $P_{\mathrm{EIRP}}$

<fragment>
$\begin{split} P_{\mathrm{EIRP}} &= P_{\mathrm{Sender}} \cdot 10^{\frac{g_d - a + 2,15\mathrm{dB}}{10\mathrm{dB}}}\\ &= 5W \cdot 10^{\frac{5\mathrm{dB} - 2\mathrm{dB} + 2,15\mathrm{dB}}{10\mathrm{dB}}}\\ &= 5W \cdot 3,27\\ &\approx 16,4W \end{split}$
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