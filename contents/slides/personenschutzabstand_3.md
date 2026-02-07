## Feldwellenwiderstand und Feldstärken
* Feldwellenwiderstand im Vakuum:
* $Z_{F0} = \sqrt{\dfrac{\mu_0}{\varepsilon_0}}$
* $\mu_0$ ist die magnetische Feldkonstante, $\varepsilon_0$ die elektrische Feldkonstante  
* Magnetische Feldstärke wird über $\mu_0$, magnetische Flussdichte und Magnetisierung berechnet  

---

* In einem Medium (z. B. Luft) gilt:
* $Z_{F} = \sqrt{\dfrac{\mu}{\varepsilon}}$
* Elektrische und magnetische Feldstärke hängen vom Wellenwiderstand des Mediums ab

---
[question:AK102]

---
### Leistung am Einspeisepunkt der Antenne

* Antenneneingangsleistung ergibt sich aus der Sendeleistung abzüglich der Kabeldämpfung  
* Kabelverluste werden als Dämpfungsfaktor (z. B. 10 dB → 0,1) berücksichtigt  
* Formel: $P_{Ant} = D \cdot P_{Sender}$

---
[question:AK104]

---
## Maximale Sendeleistung gemäß BEMFV

* Sicherheitsabstand muss im Fernfeld liegen:  

<fragment>
$d > \dfrac{\lambda}{2\pi}$  
</fragment>

---

[question:AK107]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_d = 6dBd$
* gegeben: $E = 28\frac{V}{m}$
</left>
<right>
* gegeben: $d = 5m$
* gesucht: $P_S$
</right>

<fragment>
<left>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow P_{EIRP} &= \frac{(E \cdot d)^2}{30Ω}\\ &= \frac{(28\frac{V}{m} \cdot 5m)^2}{30Ω}\\ &= 653W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d - a + 2,15dB}{10dB}}\\ \Rightarrow P_S &= \frac{P_{EIRP}}{10^{\frac{g_d - a + 2,15dB}{10dB}}}\\ &= \frac{653W}{10^{\frac{6dBd - 0 + 2,15dB}{10dB}}}\\ &= \frac{653W}{6,53}\\ &\approx 100W\end{split}$
</right>
</fragment>

---

[question:AK113]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_i = 12,15dBi$
* gegeben: $P_A = 250W$
</left>
<right>
* gegeben: $d = 30m$
* gesucht: $E$
</right>

<fragment>
<left>
$\begin{split}G_i &= 10^{\frac{g_i}{10dB}}\\ &= 10^{\frac{12,15dBi}{10dB}}\\ &= 16,4\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_A \cdot G_i}}{d}\\ &= \frac{\sqrt{30Ω \cdot 250W \cdot 16,4}}{30m}\\ &= \frac{350V}{30m}\\ &\approx 11,7\frac{V}{m}\end{split}$
</right>
</fragment>

---

[question:AK114]

--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $P_{ERP} = 100W$
* gegeben: $d = 100m$
* gesucht: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1,64\\ &= 100W \cdot 1,64\\ &= 164W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{30Ω \cdot 164W}}{100m}\\ &= 0,7\frac{V}{m}\end{split}$
</right>
</fragment>

---

[question:AK115]

--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $P_{ERP} = 100W$
* gegeben: $d = 100m$
* gesucht: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1,64\\ &= 100W \cdot 1,64\\ &= 164W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{30Ω \cdot 164W}}{100m}\\ &= 0,7\frac{V}{m}\end{split}$
</right>
</fragment>
