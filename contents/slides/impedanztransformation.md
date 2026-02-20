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
* gegeben: $Z_A = \qty{60}{\ohm}$
* gegeben: $Z_E = \qty{240}{\ohm}$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{\qty{240}{\ohm} \cdot \qty{60}{\ohm}}\\ &= \qty{120}{\ohm}\end{split}$ 
</fragment>
---
[question:AG418]
---
#### Lösungsweg
* gegeben: $Z_A = \qty{240}{\ohm}$
* gegeben: $Z_E = \qty{600}{\ohm}$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \sqrt{Z_E \cdot Z_A}\\ &= \sqrt{\qty{600}{\ohm} \cdot \qty{240}{\ohm}}\\ &= \qty{380}{\ohm}\end{split}$ 
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
