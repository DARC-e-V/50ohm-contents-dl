## Genauigkeit von Frequenzen und Messbereichen

* Genauigkeitsangaben erfolgen in % (z.B. ${1 \cdot 10^{-2}}$) oder in parts per million (ppm = ${1 \cdot 10^{-6}}$)
* Manchmal wird auch direkt in Exponentialschreibweise angegeben, z.B. ${1 \cdot 10^{-7}}$
* Die angegebene Genauigkeit wird mit der Frequenz multipliziert, um die mögliche Abweichung von Messwerten oder Anzeigen zu berechnen

<note>
Hinweis bzgl. Umrechnung/Darstellung von 10er Potenzen:

\(1 \cdot 10^{-2} = \frac{1}{10^2}\)  
\(1 \cdot 10^{-6} = \frac{1}{10^6}\)  
usw.
</note>

---
[question:AA115]
---
#### Lösungsweg
* gegeben: $f = 435MHz$
* gesucht: $1ppm$ von $f$

<fragment>
$435MHz \cdot \frac{1}{10^6} = \frac{435\cdot \cancel{10^6}Hz}{\cancel{10^6}} = 435Hz$
</fragment>
---
[question:AA116]
---
#### Lösungsweg Teil 1
* gegeben: $f = 14,200.000MHz$
* gegeben: $\textrm{Abw.} = 10ppm$
* gesucht: $f_{min}, f_{max}$

<fragment>
$\begin{split}f_{min} &= f\,-\,f \cdot \frac{10}{10^6}\\ &= 14,2MHz\,-\,\frac{14,2\cdot \cancel{10^6}Hz\cdot 10}{\cancel{10^6}}\\ &= 14,2MHz\,-\,142Hz\\ &= 14,199858MHz\end{split}$
</fragment>
---
#### Lösungsweg Teil 2
* gegeben: $f = 14,200.000MHz$
* gegeben: $\textrm{Abw.} = 10ppm$
* gesucht: $f_{min}, f_{max}$

<fragment>
$\begin{split}f_{max} &= f\,+\,f \cdot \frac{10}{10^6}\\ &= 14,2MHz\,+\,\frac{14,2\cdot \cancel{10^6}Hz\cdot 10}{\cancel{10^6}}\\ &= 14,2MHz\,+\,142Hz\\ &= 14,200142MHz\end{split}$
</fragment>
---
[question:AI506]
---
#### Lösungsweg
* gegeben: $f = 29MHz$
* gegeben: $\textrm{Abw.} = 0,01\%$
* gesucht: $\Delta f$

<fragment>
$\begin{split}\Delta f &= 29MHz \cdot 0,01\%\\ &= 29\cdot \cancel{10^6}Hz \cdot 100\cdot \cancel{10^{-6}}\\ &= 2900Hz\end{split}$
</fragment>
---
[question:AI507]
---
#### Lösungsweg
* gegeben: $f = 14100kHz$
* gegeben: $\textrm{Abw.} = \pm0,00001\%$
* gesucht: $\Delta f$

<fragment>
$\begin{split}\Delta f &= 14100kHz \cdot 0,00001\%\\ &= 14,1\cdot \cancel{10^6}Hz \cdot 0,1\cdot \cancel{10^{-6}}\\ &= 1,41Hz\end{split}$
</fragment>
---
[question:AI508]
---
#### Lösungsweg
* gegeben: $f = 100MHz$
* gegeben: $\textrm{Abw.} = \pm1ppm$
* gesucht: $\Delta f$

<fragment>
$\begin{split}\Delta f &= 100MHz \cdot \frac{1}{10^6}\\ &= \frac{100\cdot \cancel{10^6}Hz}{\cancel{10^6}}\\ &= 100Hz\end{split}$
</fragment>
---
[question:AI509]
--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $f = 145MHz$
* gegeben: $\textrm{Abw.} = 10ppm$
* gesucht: $f_{min},f_{max}$

<fragment>
$\begin{split}\Delta f &= 145MHz \cdot \frac{10}{10^6}\\ &= \frac{145\cdot \cancel{10^6}Hz \cdot 10}{\cancel{10^6}}\\ &= 1450Hz\end{split}$
</fragment>
<fragment>
<left>
$\begin{split}f_{min} &= f\,-\,\Delta f\\ &= 145MHz\,-\,1450Hz\\ &= 144,99855MHz\end{split}$
</left>
<right>
$\begin{split}f_{max} &= f\,+\,\Delta f\\ &= 145MHz\,+\,1450Hz\\ &= 145,00145MHz\end{split}$
</right>
</fragment>
---
[question:AI510]
---
#### Lösungsweg
* gegeben: $f = 144,400MHz$
* gegeben: $\textrm{Abw.} = 1ppm$
* gegeben: $f_{B,max} = 2,7kHz$
* gesucht: $f_{B,max,Abw}$

<fragment>
<left>
$\begin{split}\Delta f &= 144,4MHz \cdot \frac{1}{10^6}\\ &= \frac{144,4\cdot \cancel{10^6}Hz}{\cancel{10^6}}\\ &= 144,4Hz\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}f_{B,max,Abw} &= f_{B,max} + \Delta f\\ &= 2,7kHz + 144,4Hz\\ &= 2,8444kHz\end{split}$
</right>
</fragment>
