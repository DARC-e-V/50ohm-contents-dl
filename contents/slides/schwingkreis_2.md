## Grenzfrequenz

Bei Hoch- und Tiefpässen gilt für die Grenzfrequenz

<left>
Bei RL-Gliedern
$R = X_\text{L}$
$f_\text{g} = \frac{R}{2 \pi \cdot L}$
</left>
<right>
Bei RC-Gliedern
$R = X_\text{C}$
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C}$
</right>


---
[question:AD201]
---
#### Lösungsweg
* gegeben: $R = \qty{4,7}{\kilo\ohm}$
* gegeben: $C = \qty{2,2}{\nano\farad}$
* gesucht: $f_\text{g}$

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C} = \frac{1}{2 \pi \cdot \qty{4,7}{\kilo\ohm} \cdot \qty{2,2}{\nano\farad}} \approx \qty{15,4}{\kilo\hertz}$
</fragment>
---
[question:AD202]
---
#### Lösungsweg
* gegeben: $R = \qty{10}{\kilo\ohm}$
* gegeben: $C = \qty{47}{\nano\farad}$
* gesucht: $f_\text{g}$

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C} = \frac{1}{2 \pi \cdot \qty{10}{\kilo\ohm} \cdot \qty{47}{\nano\farad}} \approx \qty{339}{\hertz}$
</fragment>
---
[question:AD203]
---
#### Lösungsweg
* gegeben: $R_1 = \qty{4,7}{\kilo\ohm}$
* gegeben: $C_1 = \qty{6,8}{\nano\farad}$
* gesucht: $f_\text{g}$

<fragment>
$C_2$ und alle weiteren Angaben sind für den Tiefpass uninteressant.
</fragment>

<fragment>
$f_\text{g} = \frac{1}{2 \pi \cdot R_1 \cdot C_1} = \frac{1}{2 \pi \cdot \qty{4,7}{\kilo\ohm} \cdot \qty{6,8}{\nano\farad}} \approx \qty{5}{\kilo\hertz}$
</fragment>
---
## Resonanzfrequenz

* Parallel- oder Reihenschaltung von Spule und Kondensator $\rightarrow$ Schwingkreis
* Hohe Frequenzen $\rightarrow$ hoher Widerstand an Spule
* Niedrige Frequenzen $\rightarrow$ hoher Widerstand an Kondensator
* Es gibt eine Frequenz, bei der Spule und Kondensator den gleichen Widerstand haben $\rightarrow$ *Resonanzfrequenz*

---
[question:AD206]
--- style="font-size: smaller;"
## Parallelschwingkreis

[picture:233:a_schwingkreis_parallelschwingkreis:Parallelschwingkreis und Darstellung der Impedanz gegenüber der Frequenz]

* Ideale Bauelemente laden sich ständig um
* Theoretisch ist die Impedanz bei Resonanzfrequenz unendlich hoch
* Praktisch bestimmt das Bauteil mit dem geringsten Widerstand die Gesamtimpedanz
* Bei Frequenzen über und unter der Resonanzfrequenz hat der Parallelschwingkreis eine geringere Impedanz

--- style="font-size: smaller;"
## Reihenschwingkreis

[picture:230:a_schwingkreis_reihenschwingkreis:Reihenschwingkreis und Darstellung der Impedanz gegenüber der Frequenz]

* Oder Serienschwingkreis
* Theoretisch ist die Impedanz bei Resonanzfrequenz $\qty{0}{\ohm}$
* Praktisch wird die Impedanz durch den ohmschen Widerstand bestimmt
* Bei Frequenzen über und unter der Resonanzfrequenz hat der Reihenschwingkreis eine höhere Impedanz

---
[question:AD207]
---
[question:AD204]
---
## Resonanzfall

Für Parallel- und Reihenschwingkreis:

$X_\text{C} = X_\text{L}$

Impedanzen sind gleich groß.

<fragment>
Resonanzfrequenz mit Thomsonsche Schwingkreisformel:

$f_0 = \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}$
</fragment>

<note>
William Thomson, später Lord Kelvin, in 1853
</note>
---


