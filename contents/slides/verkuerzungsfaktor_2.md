## Antennenlänge und Verkürzungsfaktor

* Antennenlänge hängt vom Verkürzungsfaktor ab  
* Halbwellendipol: Hälfte der Wellenlänge $\times$ Verkürzungsfaktor  
* Viertelwellenstrahler: Viertel der Wellenlänge $\times$ Verkürzungsfaktor  
* Typischer Wert: $\num{0,95}$  

---

[question:AG101]

---
#### Lösungsweg
<left>
* gegeben: $f = \qty{14,2}{\mega\hertz}$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{2}$-Dipol
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{14,2}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{21,13}{\meter}\\ &\approx \qty{5,28}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot \qty{5,28}{\meter}\\ &\approx \qty{5,02}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG102]

---

#### Lösungsweg
<left>
* gegeben: $f = \qty{7,1}{\mega\hertz}$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{2}$-Dipol
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7,1}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{42,25}{\meter}\\ &\approx \qty{10,56}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot \qty{10,56}{\meter}\\ &\approx \qty{10,04}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG103]

---
#### Lösungsweg
<left>
* gegeben: $l_G = \qty{20}{\meter}$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: Dipol
* gesucht: $f$
</right>

<left>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_E &= \frac{l_G}{k_v}\\ &= \frac{\qty{20}{\meter}}{0,95}\\ &\approx \qty{21,05}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{2}\\ &= \frac{1}{2} \cdot \frac{c}{f}\\ \Rightarrow f &= \frac{1}{2} \cdot \frac{c}{l_E}\\ &\approx \frac{1}{2} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{21,05}{\meter}}\\&\approx \qty{7,125}{\mega\hertz}\end{split}$
</fragment>
</right>

---

[question:AG104]

---

#### Lösungsweg
<left>
* gegeben: $f = \qty{7,1}{\mega\hertz}$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{4}$-Groundplane
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{4}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &\approx \frac{1}{4} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7,1}{\mega\hertz}}\\ &\approx \frac{1}{4} \cdot \qty{42,25}{\meter}\\ &\approx \qty{10,56}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot \qty{10,56}{\meter}\\ &\approx \qty{10,04}{\meter}\end{split}$
</fragment>
</right>

---

[question:AG105]

---

#### Lösungsweg
<left>
* gegeben: $f = \qty{14,2}{\mega\hertz}$
* gegeben: $k_v = 0,97$
</left>
<right>
* gegeben: $\frac{5}{8}\lambda$-Vertikalantenne
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{5}{8}\lambda\\ &= \frac{5}{8} \cdot \frac{c}{f}\\ &\approx \frac{5}{8} \cdot \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{14,2}{\mega\hertz}}\\ &\approx \frac{5}{8} \cdot \qty{21,13}{\meter}\\ &\approx \qty{13,20}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,97 \cdot \qty{13,20}{\meter}\\ &\approx \qty{12,80}{\meter}\end{split}$
</fragment>
</right>

---

### Ursache des Verkürzungsfaktors

* Leiter sind nicht unendlich dünn  
* Zusätzliche Kapazität zwischen Leiter und Umgebung  
* Beeinflusst die effektive elektrische Länge der Antenne  

---

[question:AG202]

---

### Verlängerungsfaktor bei Schleifenantennen

* Unterschied zum Verkürzungsfaktor  
* Führt zu einer scheinbaren Verlängerung der Antenne  

<note>
Ein Verlängerungsfaktor bedeutet <u>nicht</u>, dass sich die Welle mit *Überlichtgeschwindigkeit* ausbreitet. Es handelt sich um die Phasengeschwindigkeit, nicht um die Gruppengeschwindigkeit.
</note>

---

[question:AG118]

---

#### Lösungsweg
<left>
* gegeben: $f = \qty{7,1}{\mega\hertz}$
* gegeben: $k_v = 1,02$
</left>
<right>
* gegeben: Delta-Loop
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &= \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{7,1}{\mega\hertz}}\\ &\approx \qty{42,23}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 1,02 \cdot \qty{42,23}{\meter}\\ &\approx \qty{43,10}{\meter}\end{split}$
</fragment>
</right>

---

### Verkürzungsfaktor bei Paralleldrahtleitungen

* Welle befindet sich zwischen den Leitern  
* Skineffekt verhindert tiefes Eindringen ins Metall  
* Verkürzungsfaktor annähernd $1$ (wie Freiraumausbreitung)  

---

[question:AG313]

---

### Verkürzungsfaktor bei Koaxialkabeln

* Welle befindet sich im Dielektrikum zwischen den Leitern
* Beispiel für Polyäthylen: $\epsilon_\mathrm{r} = 2,29$  
* Skineffekt verhindert tiefes Eindringen ins Metall  
* Geometrie des Kabels hat kaum Einfluss  
* Berechnung des Verkürzungsfaktors:  

<fragment>
$v_\mathrm{k} = \dfrac{1}{\sqrt{\epsilon_\mathrm{r}}}$
</fragment>

---

[question:AG315]

---

[question:AG316]

---
#### Lösungsweg
* gegeben: $f = \qty{145}{\mega\hertz}$
* gegeben: $k_v = 0,66$
* gesucht: $l_G$

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &\approx \frac{\qty{3\cdot 10^8}{\meter\per\second}}{\qty{145}{\mega\hertz}}\\ &\approx \qty{2,07}{\meter}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,66 \cdot \qty{2,07}{\meter}\\ &\approx \qty{1,37}{\meter}\end{split}$
</fragment>
</right>