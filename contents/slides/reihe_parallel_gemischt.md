### Parallelschwingkreis

* Spulen und Kondensatoren werden kombiniert
* Zu beachten ist auch die *Wicklungskapazität*
* Dadurch kommen "unsichtbare" Kapazitäten mit in die Schaltung

<note>
Eigenkapazität einer Spule
</note>
---
[question:AD101]
---
#### Lösungsweg

* gegeben: $C_1 = \qty{0,10}{\nano\farad}$
* gegeben: $C_2 = \qty{47}{\pico\farad}$
* gegeben: $C_3 = \qty{22}{\pico\farad}$
* gesucht: $C_{\mathrm{ges}}$

<fragment>
$\begin{split} \tfrac{1}{C_{\mathrm{ges}}} &= \tfrac{1}{C_1} + \tfrac{1}{C_2} + \tfrac{1}{C_3} = \tfrac{1}{\qty{0,10}{\nano\farad}} + \tfrac{1}{\qty{47}{\pico\farad}} + \tfrac{1}{\qty{22}{\pico\farad}}\\ &= \qty{7,67e10}{\farad^{-1}}\\ \Rightarrow C_{\mathrm{ges}} &= \frac{1}{\qty{7,67e10}{\farad^{-1}}} \approx \qty{13,0}{\pico\farad} \end{split}$
</fragment>
---
[question:AD103]
---
#### Lösungsweg

* gegeben: $C_1 = \qty{0,1}{\nano\farad}$
* gegeben: $C_2 = \qty{1,5}{\nano\farad}$
* gegeben: $C_3 = \qty{220}{\pico\farad}$
* gegeben: $C_\text{L} = \qty{1}{\pico\farad}$
* gesucht: $C_{\mathrm{ges}}$

<fragment>
$\begin{split} C_{\mathrm{ges}} &= C_1 + C_2 + C_3 + C_\text{L}\\ &= \qty{0,1}{\nano\farad} + \qty{1,5}{\nano\farad} + \qty{220}{\pico\farad} + \qty{1}{\pico\farad}\\ &= \qty{1821}{\pico\farad} \end{split}$
</fragment>
<note>
Einheitenpräfixe beachten und mit Kehrwerten rechnen
</note>

---
[question:AD105]
---
#### Lösungsweg

* gegeben: $R = \qty{100}{\ohm}$
* gegeben: $L = \qty{100}{\micro\henry}$
* gegeben: $f = \qty{1}{\mega\hertz}$
* gesucht: $Z$

<fragment>
$\begin{split} X_\text{L} &= \omega \cdot L = 2\pi \cdot f \cdot L\\ &= 2\pi \cdot \qty{1}{\mega\hertz} \cdot \qty{100}{\micro\henry} = \qty{628}{\ohm}\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{628}{\ohm})^2} \approx \qty{636}{\ohm}$
</fragment>

---
[question:AD104]
---
#### Lösungsweg

* gegeben: $R = \qty{100}{\ohm}$
* gegeben: $C = \qty{100}{\nano\farad}$
* gegeben: $f = \qty{1}{\mega\hertz}$
* gesucht: $Z$

<fragment>
$\begin{split} X_\text{C} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{1}{\mega\hertz} \cdot \qty{100}{\nano\farad}} = \qty{159}{\ohm}\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{159}{\ohm})^2} \approx \qty{188}{\ohm}$
</fragment>