[question:AD208]
---
#### Lösungsweg
* gegeben: $L = \qty{1,2}{\micro\henry}$
* gegeben: $C = \qty{6,8}{\pico\farad}$
* gegeben: $R = \qty{10}{\ohm}$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{1,2}{\micro\henry} \cdot \qty{6,8}{\pico\farad}}} \approx \qty{55,7}{\mega\hertz} \end{split}$
</fragment>
<fragment>
Widerstand $R$ wird zur Berechnung nicht benötigt.
</fragment>
---
[question:AD209]
---
#### Lösungsweg
* gegeben: $L = \qty{10}{\micro\henry}$
* gegeben: $C = \qty{1}{\nano\farad}$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{10}{\micro\henry} \cdot \qty{1}{\nano\farad}}} \approx \qty{1,592}{\mega\hertz} \end{split}$
</fragment>
---
[question:AD210]
---
#### Lösungsweg
* gegeben: $L = \qty{100}{\micro\henry}$
* gegeben: $C = \qty{0,01}{\micro\farad}$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{100}{\micro\henry} \cdot \qty{0,01}{\micro\farad}}} \approx \qty{159}{\kilo\hertz} \end{split}$
</fragment>
---
[question:AD211]
---
#### Lösungsweg
* gegeben: $L = \qty{2,2}{\micro\henry}$
* gegeben: $C = \qty{56}{\pico\farad}$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{2,2}{\micro\henry} \cdot \qty{56}{\pico\farad}}} \approx \qty{14,34}{\mega\hertz} \end{split}$
</fragment>
---
[question:AD212]
--- style="font-size: 0.7em;"
#### Lösungsweg
* gegeben: $C_1 = \qty{0,1}{\nano\farad}$
* gegeben: $C_2 = \qty{1,5}{\nano\farad}$
* gegeben: $C_3 = \qty{220}{\pico\farad}$
* gegeben: $L = \qty{1,2}{\milli\henry}$
* gesucht: $f_0$

<fragment>
$C = C_1 + C_2 + C_3 = \qty{0,1}{\nano\farad} + \qty{1,5}{\nano\farad} + \qty{220}{\pico\farad} = \qty{1,82}{\nano\farad}$
</fragment>
<fragment>
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{1,2}{\milli\henry} \cdot \qty{1,82}{\nano\farad}}} \approx \qty{107,7}{\kilo\hertz} \end{split}$
</fragment>
---
### Verändern der Resonanzfrequenz

* Größere Spule oder Kondensator $\rightarrow$ kleinere Resonanzfrequenz
* Kleinere Spule oder Kondensator $\rightarrow$ größere Resonanzfrequenz

<fragment>
Induktivität vergrößern
* Vergrößern der Windungszahl
* Zusammenschieben
* Einführen eines Ferritkerns

</fragment>

---
[question:AD213]
---
[question:AD214]
---
[question:AD215]
---
[question:AD216]
---
[question:AD217]
---
### Spannungsgesteuerter Schwingkreis

[picture:752:a_schwingkreis_potentiometer:Veränderung der Kapazität durch einen Varicap]

* Varicap wird durch eine Steuerspannung am Widerstandsspannungsteiler verändert
* Kleinere Spannung am Varicap $\rightarrow$ kleinere Grenzschicht im Varicap $\rightarrow$ größere Kapazität
* In Reihe geschaltete Kondensatoren $\rightarrow$ Kapazität wird kleiner $\rightarrow$ Resonanzfrequenz steigt

---
[question:AD218]
--- style="font-size: smaller;"
## Bandpassfilter

[picture:785:a_schwingkreis_bandpass:Bandpassfilter aus mehreren Schwingkreisen]

* Kombination aus Parallel- und Reihenschwingkreisen
* Lässt einen bestimmten Frequenzbereich passieren
* Parallelschwingkreise wie hochohmige Widerstände
* Reihenschwingkreis wie niederohmiger Widerstand

---
[question:AD205]
---
## Bandbreite

* Große Abhängigkeit vom ohmschen Widerstand
* In Angabe von dB auf einen Referenzwert des Filters
* Z.B. *Bandbreite* bei *$\qty{-3}{\dB}$-Wert*
* Halbe Leistung eines Signals kann noch das Filter passieren
* Oder die $\num{0,7}$-fache Signalspannung

---
[question:AD219]
---
[question:AD220]
---
### Übliche Bandbreiten

* Schmalbandig mit $\qty{500}{\hertz}$ für Telegrafie (CW)
* Breitbandig mit $\qty{2,7}{\kilo\hertz}$ für Sprachmodulation (SSB)

---
[question:AD221]
---
[question:AD222]
---
## Güte eines Schwingkreises

* Auch Q-Faktor
* Kennzeichen für Energieverlust
* Verhältnis der Blindwiderstände zum ohmschen Widerstand im Resonanzfall ($X_\text{L} = X_\text{C}$)

<fragment>
<left>
Reihenschwingkreis
$Q = \frac{f_0}{B} = \frac{X_\text{L}}{R_\text{S}}$
</left>
<right>
Parallelschwingkreis
$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$
</right>
</fragment>
  
---
[question:AD225]
--- style="font-size: 0.7em;"
#### Lösungsweg
<left>
* gegeben: $L = \qty{100}{\micro\henry}$
* gegeben: $C = \qty{0,01}{\micro\farad}$
</left>
<right>
* gegeben: $R_\text{S} = \qty{10}{\ohm}$
* gesucht: $Q$
</right>

