<left>
[photo:267:a_U_eilt_vor:Phasenverschiebung an einer Spule zwischen Spannung und Strom]
</left>
<right>
* Phasenverschiebung von 90°
* Spannung eilt dem Strom voraus
</right>
<note>
Merke: Bei Induktivitäten, Ströme sich verspäten -oder- Induktivitääät, Strom zu spääät!
</note>

---
[question:AC201]

---
### Wirkleistung

<left>
[picture:944:a_Blindleistung Spule:Das Produkt von U &times; I ergibt die grüne Leistungskurve]
</left>
<right>
* Die grüne Leistungskurve ist das Produkt von Strom und Spannung
* Die Leistung schwankt symmetrisch um die Nulllinie und gleicht sich aus
* *Blindleistung* an einem *Blindwiderstand*
</right>

---

* Blindwiderstand nimmt keine Wirkenergie auf
* Eine ideale Spule wird nicht warm
* Jedoch besteht eine Spule aus Draht und hat dadurch ohmsche Verluste
* Zusätzlich wirkt der Skin-Effekt

---
[question:AC202]

--- style="font-size: smaller;"
### Induktiver Blindwiderstand $X_{\textrm{L}}$

Spule dreht an Wechselspannung angeschlossen ständig das magnetische Feld &rarr; Wechselstromwiderstand / induktiver Blindwiderstand

1. Wenn die Frequenz der Wechselspannung an einer Spule erhöht wird, dann fließt weniger Strom; dies bedeutet, der induktive Blindwiderstand ist größer geworden.
2. Wenn die Induktivität der Spule erhöht wird, dann verringert sich auch der Strom, d.h. der Blindwiderstand wird auch größer.

<fragment>
$X_{\textrm{L}} = \omega \cdot L = 2\pi \cdot f \cdot L$
</fragment>

---
[question:AC203]
---
[question:AC204]
---
#### Lösungsweg
* gegeben: $L = 3\mu H$
* gegeben: $f = 100MHz$
* gesucht: $X_{\textrm{L}}$

<fragment>
$\begin{split} X_{\textrm{L}} &= \omega \cdot L = 2\pi \cdot f \cdot L\\ &= 2\pi \cdot 100MHz \cdot 3\mu H\\ &\approx 1885\Omega \end{split}$
</fragment>

---
### Steigerung der Induktivität
<left>
Zylinderspule
<fragment>
$L = \dfrac{\mu_0 \cdot \mu_r \cdot N^2 \cdot A_S}{l}$
</fragment>

* Windungszahl $N$ erhöhen
* Spulenlänge $l$ verkürzen
* Querschnittsfläche $A_S$ der Spule vergrößern

</left>
<right>
Ringkernspule
<fragment>
$L = N^2 \cdot A_{\textrm{L}}$
</fragment>
  
* Windungszahl $N$ erhöhen
* Magnetisch leitfähigereres Material (mit größerer Induktivitätskonstante $A_{\textrm{L}}$) als Kern verwenden

</right>

<note>
Deshalb werden (Ring-)Kerne eingesetzt
</note>
---
[question:AC211]

---
[question:AC205]
---
#### Lösungsweg
* gegeben: $N = 14$
* gegeben: $A_{\textrm{L}} = 1,5nH$
* gesucht: $L$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ &= 14^2 \cdot 1,5nH\\ &= 0,294\mu H \end{split}$
</fragment>

---
[question:AC206]
---
#### Lösungsweg
* gegeben: $N = 300$
* gegeben: $A_{\textrm{L}} = 1250nH$
* gesucht: $L$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ &= 300^2 \cdot 1250nH\\ &= 112,5mH \end{split}$
</fragment>

---
[question:AC207]
---
#### Lösungsweg
* gegeben: $L = 2mH$
* gegeben: $A_{\textrm{L}} = 250nH$
* gesucht: $N$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ N &= \sqrt{\frac{L}{A_{\textrm{L}}}} = \sqrt{\frac{2mH}{250nH}} \\ &= 89\ \textrm{Windungen} \end{split}$
</fragment>

---
[question:AC208]
---
#### Lösungsweg
* gegeben: $L = 12\mu H$
* gegeben: $A_{\textrm{L}} = 30nH$
* gesucht: $N$

<fragment>
$\begin{split} L &= N^2 \cdot A_{\textrm{L}}\\ N &= \sqrt{\frac{L}{A_{\textrm{L}}}} = \sqrt{\frac{12\mu H}{30nH}} \\ &= 20\ \textrm{Windungen} \end{split}$
</fragment>

---
### Spulenverluste

* Verlustfaktor $\tan(\delta) = \frac{R}{X_L}$
* Verluste im Leiter

---
[question:AC209]

---
### Scheinwiderstand

* Reihenschaltung von Blindwiderstand und Wirkwiderstand &rarr; Scheinwiderstand $Z$
* Tritt nur bei Wechselspannung auf
* Kann nicht mit einem Ohm-Meter gemessen werden
* Spule in der Funktechnik &rarr; *Impedanz*
* Antennenimpedanz, Eingangs- und Ausgangsimpedanz, Impedanzwandler, …
* Impedanz Z in Ω

---
<left>
[photo:269:a_Widerstandsdreieck_R_L:Geometrische Addition von $R$ und $X_L$ und Phasenverschiebung zwischen $Z$ und $R$]
  
$Z = \sqrt{R^2 + X^2}$
</left>
<right>
* Wirkwiderstand $R$
* Blindwiderstand $X_{\textrm{L}}$
* Scheinwiderstand ist über Pythagoras zu berechnen
</right>

---
[question:AA101]

---
### Abschirmung von elektrischen Feldern

Ein Gehäuse aus einem magnetisch gut leitfähigem Material.

---
[question:AC210]
