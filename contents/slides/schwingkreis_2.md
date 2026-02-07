## Grenzfrequenz

Bei Hoch- und Tiefpässen gilt für die Grenzfrequenz

<left>
Bei RL-Gliedern
$R = X_L$
$f_g = \frac{R}{2 \cdot \pi \cdot L}$
</left>
<right>
Bei RC-Gliedern
$R = X_C$
$f_g = \frac{1}{2 \cdot \pi \cdot R \cdot C}$
</right>


---
[question:AD201]
---
#### Lösungsweg
* gegeben: $R = 4,7kΩ$
* gegeben: $C = 2,2nF$
* gesucht: $f_g$

<fragment>
$f_g = \frac{1}{2 \cdot \pi \cdot R \cdot C} = \frac{1}{2 \cdot \pi \cdot 4,7kΩ \cdot 2,2nF} = 15,4kHz$
</fragment>
---
[question:AD202]
---
#### Lösungsweg
* gegeben: $R = 10kΩ$
* gegeben: $C = 47nF$
* gesucht: $f_g$

<fragment>
$f_g = \frac{1}{2 \cdot \pi \cdot R \cdot C} = \frac{1}{2 \cdot \pi \cdot 10kΩ \cdot 47nF} = 339Hz$
</fragment>
---
[question:AD203]
---
#### Lösungsweg
* gegeben: $R_1 = 4,7kΩ$
* gegeben: $C_1 = 6,8nF$
* gesucht: $f_g$

<fragment>
$C_2$ und alle weiteren Angaben sind für den Tiefpass uninteressant.
</fragment>

<fragment>
$f_g = \frac{1}{2 \cdot \pi \cdot R_1 \cdot C_1} = \frac{1}{2 \cdot \pi \cdot 4,7kΩ \cdot 6,8nF} \approx 5kHz$
</fragment>
---
## Resonanzfrequenz

* Parallel- oder Reihenschaltung von Spule und Kondensator &rarr; Schwingkreis
* Hohe Frequenzen &rarr; hoher Widerstand an Spule
* Niedrige Frequenzen &rarr; hoher Widerstand an Kondensator
* Es gibt eine Frequenz, bei der Spule und Kondensator den gleichen Widerstand haben &rarr; *Resonanzfrequenz*

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
* Theoretisch ist die Impedanz bei Resonanzfrequenz 0Ω
* Praktisch wird die Impedanz durch den ohmschen Widerstand bestimmt
* Bei Frequenzen über und unter der Resonanzfrequenz hat der Reihenschwingkreis eine höhere Impedanz

---
[question:AD207]
---
[question:AD204]
---
## Resonanzfall

Für Parallel- und Reihenschwingkreis:

$X_C = X_L$

Impedanzen sind gleich groß.

<fragment>
Resonanzfrequenz mit Thomson'sche Schwingkreisformel:

$f_0 = \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}$
</fragment>

<note>
William Thomson, später Lord Kelvin, in 1853
</note>
---


[question:AD208]
---
#### Lösungsweg
* gegeben: $L = 1,2µH$
* gegeben: $C = 6,8pF$
* gegeben: $R = 10Ω$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{1,2µH \cdot 6,8pF}} = 55,7MHz \end{split}$
</fragment>
<fragment>
Widerstand $R$ wird zur Berechnung nicht benötigt.
</fragment>
---
[question:AD209]
---
#### Lösungsweg
* gegeben: $L = 10µH$
* gegeben: $C = 1nF$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{10µH \cdot 1nF}} = 1,592MHz \end{split}$
</fragment>
---
[question:AD210]
---
#### Lösungsweg
* gegeben: $L = 100µH$
* gegeben: $C = 0,01µF$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{100µH \cdot 0,01µF}} = 159kHz \end{split}$
</fragment>
---
[question:AD211]
---
#### Lösungsweg
* gegeben: $L = 2,2µH$
* gegeben: $C = 56pF$
* gesucht: $f_0$

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{2,2µH \cdot 56pF}} = 14,34MHz \end{split}$
</fragment>
---
[question:AD212]
--- style="font-size: 0.7em;"
#### Lösungsweg
* gegeben: $C_1 = 0,1nF$
* gegeben: $C_2 = 1,5nF$
* gegeben: $C_3 = 220pF$
* gegeben: $L = 1,2mH$
* gesucht: $f_0$

<fragment>
$C = C_1 + C_2 + C_3 = 0,1nF + 1,5nF + 220pF = 1,82nF$
</fragment>
<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{1,2mH \cdot 1,82nF}} = 107,7kHz \end{split}$
</fragment>
---
### Verändern der Resonanzfrequenz

* Größere Spule oder Kondensator &rarr; kleinere Resonanzfrequenz
* Kleinere Spule oder Kondensator &rarr; größere Resonanzfrequenz

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
* Kleinere Spannung am Varicap &rarr; kleinere Grenzschicht im Varicap &rarr; größere Kapazität
* In Reihe geschaltete Kondensatoren &rarr; Kapazität steigt &rarr; Resonanzfrequenz fällt

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
* Z.B. *Bandbreite* bei *-3dB-Wert*
* Halbe Leistung eines Signals kann noch das Filter passieren
* Oder die 0,7-fache Signalspannung

---
[question:AD219]
---
[question:AD220]
---
### Übliche Bandbreiten

* Schmalbandig mit 500 Hz für Telegrafie (CW)
* Breitbandig mit 2,7 kHz für Sprachmodulation (SSB)

