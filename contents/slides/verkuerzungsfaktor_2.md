## Antennenlänge und Verkürzungsfaktor

* Antennenlänge hängt vom Verkürzungsfaktor ab  
* Halbwellendipol: Hälfte der Wellenlänge $\times$ Verkürzungsfaktor  
* Viertelwellenstrahler: Viertel der Wellenlänge $\times$ Verkürzungsfaktor  
* Typischer Wert: $0,95$  

---

[question:AG101]

---
#### Lösungsweg
<left>
* gegeben: $f = 14,2MHz$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{2}$-Dipol
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &= \frac{1}{4} \cdot \frac{3\cdot 10^8\frac{m}{s}}{14,2MHz}\\ &= \frac{1}{4} \cdot 21,13m\\ &= 5,28m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot 5,28m\\ &= 5,02m\end{split}$
</fragment>
</right>

---

[question:AG102]

---

#### Lösungsweg
<left>
* gegeben: $f = 7,1MHz$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{2}$-Dipol
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{1}{2} \cdot \frac{\lambda}{2}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &= \frac{1}{4} \cdot \frac{3\cdot 10^8\frac{m}{s}}{7,1MHz}\\ &= \frac{1}{4} \cdot 42,25m\\ &= 10,56m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot 10,56m\\ &= 10,04m\end{split}$
</fragment>
</right>

---

[question:AG103]

---
#### Lösungsweg
<left>
* gegeben: $l_G = 20m$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: Dipol
* gesucht: $f$
</right>

<left>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_E &= \frac{l_G}{k_v}\\ &= \frac{20m}{0,95}\\ &= 21,05m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{2}\\ &= \frac{1}{2} \cdot \frac{c}{f}\\ \Rightarrow f &= \frac{1}{2} \cdot \frac{c}{l_E}\\ &= \frac{1}{2} \cdot \frac{3\cdot 10^8\frac{m}{s}}{21,05m}\\&= 7,125MHz\end{split}$
</fragment>
</right>

---

[question:AG104]

---

#### Lösungsweg
<left>
* gegeben: $f = 7,1MHz$
* gegeben: $k_v = 0,95$
</left>
<right>
* gegeben: $\frac{\lambda}{4}$-Groundplane
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{\lambda}{4}\\ &= \frac{1}{4} \cdot \frac{c}{f}\\ &= \frac{1}{4} \cdot \frac{3\cdot 10^8\frac{m}{s}}{7,1MHz}\\ &= \frac{1}{4} \cdot 42,25m\\ &= 10,56m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,95 \cdot 10,56m\\ &= 10,04m\end{split}$
</fragment>
</right>

---

[question:AG105]

---

#### Lösungsweg
<left>
* gegeben: $f = 14,2MHz$
* gegeben: $k_v = 0,97$
</left>
<right>
* gegeben: $\frac{5}{8}\lambda$-Vertikalantenne
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \frac{5}{8}\lambda\\ &= \frac{5}{8} \cdot \frac{c}{f}\\ &= \frac{5}{8} \cdot \frac{3\cdot 10^8\frac{m}{s}}{14,2MHz}\\ &= \frac{5}{8} \cdot 21,13\\ &= 13,20m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,97 \cdot 13,20m\\ &= 12,80m\end{split}$
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
* gegeben: $f = 7,1MHz$
* gegeben: $k_v = 1,02$
</left>
<right>
* gegeben: Delta-Loop
* gesucht: $l_G$
</right>

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &= \frac{3\cdot 10^8\frac{m}{s}}{7,1MHz}\\ &= 42,23m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 1,02 \cdot 42,23m\\ &= 43,10m\end{split}$
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
* gegeben: $f = 145MHz$
* gegeben: $k_v = 0,66$
* gesucht: $l_G$

<left>
<fragment>
$\begin{split}l_E &= \lambda\\ &= \frac{c}{f}\\ &= \frac{3\cdot 10^8\frac{m}{s}}{145MHz}\\ &= 2,07m\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}k_v &= \frac{l_G}{l_E}\\ \Rightarrow l_G &= k_v \cdot l_E\\ &= 0,66 \cdot 2,07m\\ &= 1,37m\end{split}$
</fragment>
</right>