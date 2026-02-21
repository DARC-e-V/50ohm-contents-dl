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

* Der Frequenzplan für das $\qty{630}{\meter}$-Band gibt eine maximale ERP von $\qty{1}{\watt}$ vor
* Ein Halbwellendipol hätte bei $\qty{630}{\meter}$ eine Länge von $\qty{315}{\meter}$ – meist nicht realisierbar, daher werden verkürzte Antennen eingesetzt
* Verkürzte Antennen haben einen geringeren Wirkungsgrad, z. B. ein Antennengewinn von $\qty{-20}{\dBd}$
* Leistungsverhältnis: $\qty{-20}{\dB}$ entspricht einem Faktor von $\num{0,01}$; Beispiel: $\qty{50}{\watt} \cdot 0,01 = \qty{0,5}{\watt}$ ERP

--- style="font-size: 0.7em;"

### Leistungsverhältnisse in der Formelsammlung

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

---
[question:AG503]
---
#### Lösungsweg
* gegeben: $P_S = \qty{50}{\watt}$
* gegeben: $a \approx \qty{0}{\dB}$
* gegeben: $g_d = \qty{-20}{\dBd}$
* gesucht: $P_{\textrm{ERP}}$

<fragment>
$\begin{split} P_{\textrm{ERP}} &= P_S \cdot 10^{\frac{g_d - a}{\qty{10}{\dB}}}\\ &= \qty{50}{\watt} \cdot 10^{\frac{\qty{-20}{\dBd} - \qty{0}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{50}{\watt} \cdot 10^{-2} = \qty{0,5}{\watt}\end{split}$
</fragment>
