<left>
[photo:268:a_I eilt vor:Phasenverschiebung am Kondensator zwischen Spannung und Strom]
</left>
<right>
* Phasenverschiebung von $\qty{90}{\degree}$
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
[picture:943:a_Blindleistung Kondensator:Das Produkt von $U \cdot I$ ergibt die grüne Leistungskurve]
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
* gegeben: $C = \qty{10}{\pico\farad}$
* gegeben: $f = \qty{100}{\mega\hertz}$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{10}{\pico\farad}}\\ &\approx \qty{159}{\ohm} \end{split}$
</fragment>

---
[question:AC105]
---
#### Lösungsweg
* gegeben: $C = \qty{50}{\pico\farad}$
* gegeben: $f = \qty{145}{\mega\hertz}$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{145}{\mega\hertz} \cdot \qty{50}{\pico\farad}}\\ &\approx \qty{22}{\ohm} \end{split}$
</fragment>
---
[question:AC106]
---
#### Lösungsweg
* gegeben: $C = \qty{100}{\pico\farad}$
* gegeben: $f = \qty{100}{\mega\hertz}$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{100}{\pico\farad}}\\ &\approx \qty{15,9}{\ohm} \end{split}$
</fragment>

---
[question:AC107]
---
#### Lösungsweg
* gegeben: $C = \qty{100}{\pico\farad}$
* gegeben: $f = \qty{435}{\mega\hertz}$
* gesucht: $X_{\textrm{C}}$

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} = \frac{1}{2\pi \cdot f \cdot C}\\ &= \frac{1}{2\pi \cdot \qty{435}{\mega\hertz} \cdot \qty{100}{\pico\farad}}\\ &\approx \qty{3,7}{\ohm} \end{split}$
</fragment>

---
[question:AC108]
---
#### Lösungsweg
<left>
* gegeben: $U = \qty{16}{\volt}$
* gegeben: $I = \qty{32}{\milli\ampere}$
</left>
<right>
* gegeben: $f = \qty{50}{\hertz}$
* gesucht: $C$
</right>

<fragment>
$X_{\textrm{C}} = \frac{U}{I} = \frac{\qty{16}{\volt}}{\qty{32}{\milli\ampere}} = \qty{500}{\ohm}$
</fragment>

<fragment>
$\begin{split} X_{\textrm{C}} &= \frac{1}{\omega \cdot C} \\ \Rightarrow C &= \frac{1}{\omega \cdot X_{\textrm{C}}} = \frac{1}{2\pi \cdot f \cdot X_{\textrm{C}}}\\ &= \frac{1}{2\pi \cdot \qty{50}{\hertz} \cdot \qty{500}{\ohm}}\\ &\approx \qty{6,37}{\micro\farad}\end{split}$
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