<fragment>
Zuerst $f_0$ ausrechnen
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{100}{\micro\henry} \cdot \qty{0,01}{\micro\farad}}} \approx \qty{159,2}{\kilo\hertz} \end{split}$
</fragment>
<fragment>
Dann $B$ oder $X_\text{L}$ ausrechnen
$\begin{split} X_\text{L} &= \omega \cdot L = 2 \pi \cdot f_0 \cdot L\\ &= 2 \pi \cdot \qty{159,2}{\kilo\hertz} \cdot \qty{100}{\micro\henry} \approx \qty{100,03}{\ohm} \end{split}$
</fragment>
<fragment>
$Q = \frac{X_\text{L}}{R_\text{S}} = \frac{\qty{100,03}{\ohm}}{\qty{10}{\ohm}} \approx 10$
</fragment>
---
[question:AD226]
--- style="font-size: 0.7em;"
#### Lösungsweg
<left>
* gegeben: $L = \qty{2,2}{\micro\henry}$
* gegeben: $C = \qty{56}{\pico\farad}$
</left>
<right>
* gegeben: $R_\text{P} = \qty{1}{\kilo\ohm}$
* gesucht: $Q$
</right>

<fragment>
Zuerst $f_0$ ausrechnen
$\begin{split} f_0 &= \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \pi \cdot \sqrt{\qty{2,2}{\micro\henry} \cdot \qty{56}{\pico\farad}}} \approx \qty{14,34}{\mega\hertz} \end{split}$
</fragment>
<fragment>
Dann $B$ oder $X_\text{L}$ ausrechnen
$\begin{split} X_\text{L} &= \omega \cdot L = 2 \pi \cdot f_0 \cdot L\\ &= 2 \pi \cdot \qty{14,34}{\mega\hertz} \cdot \qty{2,2}{\micro\henry} \approx \qty{198,2}{\ohm} \end{split}$
</fragment>
<fragment>
$Q = \frac{R_\text{P}}{X_\text{L}} = \frac{\qty{1}{\kilo\ohm}}{\qty{198,2}{\ohm}} \approx 5$
</fragment>
---
### Bandbreite berechnen

Über Resonanzfrequenz und Güte

$Q = \frac{f_0}{B} \Rightarrow B = \frac{f_0}{Q}$

<fragment>
Oder eingesetzt mit der Thomsonschen Schwingkreisformel

<left>
Reihenschwingkreis
$B = \frac{R_\text{S}}{2 \pi \cdot L}$
</left>
<right>
Parallelschwingkreis
$B = \frac{1}{2 \pi \cdot R_\text{P} \cdot C}$
</right>
</fragment>
<note>
Herleitung nicht gezeigt
</note>

---
[question:AD224]
---
#### Lösungsweg
* gegeben: $L = \qty{2,2}{\micro\henry}$
* gegeben: $C = \qty{56}{\pico\farad}$
* gegeben: $R_\text{P} = \qty{1}{\kilo\ohm}$
* gesucht: $B$

<fragment>
$\begin{split} B &= \frac{1}{2 \pi \cdot R_\text{P} \cdot C}\\ &= \frac{1}{2 \pi \cdot \qty{1}{\kilo\ohm} \cdot \qty{56}{\pico\farad}} \approx \qty{2,84}{\mega\hertz} \end{split}$
</fragment>

---
[question:AD223]
---
#### Lösungsweg
* gegeben: $L = \qty{100}{\micro\henry}$
* gegeben: $C = \qty{0,01}{\micro\farad}$
* gegeben: $R_\text{S} = \qty{10}{\ohm}$
* gesucht: $B$

<fragment>
$B = \frac{R_\text{S}}{2 \pi \cdot L} = \frac{\qty{10}{\ohm}}{2 \pi \cdot \qty{100}{\micro\henry}} \approx \qty{15,9}{\kilo\hertz}$
</fragment>
--- style="font-size: 0.7em;" data-transition="none"
## Kopplung

[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* Zwischen Schaltungsstufen oder Filtern werden häufig gekoppelte Schwingkreise verwendet
* Zwei Schwingkreise induktiv oder kapazitiv aneinander gekoppelt
* Grad der Kopplung bestimmt die gegenseitige Beeinflussung, Bandbreite und Durchlasskurve

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* d: *lose Kopplung* $\rightarrow$ kaum gegenseitige Beeinflussung, sehr hohe Durchlassdämpfung und sehr geringe Bandbreite
* c: *unterkritische Kopplung* $\rightarrow$ kaum gegenseitige Beeinflussung, hohe Durchlassdämpfung und geringe Bandbreite

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* b: *kritische Kopplung* $\rightarrow$ etwas gegenseitige Beeinflussung, flache Durchlasskurve mit geringer Dämpfung und Plateau im Durchlassbereich sowie gute Bandbreite

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]
* a: *überkritische Kopplung* $\rightarrow$ starke gegenseitige Beeinflussung, Änderung der Resonanzfrequenzen, große Bandbreite und Verzerrung der Durchlasskurve im Durchlassbereich mit "Dellen"

---
[question:AD227]
---
[question:AD228]
---
[question:AD229]
