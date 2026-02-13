<left>
[photo:268:a_I eilt vor:Phasenverschiebung am Kondensator zwischen Spannung und Strom]
</left>
<right>
* Phasenverschiebung von 90°
* Strom eilt der Spannung voraus
</right>
<note>
Merke: Kondensatoooor, Strom eilt vooor!
</note>
---
[question:AC101]
---
### Wirkleistung
<left>
[picture:943:a_Blindleistung Kondensator:Das Produkt von U &times; I ergibt die grüne Leistungskurve]
</left>
<right>
* Die grüne Leistungskurve ist das Produkt von Strom und Spannung
* Die Leistung schwankt symmetrisch um die Nulllinie und gleicht sich aus
* *Blindleistung* an einem *Blindwiderstand*
</right>
---
[question:AC111]
<note>
Im eingeschwungenen Zustand fließt nahezu kein Strom mehr, weshalb die Leistung ebenso nahezu 0W ist.
</note>
---
* Wirkleistung wird nur in einem ohmschen Widerstand umgesetzt (Strom und Spannung in Phase)
* Blindwiderstand nimmt keine Wirkenergie auf
* Wird deshalb nicht warm
* Ein warmer Kondensator bei Hochfrequenz hat einen ohmschen Anteil und sollte ersetzt werden

---
[question:AC103]

--- style="font-size: smaller;"
### Kapazitiver Blindwiderstand $X_{\textrm{C}}$

Kondensator wird an Wechselspannung angeschlossen ständig geladen und entladen &rarr; Wechselstromwiderstand / kapazitiver Blindwiderstand

<fragment>
1. Wenn die Frequenz der Wechselspannung an einem Kondensator erhöht wird, dann fließt mehr Strom; dies bedeutet, der kapazitive Blindwiderstand ist kleiner geworden.
</fragment>
<fragment>
2. Wenn die Kapazität des Kondensators erhöht wird, dann steigt auch der Strom, d.h. der Blindwiderstand wird auch kleiner.
</fragment>

<fragment>
$X_{\textrm{C}} = \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}$
</fragment>

<note>
Ein VNA misst die Veränderung des Blindwiderstandes $X_C$ in Abhängigkeit der Frequenz
</note>
---
[question:AC102]
---
[question:AC104]
---
#### Lösungsweg
* gegeben: $C = 10pF$
* gegeben: $f = 100MHz$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot 100MHz \cdot 10pF}\\ &\approx 159\Omega \end{split}$
</fragment>

---
[question:AC105]
---
#### Lösungsweg
* gegeben: $C = 50pF$
* gegeben: $f = 145MHz$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot 145MHz \cdot 50pF}\\ &\approx 22\Omega \end{split}$
</fragment>
---
[question:AC106]
---
#### Lösungsweg
* gegeben: $C = 100pF$
* gegeben: $f = 100MHz$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot 100MHz \cdot 100pF}\\ &\approx 15,9\Omega \end{split}$
</fragment>

---
[question:AC107]
---
#### Lösungsweg
* gegeben: $C = 100pF$
* gegeben: $f = 435MHz$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot 435MHz \cdot 100pF}\\ &\approx 3,7\Omega \end{split}$
</fragment>

---
[question:AC108]
---
#### Lösungsweg
<left>
* gegeben: $U = 16V$
* gegeben: $I = 32mA$
</left>
<right>
* gegeben: $f = 50Hz$
* gesucht: $C$
</right>

<fragment>
$X_{\textrm{C}} = \frac{U}{I} = \frac{16V}{32mA} = 500\Omega$
</fragment>

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} \\ \Rightarrow C &= \frac{1}{\omega \cdot X_{\textrm{C}}} = \frac{1}{2\pi \cdot f \cdot X_{\textrm{C}}}\\ &= \frac{1}{2\pi \cdot 50Hz \cdot 500\Omega}\\ &\approx 6,37\mu F\end{split}$
</fragment>

---
### Kondensatorverluste

<left>
[photo:260:a_Kondensator Ersatzschaltbild:Ersatzschaltbild eines realen Kondensators mit einem seriellen Verlustwiderstand (ESR).]
</left>
<right>
* Verlustfaktor<br/>$\tan(\delta) = \frac{R}{X_C}$
* Verluste in Dielektrikum und Zuleitung
</right>

---
[question:AC109]
---
[question:AC110]
