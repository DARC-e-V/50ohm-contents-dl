### Transformator-Prinzip

<left>
[photo:239:e_Trafo mit getrennten Wicklungen:Trafo mit sichtbar getrennten Wicklungen]
</left>
<right>
* Magnetisch gekoppelte Spulen
* Veränderlicher Strom in einer Spule
* Erzeugt Spannung in der anderen Spule
* $\rightarrow$ Gegendinduktion
</right>

---
[question:AC301]
--- style="font-size: 0.7em;"
Das Verhältnis der Windungen zwischen Primär- und Sekundärseite ist wie das Verhältnis der Spannung zwischen Primär- zu Sekundärseite, aber wie das Verhältnis der Ströme zwischen Sekundär- zu Primärseite:

$ü = \frac{N_\text{P}}{N_\text{S}} = \frac{U_\text{P}}{U_\text{S}} = \frac{I_\text{S}}{I_\text{P}}$

<fragment>
Das Verhältnis der Primär- zur Sekundärimpedanz ist wie die obigen Verhältnisse zum Quadrat:

$ü^2 = \frac{Z_P}{Z_S} = \left(\frac{N_\text{P}}{N_\text{S}}\right)^2 = \left(\frac{U_\text{P}}{U_\text{S}}\right)^2 = \left(\frac{I_\text{S}}{I_\text{P}}\right)^2$
</fragment>

<fragment>
Oder nach ziehen der Wurzel:

$ü = \frac{N_\text{P}}{N_\text{S}} = \frac{U_\text{P}}{U_\text{S}} = \frac{I_\text{S}}{I_\text{P}} = \sqrt{\frac{Z_P}{Z_S}}$
</fragment>

<note>
Die letzte Formel steht so in der Formelsammlung
</note>
---
[question:AC302]
---
#### Lösungsweg
* gegeben: $U_\text{P} = \qty{230}{\volt}$
* gegeben: $U_\text{S} = \qty{6}{\volt}$
* gegeben: $I_\text{S} = \qty{1,15}{\ampere}$
* gesucht: $I_\text{P}$

<fragment>
$\begin{split} \frac{U_\text{P}}{U_\text{S}} &= \frac{I_\text{S}}{I_\text{P}} \\ \Rightarrow I_\text{P} &= \frac{I_\text{S} \cdot U_\text{S}}{U_\text{P}} = \frac{\qty{1,15}{\ampere} \cdot \qty{6}{\volt}}{\qty{230}{\volt}} \\ &= \qty{30}{\milli\ampere} \end{split}$
</fragment>

---
## Impedanzanpassung

<left>
[picture:260:a_impedanzanpassung:Anpassung von $\qty{2450}{\ohm}$ an $\qty{50}{\ohm}$ mit einem Übertrager mit einem Windungsverhältnis von 1 zu 7]
</left>
<right>
[photo:332:a_unun:Beispiel für einen Unun-Übertrager mit einem Windungsverhältnis von 2 zu 14, wobei die Primärseite und Sekundärseite zusammen bifilar (verdrillt) gewickelt sind]
</right>

---
[question:AC306]
---
#### Lösungsweg
* gegeben: $Z_P = \qty{50}{\ohm}$
* gegeben: $Z_S = \qty{2,5}{\kilo\ohm}$
* gesucht: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{\qty{50}{\ohm}}{\qty{2,5}{\kilo\ohm}}} \\ &= \sqrt{\frac{1}{50}} \approx \frac{1}{7} \end{split}$
</fragment>

---
[question:AC303]
---
#### Lösungsweg
* gegeben: $Z_S = \qty{16}{\kilo\ohm}$
* gegeben: $ü = \frac{1}{4}$
* gesucht: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot \qty{16}{\kilo\ohm} \\ &= \frac{\qty{16}{\kilo\ohm}}{16} = \qty{1}{\kilo\ohm} \end{split}$
</fragment>

---
[question:AC304]
---
#### Lösungsweg
* gegeben: $Z_S = \qty{6,4}{\kilo\ohm}$
* gegeben: $ü = \frac{1}{4}$
* gesucht: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot \qty{6,4}{\kilo\ohm} \\ &= \frac{\qty{6,4}{\kilo\ohm}}{16} = \qty{0,4}{\kilo\ohm} \end{split}$
</fragment>

---
[question:AC305]
---
#### Lösungsweg
* gegeben: $Z_P = \qty{450}{\ohm}$
* gegeben: $Z_S = \qty{50}{\ohm}$
* gesucht: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{\qty{450}{\ohm}}{\qty{50}{\ohm}}} \\ &= \sqrt{\frac{9}{1}} = \frac{3}{1} \end{split}$
</fragment>


---
### Maximaler Strom
<left>
* Leitung darf nicht zu warm werden
* Sonst schmilzt die Isolation
* Oder der Leiter glüht
* $\rightarrow$ zulässige Stromdichte in Stromstärke bezogen auf den Leiterquerschnitt
</left>
<right>
<fragment>
[photo:236:e_HF Übertrager:HF-Übertrager (BALUN), der bei zu viel Leistung schmelzen kann]
</fragment>
</right>
<note>
Geschmolzene, selbstgebastelte BALUNs in Plastikgehäusen kommen häufiger vor, wenn "nur noch etwas mehr Leistung" gegeben wird
</note>

---
### Beispiele zulässige Stromdichte

nach VDE

* Frei verlegte Leiter aus Kupfer: $\frac{\qty{12}{\ampere}}{\qty{0,75}{\milli\meter\squared}}$
* Schmelzsicherungen: bis zu $\qty{3000}{\ampere\per\milli\meter\squared}$
* Transformatoren: $\qty{2,5}{\ampere\per\milli\meter\squared}$ (schlechte Wärmeabstrahlung der Wicklungen)

---
[question:AC307]
---
#### Lösungsweg
* gegeben: $d = \qty{0,5}{\milli\meter}$
* gegeben: Stromdichte $\frac{I}{A} = \frac{\qty{2,5}{\ampere}}{\qty{1}{\milli\meter\squared}}$
* gesucht: $I_{\mathrm{max}}$

<fragment>
$A_{Dr} = \frac{d^2 \cdot \pi}{4} = \frac{(\qty{0,5}{\milli\meter})^2 \cdot \pi}{4} \approx \qty{0,196}{\milli\meter\squared}$
</fragment>
<fragment>
$I_{\mathrm{max}} = \frac{I}{A} \cdot A_{Dr} = \frac{\qty{2,5}{\ampere}}{\qty{1}{\milli\meter\squared}} \cdot \qty{0,196}{\milli\meter\squared} = \qty{0,49}{\ampere}$
</fragment>
