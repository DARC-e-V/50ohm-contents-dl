## Impedanztransformation im Speisekabel

* Wellenwiderstand ungleich Lastwiderstand führt neben Stehwellen zu Impedanztransformation
* Signalquelle "sieht" an den Kabelenden unterschiedliche Widerstände
* $\lambda/4$-Leitungen transformieren kleine in große und große in kleine Wirkwiderstände
* $\lambda/2$-Leitungen bewirken keine Impedanztransformation

---
[question:AG412]

---
[question:AG416]
---

### Speisung bei Halb- und Ganzwellendipolen

<left>
[picture:312:a_impedanztransformation_speiseleitung:Halbwellendipol mit Impedanztransformation über Speiseleitung]
</left>
<right>
* Halbwellendipol: stromgespeist (niederohmig)
* Ganzwellendipol: spannungsgespeist (hochohmig)
</right>

---
[question:AG413]

---
[question:AG414]

---
[question:AG415]
---

### Berechnung des Wellenwiderstands
* Für eine gezielte Impedanztransformation gilt: $Z = \sqrt{Z_\mathrm{E} \cdot Z_\mathrm{A}}$
* Der Wellenwiderstand ergibt sich als geometrisches Mittel aus Speise- und Lastwiderstand

---
[question:AG417]
---
#### Lösungsweg
* gegeben: $Z_A = 60Ω$
* gegeben: $Z_E = 240Ω$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{240Ω \cdot 60Ω}\\ &= 120Ω\end{split}$ 
</fragment>
---
[question:AG418]
---
#### Lösungsweg
* gegeben: $Z_A = 240Ω$
* gegeben: $Z_E = 600Ω$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{600Ω \cdot 240Ω}\\ &= 380Ω\end{split}$ 
</fragment>
---

### Impedanzanpassung mit Pi-Filtern

<left>
[picture:425:a_impedanztransformation_pi_filter:Pi-Filter zur Impedanztransformation]
</left>
<right>
* Spulen und Kondensatoren werden zur Impedanzanpassung eingesetzt
* Pi-Filter wirken als Tiefpass und transformieren die Impedanz
* Sie können als Antennentuner verwendet werden
</right>

<note>
Der Name "Pi-Filter" stammt von der Anordnung der Bauteile, die an den griechischen Buchstaben $\pi$ erinnern und nichts mit der Kreiszahl zu tun haben.
</note>

---
[question:AG406]
