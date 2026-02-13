[picture:810:doppelsuper_blockschaltbild:Blockschaltbild eines Doppelsuper]

1. HF-Teil mit Vorselektion
2. Erster Mischer mit VFO
3. Erster ZF-Verstärker mit Roofing-Filter
4. Zweiter Mischer mit CO

--- data-transition="none"
[picture:810:doppelsuper_blockschaltbild:Blockschaltbild eines Doppelsuper]

5. Zweiter ZF-Verstärker mit Filter
6. Dritter Mischer als Produktdetektor oder Demodulator ggf. mit BFO
7. NF-Verstärker

--- data-transition="none"
[picture:810:doppelsuper_blockschaltbild:Blockschaltbild eines Doppelsuper]

* Verwendung von zwei Zwischenfrequenzen
* Hohe 1. ZF &rarr; gute Spiegelfrequenzunterdrückung
* Niedrige 2. ZF &rarr; hohe Trennschärfe

---
* Nach 1. ZF ist ein Eingangsfilter vor 2. Mischer
* Spiegelfrequenz lässt sich durch großen Abstand gut unterdrücken
* Nach 2. ZF Filter mit hoher Güte
* Lässt sich für niedrige Frequenzen gut realisieren
* ZF und gewünschte Empfangsfrequenz weit entfernt legen &rarr; Vermeidung des Direktempfangs der ZF
* Die 1. ZF sollte das Doppelte der maximalen Empfangsfrequenz sein

---
[question:AF112]
---
[question:AF113]
---
[question:AF114]
---
### Roofing Filter

* Nach 1. Mischer schmales Filter (*Roofing Filter*)
* Auf 1. ZF abgestimmt
* Bandbreite mindestens so groß wie größte benötigte Empfangsbandbreite

---
[question:AF116]
---
[question:AF209]
---
[question:AF117]
---
### Oszillator-Frequenzen
* Oszillatorfrequenzen sind jeweils ober- oder unterhalb der gewünschten Eingangsfrequenz
* Es existieren für jeden Mischer zwei Lösungsmöglichkeiten

<fragment>
1. $f_{OSZ} = f_{ZF}\,+\,f_{E}$
2. $f_{OSZ} = f_{ZF}\,-\,f_{E}$
</fragment>

---
[question:AF210]
--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $f_E = 3\dots30MHz$
* gegeben: $f_{ZF1} = 50MHz$
* gesucht: $f_{OSZ}$

<fragment>
$f_{ZF} = |f_E − f_{OSZ}| \Rightarrow f_{OSZ} = f_{ZF} \pm f_{E}$
</fragment>
<fragment>
1. Lösung: $\begin{split} f_{OSZ} &= f_{ZF} \, + \, f_{E}\\ &= 50MHz \, + \, 3\dots30MHz\\ &= 53\dots80MHz \end{split}$
2. Lösung: $\begin{split} f_{OSZ} &= f_{ZF} \, - \, f_{E}\\ &= 50MHz \, - \, 3\dots30MHz\\ &= 47\dots20MHz \end{split}$
</fragment>
---
[question:AF120]
--- style="font-size: smaller;"
### Lösungsweg
<left>
* gegeben: $f_{E} = 3,65MHz$
* gegeben: $f_{ZF1} = 50MHz$
</left>
<right>
* gegeben: $f_{ZF2} = 9MHz$
* gegeben: $f_{NF} = 455kHz$
</right>
* gesucht: $f_{OSZ}$ für $f_{VFO}, f_{CO1}, f_{CO2}$

<fragment>
$f_{ZF1} = \begin{cases}f_E\,+\,f_{OSZ}\\ f_{OSZ}\,-\,f_E\\ f_E\,-\,f_{OSZ}\end{cases} \Rightarrow f_{OSZ} = \begin{cases}f_{ZF}\,-\,f_E\\ f_E\,+\,f_{ZF}\\ f_E\,-\,f_{ZF}\end{cases}$
</fragment>
<fragment>
$f_{VFO} = \begin{cases}f_{ZF1}\,-\,f_E = 50MHz\,-\,3,65MHz = 46,35MHz\\ f_E\,+\,f_{ZF1} = 3,65MHz\,+\,50MHz = 53,64MHz\\ f_E\,-\,f_{ZF1} = 3,65MHz\,-\,50MHz = \cancel{-46,35MHz}\end{cases}$
</fragment>
--- style="font-size: smaller;"‚
<fragment>
$f_{CO1} = \begin{cases}f_{ZF2}\,-\,f_{ZF1} = 9MHz\,-\,50MHz = \cancel{-41MHz}\\ f_{ZF1}\,+\,f_{ZF2} = 50MHz\,+\,9MHz = 59MHz\\ f_{ZF1}\,-\,f_{ZF2} = 50MHz\,-\,9MHz = 41MHz\end{cases}$
</fragment>
<fragment>
$f_{CO2} = \begin{cases}f_{NF}\,-\,f_{ZF2} = 455kHz\,-\,9MHz = \cancel{-8,545MHz}\\ f_{ZF2}\,+\,f_{NF} = 9MHz\,+\,455kHz = 9,455MHz\\ f_{ZF2}\,-\,f_{NF} = 9MHz\,-\,455kHz = 8,545MHz\end{cases}$
</fragment>
<fragment>
VFO: $\bold{46,35MHz} \And 53,65MHz$, CO1: $\bold{41MHz} \And 59MHz$, CO2: $8,545MHz \And \bold{9,455MHz}$
</fragment>
---
[question:AF118]
--- style="font-size: smaller;"‚
#### Lösungsweg
<left>
* gegeben: $f_{E} = 21,1MHz$
* gegeben: $f_{ZF1} = 9MHz$
</left>
<right>
* gegeben: $f_{ZF2} = 460kHz$
</right>
* gesucht: $f_{VFO} \gt f_E, f_{CO} \lt f_{ZF1}$

<fragment>
$f_{ZF} = \begin{cases}f_{OSZ}\,-\,f_E\\ f_E\,-\,f_{OSZ}\end{cases} \Rightarrow f_{OSZ} = \begin{cases}f_E\,+\,f_{ZF}\\ f_E\,-\,f_{ZF}\end{cases}$
</fragment>
<fragment>
$f_{VFO} = f_E\,+\,f_{ZF1} = 21,1MHz\,+\,9MHz = 30,1MHz$
</fragment>
<fragment>
$f_{CO} = f_{ZF1}\,-\,f_{ZF2} = 9MHz\,-\,460kHz = 8,54MHz$
</fragment>

---
[question:AF119]
--- style="font-size: smaller;"‚
#### Lösungsweg
<left>
* gegeben: $f_{E} = 28MHz$
* gegeben: $f_{ZF1} = 10,7MHz$
</left>
<right>
* gegeben: $f_{ZF2} = 460kHz$
</right>
* gesucht: $f_{VFO} \gt f_E, f_{CO} \gt f_{ZF1}$

<fragment>
$f_{ZF} = \begin{cases}f_{OSZ}\,-\,f_E\\ f_E\,-\,f_{OSZ}\end{cases} \Rightarrow f_{OSZ} = \begin{cases}f_E\,+\,f_{ZF}\\ f_E\,-\,f_{ZF}\end{cases}$
</fragment>
<fragment>
$f_{VFO} = f_E\,+\,f_{ZF1} = 28MHz\,+\,10,7MHz = 38,70MHz$
</fragment>
<fragment>
$f_{CO} = f_{ZF1}\,+\,f_{ZF2} = 10,7MHz\,+\,460kHz = 11,16MHz$
</fragment>
