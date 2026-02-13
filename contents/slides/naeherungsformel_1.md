## Näherungsformel für Feldstärke
<left>
* Berechnung der elektrischen Feldstärke
* Im Abstand zu einem Strahler
* Bei gegebener Leistung und Gewinn
* Gilt nur im Freiraum <br/> ($d > \frac{\lambda}{2\pi}$)
</left>
<right>
$\begin{split} E &= \dfrac{\sqrt{30\Omega \cdot P_A \cdot G_i}}{d}\\ &= \dfrac{\sqrt{30\Omega \cdot P_{\textrm{EIRP}}}}{d} \end{split}$
</right>

---
## Näherungsformel für Abstand
<left>
* Bei gegebener Feldstärke
* Umstellen nach $d$
</left>
<right>
$\begin{split} d &= \dfrac{\sqrt{30\Omega \cdot P_A \cdot G_i}}{E}\\ &= \dfrac{\sqrt{30\Omega \cdot P_{\textrm{EIRP}}}}{E} \end{split}$
</right>

---
[question:EK108]
---
### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $g_d = 7,5dBd$
* gegeben: $P_S = 100W$
</left>
<right>
* gegeben: $a_{\textrm{Kabel}} = 1,5dB$
* gesucht: $P_{\textrm{EIRP}}$
* gesucht: $d$
</right>

<left>
<fragment>
$\begin{split} P_{\textrm{EIRP}} &= P_S \cdot 10^{\frac{g_d - a + 2,15dB}{10dB}}\\ &= 100W \cdot 10^{\frac{7,5dB - 1,5dB + 2,15dB}{10dB}}\\ &\approx 100W \cdot 6,5\\ &= 650W \end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split} d &= \dfrac{\sqrt{30\Omega \cdot P_{\textrm{EIRP}}}}{E}\\ &= \dfrac{\sqrt{30\Omega \cdot 650W}}{28\frac{V}{m}}\\ &\approx 5m \end{split}$
</fragment>
</right>

---
### Bonusfrage

Liegen die errechneten 5m nicht im Nahfeld für das 10m-Band aus der Frage?

<fragment>
$\begin{split} d &> \frac{\lambda}{2\pi}\\ 5m &> \frac{10m}{2\pi}\\ 5m &\gtrapprox 1,6m \end{split}$
</fragment>

---
[question:EK106]
---
### Lösung

* Personenschutz-Sicherheitsabstand gilt nur im Freiraum
* $d > \frac{\lambda}{2\pi}$
* 160m-Band: 25,5 m
* 80m-Band: 12,7 m

---
[question:EK105]

<note>
Liegt im Nahfeld, was wir vorher ausgerechnet haben
</note>

