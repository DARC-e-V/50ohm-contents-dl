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

* gegeben: $C_1 = 0,10nF$
* gegeben: $C_2 = 47pF$
* gegeben: $C_3 = 22pF$
* gesucht: $C_{\textrm{ges}}$

<fragment>
$\begin{split} \tfrac{1}{C_{\textrm{ges}}} &= \tfrac{1}{C_1} + \tfrac{1}{C_2} + \tfrac{1}{C_3} = \tfrac{1}{0,10nF} + \tfrac{1}{47pF} + \tfrac{1}{22pF}\\ &= 7,67\cdot 10^{10} \tfrac{1}{F}\\ \Rightarrow C_{\textrm{ges}} &= \frac{1}{7,67\cdot 10^{10} \frac{1}{F}} \approx 13,0pF \end{split}$
</fragment>
---
[question:AD103]
---
#### Lösungsweg

* gegeben: $C_1 = 0,1nF$
* gegeben: $C_2 = 1,5nF$
* gegeben: $C_3 = 220pF$
* gegeben: $C_{\textrm{L}} = 1pF$
* gesucht: $C_{\textrm{ges}}$

<fragment>
$\begin{split} C_{\textrm{ges}} &= C_1 + C_2 + C_3 + C_{\textrm{L}}\\ &= 0,1nF + 1,5nF + 220pF + 1pF\\ &= 1821pF \end{split}$
</fragment>
<note>
Einheitenpräfixe beachten und mit Kehrwerten rechnen
</note>

---
[question:AD105]
---
#### Lösungsweg

* gegeben: $R = 100\Omega$
* gegeben: $L = 100\mu H$
* gegeben: $f = 1MHz$
* gesucht: $Z$

<fragment>
$\begin{split} X_{\textrm{L}} &= \omega \cdot L = 2 \cdot \pi \cdot f \cdot L\\ &= 2 \cdot \pi \cdot 1MHz \cdot 100\mu H = 628\Omega\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(100\Omega)^2 + (628\Omega)^2} \approx 636\Omega$
</fragment>

---
[question:AD104]
---
#### Lösungsweg

* gegeben: $R = 100\Omega$
* gegeben: $C = 100nF$
* gegeben: $f = 1MHz$
* gesucht: $Z$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2 \cdot \pi \cdot f \cdot C}\\ &= \frac{1}{2 \cdot \pi \cdot 1MHz \cdot 100nF} = 159\Omega\end{split}$
</fragment>
<fragment>
$Z = \sqrt{R^2 + X^2} = \sqrt{(100\Omega)^2 + (159\Omega)^2} \approx 188\Omega$
</fragment>
