## Näherungsformel für Feldstärke
<left>
* Berechnung der elektrischen Feldstärke
* Im Abstand zu einem Strahler
* Bei gegebener Leistung und Gewinn
* Gilt nur im Freiraum <br/> ($d > \frac{\lambda}{2\pi}$)
</left>
<right>
$\begin{split} E &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{d}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{d} \end{split}$
</right>

---
## Näherungsformel für Abstand
<left>
* Bei gegebener Feldstärke
* Umstellen nach $d$
</left>
<right>
$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_A \cdot G_i}}{E}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{E} \end{split}$
</right>

---
[question:EK108]
---
### Lösungsweg
<left>
* gegeben: $E = \qty{28}{\volt\per\meter}$
* gegeben: $g_d = \qty{7,5}{\dBd}$
* gegeben: $P_S = \qty{100}{\watt}$
</left>
<right>
* gegeben: $a_{\textrm{Kabel}} = \qty{1,5}{\dB}$
* gesucht: $P_{\textrm{EIRP}}$
* gesucht: $d$
</right>

<left>
<fragment>
$\begin{split} P_{\textrm{EIRP}} &= P_S \cdot 10^{\frac{g_d - a + \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ &= \qty{100}{\watt} \cdot 10^{\frac{\qty{7,5}{\dBd} - \qty{1,5}{\dB} + \qty{2,15}{\dB}}{\qty{10}{\dB}}}\\ &\approx \qty{100}{\watt} \cdot 6,5\\ &= \qty{650}{\watt} \end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot P_{\textrm{EIRP}}}}{E}\\ &= \dfrac{\sqrt{\qty{30}{\ohm} \cdot \qty{650}{\watt}}}{\qty{28}{\volt\per\meter}}\\ &\approx \qty{5}{\meter} \end{split}$
</fragment>
</right>

---
### Bonusfrage

Liegen die errechneten $\qty{5}{\meter}$ nicht im Nahfeld für das $\qty{10}{\meter}$-Band aus der Frage?

<fragment>
$\begin{split} d &> \frac{\lambda}{2\pi}\\ \qty{5}{\meter} &> \frac{\qty{10}{\meter}}{2\pi}\\ \qty{5}{\meter} &\gtrapprox \qty{1,6}{\meter} \end{split}$
</fragment>

---
[question:EK106]
---
### Lösung

* Personenschutz-Sicherheitsabstand gilt nur im Freiraum
* $d > \frac{\lambda}{2\pi}$
* $\qty{160}{\meter}$-Band: $\qty{25,5}{\meter}$
* $\qty{80}{\meter}$-Band: $\qty{12,7}{\meter}$

---
[question:EK105]

<note>
Liegt im Nahfeld, was wir vorher ausgerechnet haben
</note>