---
[question:AD221]
---
[question:AD222]
---
## Güte eines Schwingkreises

* Auch Q-Faktor
* Kennzeichen für Energieverlust
* Verhältnis der Blindwiderstände zum ohmschen Widerstand im Resonanzfall ($X_L = X_C$)

<fragment>
<left>
Reihenschwingkreis
$Q = \frac{f_0}{B} = \frac{X_L}{R_S}$
</left>
<right>
Parallelschwingkreis
$Q = \frac{f_0}{B} = \frac{R_P}{X_L}$
</right>
</fragment>
  
---
[question:AD225]
--- style="font-size: 0.7em;"
#### Lösungsweg
<left>
* gegeben: $L = 100µH$
* gegeben: $C = 0,01µF$
</left>
<right>
* gegeben: $R_S = 10Ω$
* gesucht: $Q$
</right>

<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{100µH \cdot 0,01µF}} = 159,2kHz \end{split}$
</fragment>
<fragment>
$B$ oder $X_L$ ausrechnen
$\begin{split} X_L &= \omega \cdot L = 2 \cdot \pi \cdot f_0 \cdot L\\ &= 2 \cdot \pi \cdot 159,2kHz \cdot 100µH = 100,03Ω \end{split}$
</fragment>
<fragment>
$Q = \frac{X_L}{R_S} = \frac{100,03Ω}{10Ω} \approx 10$
</fragment>
---
[question:AD226]
--- style="font-size: 0.7em;"
#### Lösungsweg
<left>
* gegeben: $L = 2,2µH$
* gegeben: $C = 56pF$
</left>
<right>
* gegeben: $R_P = 1kΩ$
* gesucht: $Q$
</right>
  
<fragment>
$\begin{split} f_0 &= \frac{1}{2 \cdot \pi \cdot \sqrt{L \cdot C}}\\ &= \frac{1}{2 \cdot \pi \cdot \sqrt{2,2µH \cdot 56pF}} = 14,34MHz \end{split}$
</fragment>
<fragment>
$B$ oder $X_L$ ausrechnen
$\begin{split} X_L &= \omega \cdot L = 2 \cdot \pi \cdot f_0 \cdot L\\ &= 2 \cdot \pi \cdot 14,34MHz \cdot 2,2µH = 198,2Ω \end{split}$
</fragment>
<fragment>
$Q = \frac{R_P}{X_L} = \frac{1kΩ}{198,2Ω} \approx 5$
</fragment>
---
### Bandbreite berechnen

Über Resonanzfrequenz und Güte

$Q = \frac{f_0}{B} \Rightarrow B = \frac{f_0}{Q}$

<fragment>
Oder eingesetzt mit der Thomson'schen Schwingkreisformel

<left>
Reihenschwingkreis
$B = \frac{R_S}{2\cdot \pi \cdot L}$
</left>
<right>
Parallelschwingkreis
$B = \frac{1}{2\cdot \pi \cdot R_P \cdot C}$
</right>
</fragment>
<note>
Herleitung nicht gezeigt
</note>

---
[question:AD224]
---
#### Lösungsweg
* gegeben: $L = 2,2µH$
* gegeben: $C = 56pF$
* gegeben: $R_P = 1kΩ$
* gesucht: $B$

<fragment>
$\begin{split} B &= \frac{1}{2\cdot \pi \cdot R_P \cdot C}\\ &= \frac{1}{2\cdot \pi \cdot 1kΩ \cdot 56pF} = 2,84MHz \end{split}$
</fragment>

---
[question:AD223]
---
#### Lösungsweg
* gegeben: $L = 100µH$
* gegeben: $C = 0,01µF$
* gegeben: $R_S = 10Ω$
* gesucht: $B$

<fragment>
$B = \frac{R_S}{2\cdot \pi \cdot L} = \frac{10Ω}{2\cdot \pi \cdot 100µH} = 15,9kHz$
</fragment>
--- style="font-size: 0.7em;" data-transition="none"
## Kopplung

[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* Zwischen Schaltungsstufen oder Filtern werden häufig gekoppelte Schwingkreise verwendet
* Zwei Schwingkreise induktiv oder kapazitiv aneinander gekoppelt
* Grad der Kopplung bestimmt die gegenseitige Beeinflussung, Bandbreite und Durchlasskurve

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* d: *lose Kopplung* &rarr; kaum gegenseitige Beeinflussung, sehr hohe Durchlassdämpfung und sehr geringe Bandbreite
* c: *unterkritische Kopplung* &rarr; kaum gegenseitige Beeinflussung, hohe Durchlassdämpfung und geringe Bandbreite

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]

* b: *kritische Kopplung* &rarr; etwas gegenseitige Beeinflussung, flache Durchlasskurve mit geringer Dämpfung und Plateau im Durchlassbereich sowie gute Bandbreite

--- style="font-size: 0.7em;" data-transition="none"
[picture:184:a_schwingkreis_kopplung:Induktive Kopplung zweier Schwingkreise und das Spannungsdiagramm über die Frequenz]
* a: *überkritische Kopplung* &rarr; starke gegenseitige Beeinflussung, Änderung der Resonanzfrequenzen, große Bandbreite und Verzerrung der Durchlasskurve im Durchlassbereich mit "Dellen"

---
[question:AD227]
---
[question:AD228]
---
[question:AD229]
