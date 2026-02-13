### Transformator-Prinzip

<left>
[photo:239:e_Trafo mit getrennten Wicklungen:Trafo mit sichtbar getrennten Wicklungen]
</left>
<right>
* Magnetisch gekoppelte Spulen
* Veränderlicher Strom in einer Spule
* Erzeugt Spannung in der anderen Spule
* &rarr; Gegendinduktion
</right>

---
[question:AC301]
--- style="font-size: 0.7em;"
Das Verhältnis der Windungen zwischen Primär- und Sekundärseite ist wie das Verhältins der Spannung zwischen Primär- zu Sekundärseite, aber wie das Verhältnis der Ströme zwischen Sekundär- zu Primärseite:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S} = \frac{I_S}{I_P}$

<fragment>
Das Verhältnis der Primär- zur Sekundärimpedanz ist wie die obigen Verhältnisse zum Quadrat:

$ü = \frac{Z_P}{Z_S} = (\frac{N_P}{N_S})^2 = (\frac{U_P}{U_S})^2 = (\frac{I_S}{I_P})^2$
</fragment>

<fragment>
Oder nach Ziehung der Wurzel:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S} = \frac{I_S}{I_P} = \sqrt{\frac{Z_P}{Z_S}}$
</fragment>

<note>
Die letzte Formel steht so in der Formelsammlung
</note>
---
[question:AC302]
---
#### Lösungsweg
* gegeben: $U_P = 230V$
* gegeben: $U_S = 6V$
* gegeben: $I_S = 1,15A$
* gesucht: $I_P$

<fragment>
$\begin{split} \frac{U_P}{U_S} &= \frac{I_S}{I_P} \\ \Rightarrow I_P &= \frac{I_S \cdot U_S}{U_P} = \frac{1,15A \cdot 6V}{230V} \\ &= 30mA \end{split}$
</fragment>
---
[question:AC303]
---
#### Lösungsweg
* gegeben: $Z_S = 16k\Omega$
* gegeben: $ü = \frac{1}{4}$
* gesucht: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot 16k\Omega \\ &= \frac{16k\Omega}{16} = 1k\Omega \end{split}$
</fragment>

---
[question:AC304]
---
#### Lösungsweg
* gegeben: $Z_S = 6,4k\Omega$
* gegeben: $ü = \frac{1}{4}$
* gesucht: $Z_P$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} \\ \Rightarrow Z_P &= ü^2 \cdot Z_S = \frac{1^2}{4^2} \cdot 6,4k\Omega \\ &= \frac{6,4k\Omega}{16} = 0,4k\Omega \end{split}$
</fragment>

---
[question:AC305]
---
#### Lösungsweg
* gegeben: $Z_P = 450\Omega$
* gegeben: $Z_S = 50\Omega$
* gesucht: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{450\Omega}{50\Omega}} \\ &= \sqrt{\frac{9}{1}} = \frac{3}{1} \end{split}$
</fragment>

---
[question:AC306]
---
#### Lösungsweg
* gegeben: $Z_P = 50\Omega$
* gegeben: $Z_S = 2,5k\Omega$
* gesucht: $ü$

<fragment>
$\begin{split} ü &= \sqrt{\frac{Z_P}{Z_S}} = \sqrt{\frac{50\Omega}{2,5k\Omega}} \\ &= \sqrt{\frac{1}{50}} \approx \frac{1}{7} \end{split}$
</fragment>

---
### Maximaler Strom
<left>
* Leitung darf nicht zu warm werden
* Sonst schmilzt die Isolation
* Oder der Leiter glüht
* &rarr; zulässige Stromdichte in Stromstärke bezogen auf den Leiterquerschnitt
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

* Frei verlegte Leiter aus Kupfer: $\frac{12A}{0,75mm^2}$
* Schmelzsicherungen: bis zu $3000\frac{A}{mm^2}$
* Transformatoren: $2,5\frac{A}{mm^2}$ (schlechte Wärmeabstrahlung der Wicklungen)

---
[question:AC307]
---
#### Lösungsweg
* gegeben: $d = 0,5mm$
* gegeben: Stromdichte $\frac{I}{A} = \frac{2,5A}{1mm^2}$
* gesucht: $I_{max}$

<fragment>
$A_{Dr} = \frac{d^2 \cdot \pi}{4} = \frac{(0,5mm)^2 \cdot \pi}{4} \approx 0,196mm^2$
</fragment>
<fragment>
$I_{max} = \frac{I}{A} \cdot A_{Dr} = \frac{2,5A}{1mm^2} \cdot 0,196mm^2 = 0,49A$
</fragment>