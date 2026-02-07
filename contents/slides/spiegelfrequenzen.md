<left>
[picture:807:spiegelfrequenzen_mischen1:Mischvorgang mit Empfangsfrequenz $f_\text{e}$, Oszillatorfrequenz $f_\text{o}$ und der Zwischenfrequenz $f_\text{ZF}$]

$f_{ZF} = \left|f_e \pm f_o\right|$
</left>
<right>  
Im Mischprozess zur $f_{ZF}$ werden prinzipbedingt immer zwei Empfangsfrequenzen ausgewählt
</right>

---
<left>
[picture:806:spiegelfrequenzen_fe1_fe2:Empfangsfrequenzen die beide zur selben $f_{ZF}$ führen]
</left>
<right>
* Gewünschte Empfangsfrequenz $f_{e1}$ &rarr; Spiegelfrequenz $f_{e2}$
* Abstand zwischen gewünschter Empfangsfrequenz und Spiegelfrequenz &rarr; ${2 \cdot f_{ZF}}$
</right>
---
<left>
Oszillator schwingt oberhalb der Empfangsfrequenz<br/>
&darr;<br/>
Spiegelfrequenz bei ${2 \cdot f_{ZF}}$ oberhalb der Empfangsfrequenz
</left>
<right>
Oszillator schwingt unterhalb der Empfangsfrequenz<br/>
&darr;<br/>
Spiegelfrequenz bei ${2 \cdot f_{ZF}}$ unterhalb der Empfangsfrequenz
</right>

---

$f_S = 2 \cdot f_{OSZ}\,-\,f_E =\\ \begin{cases}f_{OSZ}\,+\,f_{ZF} = f_E\,+\,2 \cdot f_{ZF} &\text{wenn } f_E \lt f_{OSZ} \\ f_{OSZ}\,-\,f_{ZF} = f_E\,-\,2 \cdot f_{ZF} &\text{wenn } f_E \gt f_{OSZ} \end{cases}$

---
## Spiegelfrequenzunterdrückung

<left>
[picture:808:spiegelfrequenzen_mischen2:Zusätzlicher Bandpassfilter zur Spiegelfrequenzunterdrückung]
</left>
<right>
* Ohne Unterdrückung kann die Spiegelfrequenz zu Empfangsstörungen führen
* Vermeidung: Gewünschte Frequenz wird durch einen Bandpassfilter selektiert
* Spiegelfrequenz wird möglichst maximal unterdrückt
</right>
---
Maßnahme für eine möglichst hohe Unterdrückung:
* Abstand zwischen gewünschter Empfangsfrequenz und Spiegelfrequenz durch eine hohe ZF möglichst groß wählen
* Bei einem großen Abstand kann ein hochwertiges Bandpassfilter leichter realisiert werden

---
[question:AF201]
---
[question:AF202]
---
#### Lösungsweg
* gegeben: $f_{OSZ} = 134,9MHz$
* gegeben: $f_E = 145,6MHz$
* gesucht: $f_S$

<fragment>
$\begin{split}f_S &= 2 \cdot f_{OSZ} - f_E\\ &= 2 \cdot 134,9MHz - 145,6MHz\\ &= 124,2MHz\end{split}$
</fragment>
---
[question:AF203]
---
#### Lösungsweg
* gegeben: $f_{OSZ} = 39MHz$
* gegeben: $f_E = 28,3MHz$
* gesucht: $f_S$

<fragment>
$\begin{split}f_S &= 2 \cdot f_{OSZ} - f_E\\ &= 2 \cdot 39MHz - 28,3MHz\\ &= 49,7MHz\end{split}$
</fragment>
---
[question:AF204]
---
[question:AF106]
---
[question:AF107]
---
#### Lösungsweg
* gegeben: $f_{OSZ} = 24,94MHz$
* gegeben: $f_E = 14,24MHz$
* gesucht: $f_S$

<fragment>
$\begin{split}f_S &= 2 \cdot f_{OSZ} - f_E\\ &= 2 \cdot 24,94MHz - 14,24MHz\\ &= 35,64MHz\end{split}$
</fragment>
---
[question:AF108]
---
#### Lösungsweg
* gegeben: $f_{ZF} = 10,7MHz$
* gegeben: $f_E = 28,5MHz$
* gesucht: $f_S$

<fragment>
Bei $f_E &lt; f_{OSZ}$:
$\begin{split}f_S &= f_E + 2 \cdot f_{ZF}\\ &= 28,5MHz + 2 \cdot 10,7MHz\\ &= 49,9MHz\end{split}$
</fragment>
---
[question:AF109]
---
[question:AF110]
---
[question:AF111]
