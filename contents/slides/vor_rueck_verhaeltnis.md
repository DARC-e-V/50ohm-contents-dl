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
* gegeben: $P_R = 0,6W$
* gegeben: $P_V = 15W$
* gesucht: $\frac{Vor}{Rück}$

<fragment>
$\begin{split}\frac{Vor}{Rück} &= 10 \cdot \log_{10}{(\frac{P_V}{P_R})} dB\\ &= 10 \cdot \log_{10}{(\frac{15W}{0,6W})} dB\\ &= 14dB\end{split}$
</fragment>

---

[question:AG215]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_D= 10dB$
* gegeben: $\frac{Vor}{Rück} = 20dB$
</left>
<right>
* gegeben: $P_S = 100W$
* gesucht: $P_R$
</right>

<left>
<fragment>
$\begin{split}P_V &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{10dB}}\\ &= 100W \cdot 10^{\frac{10dB}{10dB}}\\ &= 1000W\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}20dB &= 10 \cdot \log_{10}{(\frac{P_V}{P_R})} dB\\ \Rightarrow \frac{P_V}{P_R} &= 10^{\frac{20dB}{10}}\\ &= 100\\ \Rightarrow P_R &= \frac{P_V}{100}\\ &= \frac{1000W}{100}\\ &= 10W\end{split}$
</fragment>
</right>
---

[question:AG216]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_D= 15dB$
* gegeben: $\frac{Vor}{Rück} = 25dB$
</left>
<right>
* gegeben: $P_S = 6W$
* gesucht: $P_R$
</right>

<left>
<fragment>
$\begin{split}P_V &= P_{ERP}\\ &= P_S \cdot 10^{\frac{g_d}{10dB}}\\ &= 6W \cdot 10^{\frac{15dB}{10dB}}\\ &= 189,7W\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}25dB &= 10 \cdot \log_{10}{(\frac{P_V}{P_R})} dB\\ \Rightarrow \frac{P_V}{P_R} &= 10^{\frac{25dB}{10}}\\ &= 316,2\\ \Rightarrow P_R &= \frac{P_V}{316,2}\\ &= \frac{189,7W}{316,2}\\ &= 0,6W\end{split}$
</fragment>
</right>

---

[question:AG218]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $U_V = 300µV/m$
* gegeben: $U_R = 20µV/m$
</left>
<right>
* gegeben: $U_D = 128µV/m$
* gesucht: $g_D$, $\frac{Vor}{Rück}$
</right>

<left>
<fragment>
$\begin{split}g_D &= 20 \cdot \log_{10}{(\frac{U_V}{U_D})} dB\\ &= 20 \cdot \log_{10}{(\frac{300µV/m}{128µV/m})}\\ &= 7,4dB\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\frac{Vor}{Rück} &= 20 \cdot \log_{10}{(\frac{U_V}{U_R})} dB\\ &= 20 \cdot \log_{10}{(\frac{300µV/m}{20µV/m})}\\ &= 23,5dB\end{split}$
</fragment>
</right>
