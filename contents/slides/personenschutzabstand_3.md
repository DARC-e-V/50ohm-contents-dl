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
* Kabelverluste werden als Dämpfungsfaktor (z. B. $\qty{10}{\dB}$ → $\num{0,1}$) berücksichtigt  
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
* gegeben: $g_d = \qty{6}{\dBd}$
* gegeben: $E = \qty{28}{\volt\per\meter}$
</left>
<right>
* gegeben: $d = \qty{5}{\meter}$
* gesucht: $P_S$
</right>

<fragment>
<left>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ \Rightarrow P_{EIRP} &= \frac{(E \cdot d)^2}{\qty{30}{\ohm}}\\ &= \frac{(\qty{28}{\volt\per\meter} \cdot \qty{5}{\meter})^2}{\qty{30}{\ohm}}\\ &\approx \qty{653}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d - a + 2,15dB}{\qty{10}{\dB}}}\\ \Rightarrow P_S &= \frac{P_{EIRP}}{10^{\frac{g_d - a + 2,15dB}{\qty{10}{\dB}}}}\\ &= \frac{\qty{653}{\watt}}{10^{\frac{\qty{6}{\dBd} - \qty{0}{\dB} + 2,15dB}{\qty{10}{\dB}}}}\\ &\approx \frac{\qty{653}{\watt}}{6,53}\\ &= \qty{100}{\watt}\end{split}$
</right>
</fragment>

---

[question:AK113]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $g_i = \qty{12,15}{\dBi}$
* gegeben: $P_A = \qty{250}{\watt}$
</left>
<right>
* gegeben: $d = \qty{30}{\meter}$
* gesucht: $E$
</right>

<fragment>
<left>
$\begin{split}G_i &= 10^{\frac{g_i}{\qty{10}{\dB}}}\\ &= 10^{\frac{\qty{12,15}{\dBi}}{\qty{10}{\dB}}}\\ &\approx 16,4\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{250}{\watt} \cdot 16,4}}{\qty{30}{\meter}}\\ &\approx \frac{\qty{350}{\volt}}{\qty{30}{\meter}}\\ &\approx \qty{11,7}{\volt\per\meter}\end{split}$
</right>
</fragment>

---

[question:AK114]

--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $P_{ERP} = \qty{100}{\watt}$
* gegeben: $d = \qty{100}{\meter}$
* gesucht: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1,64\\ &= \qty{100}{\watt} \cdot 1,64\\ &= \qty{164}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{164}{\watt}}}{\qty{100}{\meter}}\\ &\approx \qty{0,7}{\volt\per\meter}\end{split}$
</right>
</fragment>

---

[question:AK115]

--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $P_{ERP} = \qty{100}{\watt}$
* gegeben: $d = \qty{100}{\meter}$
* gesucht: $E$

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_{ERP} \cdot 1,64\\ &= \qty{100}{\watt} \cdot 1,64\\ &= \qty{164}{\watt}\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{\qty{30}{\ohm} \cdot P_{EIRP}}}{d}\\ &= \frac{\sqrt{\qty{30}{\ohm} \cdot \qty{164}{\watt}}}{\qty{100}{\meter}}\\ &\approx \qty{0,7}{\volt\per\meter}\end{split}$
</right>
</fragment>
