--- style="font-size: 0.7em;"

## Antennencharakteristik und Richtwirkung

<left>
[picture:264:a_strahlungscharakteristik_dipol_richt:Strahlungscharakteristik einer Richtantenne zu einem Dipol]
* Das *Vor-/Rück-Verhältnis* beschreibt, wie viel besser in Hauptstrahlrichtung gesendet und empfangen wird.
</left>
<right>
* Richtantennen senden und empfangen auch in Rückwärtsrichtung – ein unerwünschter Effekt.  
* Der Antennengewinn bezieht sich nur auf die Hauptstrahlrichtung (im Vergleich zu einem Dipol oder isotropen Strahler).  
</right>

---

[question:AG214]

---

[question:AG213]

---

### Vor-/Rück-Verhältnis in Dezibel

<left>
[picture:263:a_strahlungscharakteristik_richt:Strahlungscharakteristik einer Richtantenne]
</left>
<right>
* Das Vor-/Rück-Verhältnis wird häufig in Dezibel angegeben.
</right>

---

[question:AG217]

---
#### Lösungsweg
* gegeben: $P_\text{R} = \qty{0,6}{\watt}$
* gegeben: $P_\text{V} = \qty{15}{\watt}$
* gesucht: $\frac{\text{Vor}}{\text{Rück}}$

<fragment>
$\begin{split}\frac{\text{Vor}}{\text{Rück}} &= 10 \cdot \log_{10}{\left(\frac{P_\text{V}}{P_\text{R}}\right)} \unit{\dB}\\ &= 10 \cdot \log_{10}{\left(\frac{\qty{15}{\watt}}{\qty{0,6}{\watt}}\right)} \unit{\dB}\\ &= \qty{14}{\dB}\end{split}$
</fragment>

---

[question:AG215]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_D= \qty{10}{\dB}$
* gegeben: $\frac{\text{Vor}}{\text{Rück}} = \qty{20}{\dB}$
</left>
<right>
* gegeben: $P_S = \qty{100}{\watt}$
* gesucht: $P_\text{R}$
</right>

<left>
<fragment>
$\begin{split}P_\text{V} &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{\qty{10}{\dB}}}\\ &= \qty{100}{\watt} \cdot 10^{\frac{\qty{10}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{1000}{\watt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\qty{20}{\dB} &= 10 \cdot \log_{10}{\left(\frac{P_\text{V}}{P_\text{R}}\right)} \unit{\dB}\\ \Rightarrow \frac{P_\text{V}}{P_\text{R}} &= 10^{\frac{\qty{20}{\dB}}{\qty{10}{\dB}}}\\ &= 100\\ \Rightarrow P_\text{R} &= \frac{P_\text{V}}{100}\\ &= \frac{\qty{1000}{\watt}}{100}\\ &= \qty{10}{\watt}\end{split}$
</fragment>
</right>
---

[question:AG216]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_D= \qty{15}{\dB}$
* gegeben: $\frac{\text{Vor}}{\text{Rück}} = \qty{25}{\dB}$
</left>
<right>
* gegeben: $P_S = \qty{6}{\watt}$
* gesucht: $P_\text{R}$
</right>

<left>
<fragment>
$\begin{split}P_\text{V} &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{\qty{10}{\dB}}}\\ &= \qty{6}{\watt} \cdot 10^{\frac{\qty{15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{189,7}{\watt}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\qty{25}{\dB} &= 10 \cdot \log_{10}{\left(\frac{P_\text{V}}{P_\text{R}}\right)} \unit{\dB}\\ \Rightarrow \frac{P_\text{V}}{P_\text{R}} &= 10^{\frac{\qty{25}{\dB}}{\qty{10}{\dB}}}\\ &= 316,2\\ \Rightarrow P_\text{R} &= \frac{P_\text{V}}{316,2}\\ &= \frac{\qty{189,7}{\watt}}{316,2}\\ &= \qty{0,6}{\watt}\end{split}$
</fragment>
</right>

---

[question:AG218]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $U_\text{V} = \qty{300}{\micro\volt\per\meter}$
* gegeben: $U_R = \qty{20}{\micro\volt\per\meter}$
</left>
<right>
* gegeben: $U_\text{D} = \qty{128}{\micro\volt\per\meter}$
* gesucht: $g_D$, $\frac{\text{Vor}}{\text{Rück}}$
</right>

<left>
<fragment>
$\begin{split}g_D &= 20 \cdot \log_{10}{\left(\frac{U_\text{V}}{U_\text{D}}\right)} \unit{\dB}\\ &= 20 \cdot \log_{10}{\left(\frac{\qty{300}{\micro\volt\per\meter}}{\qty{128}{\micro\volt\per\meter}}\right)}\\ &= \qty{7,4}{\dB}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\frac{\text{Vor}}{\text{Rück}} &= 20 \cdot \log_{10}{\left(\frac{U_\text{V}}{U_R}\right)} \unit{\dB}\\ &= 20 \cdot \log_{10}{\left(\frac{\qty{300}{\micro\volt\per\meter}}{\qty{20}{\micro\volt\per\meter}}\right)}\\ &= \qty{23,5}{\dB}\end{split}$
</fragment>
</right>
