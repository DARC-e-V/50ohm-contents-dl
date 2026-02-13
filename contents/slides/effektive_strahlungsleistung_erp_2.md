## Berechnung der effektiven Strahlungsleistung (ERP)

* Nur die Energie berücksichtigen, die tatsächlich an der Antenne ankommt – Kabelverluste werden abgezogen
* ERP wird als Produkt aus der zugeführten Leistung und dem Antennengewinn (bezogen auf einen Halbwellendipol) berechnet

---
[question:AG501]
---

### Berechnungshinweise für ERP

* Verluste werden von der Sendeleistung subtrahiert, bevor der Gewinnfaktor ($G_{Antenne}$) angewendet wird
* Der Bezug auf einen Halbwellendipol muss bei der Berechnung eingehalten werden

---
[question:AG502]
---

### ERP im Amateurfunk – Praxisbeispiel

* Der Frequenzplan für das 630-m-Band gibt eine maximale ERP von 1 W vor
* Ein Halbwellendipol hätte bei 630 m eine Länge von 315 m – meist nicht realisierbar, daher werden verkürzte Antennen eingesetzt
* Verkürzte Antennen haben einen geringeren Wirkungsgrad, z. B. ein Antennengewinn von -20 dBd
* Leistungsverhältnis: -20 dB entspricht einem Faktor von 0,01; Beispiel: 50 W · 0,01 = 0,5 W ERP

--- style="font-size: 0.7em;"

### Leistungsverhältnisse in der Formelsammlung

Diese Tabelle ist in der Formelsammlung enthalten und steht während der Prüfung zur Verfügung.

| r:   | r: Leistungsverhältnis | r: Spannungsverhältnis |
| -20 dB | 0,01 | 0,1 |
| -10 dB | 0,1 | 0,32 |
| -6 dB | 0,25 | 0,5 |
| -3 dB | 0,5 | 0,71 |
| -1 dB | 0,79 | 0,89 |
| 0 dB | 1 | 1 |
| 1 dB | 1,26 | 1,12 |
| 3 dB | 2 | 1,41 | 
| 6 dB | 4 | 2 |
| 10 dB | 10  | 3,16 |
| 20 dB | 100 | 10 |
[table:Pegel_Verhältnis:Leistungs- und Spannungsverhältnisse für wichtige Dämpfungs- und Verstärkungswerte]

---
[question:AG503]
---
#### Lösungsweg
* gegeben: $P_S = 50W$
* gegeben: $a \approx 0W$
* gegeben: $g_d = -20dBd$
* gesucht: $P_{\textrm{ERP}}$

<fragment>
$\begin{split} P_{\textrm{ERP}} &= P_S \cdot 10^{\frac{g_d - a}{10dB}}\\ &= 50W \cdot 10^{\frac{-20dBd - 0W}{10dB}}\\ &= 50W \cdot 10^{-2} = 0,5W\end{split}$
</fragment>
