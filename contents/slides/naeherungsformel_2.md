## Sicherheitsabstand: Fernfeldberechnung (ohne Kabeldämpfung)

* Bei ortsfesten Amateurfunkanlagen wird der Sicherheitsabstand mittels Fernfeldformel ermittelt

<fragment>
$d=\dfrac{\sqrt{30\,\Omega\cdot P_A\cdot G_i}}{E}$
</fragment>

--- style="font-size: 0.7em;"
#### Zusatzinformation zu Modulationsverfahren in der Sicherheitsabstandberechnung

* Bei der Anzeige einer ortsfesten Amateurfunkanlage (nach § 9, BEMFV) muss der Umrechnungsfaktor $\textrm{Faktor}_\textrm{FmodPers}$ eingetragen werden
* Dieser Faktor wandelt die angegebene Spitzenleistung (PEP) in die mittlere Leistung um, welche in der Fernfeldformel zur Berechnung des Sicherheitsabstands verwendet wird
* Die meisten Modulationsverfahren haben hierbei den Faktor 1
* ATV: Faktor 0,38

<note>
DIN EN 50413, für Amateurfunk relevant nur ATV mit 0,38 und SATV mit 0,54
</note>

---

[question:AK106]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $P_S = P_A = 100W$
</left>
<right>
* gegeben: $G_i = 1,64$
* gesucht: $d$
</right>

<fragment>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_A \cdot G_i}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_A \cdot G_i}}{E}\\ &= \frac{\sqrt{30Ω \cdot 100W \cdot 1,64}}{28\frac{V}{m}}\\ &= 2,5m\end{split}$
</fragment>

---
## Sicherheitsabstand: Berücksichtigung der Kabeldämpfung
* Zuerst wird die effektive isotrope Strahlungsleistung (ERIP) berechnet  

<fragment>
$P_\text{EIRP} = P_S\cdot10^{\frac{g_d - a + 2,15}{10}}$
</fragment>

---

[question:AK108]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $P_S = 300W$
* gegeben: $a = 0,5dB$
</left>
<right>
* gegeben: $g_d = 0dBd$
* gesucht: $d$
</right>

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d -a + 2,15dB}{10dB}}\\ &= 300W \cdot 10^{\frac{0dBd - 0,5dB + 2,15dB}{10dB}}\\ &= 438,7W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{E}\\ &= \frac{\sqrt{30Ω \cdot 438,7W}}{28\frac{V}{m}}\\ &= 4,10m\end{split}$
</right>
</fragment>

---

[question:AK109]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $P_S = 700W$
* gegeben: $a = 0,5dB$
</left>
<right>
* gegeben: $g_d = 0dBd$
* gesucht: $d$
</right>

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d -a + 2,15dB}{10dB}}\\ &= 700W \cdot 10^{\frac{0dBd - 0,5dB + 2,15dB}{10dB}}\\ &= 1023,5W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{E}\\ &= \frac{\sqrt{30Ω \cdot 1023,5W}}{28\frac{V}{m}}\\ &= 6,26m\end{split}$
</right>
</fragment>

---

[question:AK110]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $P_S = 75W$
* gegeben: $a = 1,5dB$
</left>
<right>
* gegeben: $g_d = 11,5dBd$
* gesucht: $d$
</right>

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d -a + 2,15dB}{10dB}}\\ &= 75W \cdot 10^{\frac{11,5dBd - 1,5dB + 2,15dB}{10dB}}\\ &= 1230,4W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{E}\\ &= \frac{\sqrt{30Ω \cdot 1230,4W}}{28\frac{V}{m}}\\ &= 6,86m\end{split}$
</right>
</fragment>

---

[question:AK111]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 28\frac{V}{m}$
* gegeben: $P_S = 100W$
* gegeben: $a = 1,5dB$
</left>
<right>
* gegeben: $g_d = 10,5dBd$
* gesucht: $d$
</right>

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d -a + 2,15dB}{10dB}}\\ &= 100W \cdot 10^{\frac{10,5dBd - 1,5dB + 2,15dB}{10dB}}\\ &= 1303,2W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{E}\\ &= \frac{\sqrt{30Ω \cdot 1303,2W}}{28\frac{V}{m}}\\ &= 7,1m\end{split}$
</right>
</fragment>

---

[question:AK112]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $E = 61\frac{V}{m}$
* gegeben: $P_S = 40W$
* gegeben: $a = 2dB$
</left>
<right>
* gegeben: $g_d = 18dBd$
* gesucht: $d$
</right>

<fragment>
<left>
$\begin{split}P_{EIRP} &= P_S \cdot 10^{\frac{g_d -a + 2,15dB}{10dB}}\\ &= 40W \cdot 10^{\frac{18dBd - 2dB + 2,15dB}{10dB}}\\ &= 2612,5W\end{split}$
</left>
</fragment>
<fragment>
<right>
$\begin{split}E &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{d}\\ \Rightarrow d &= \frac{\sqrt{30Ω \cdot P_{EIRP}}}{E}\\ &= \frac{\sqrt{30Ω \cdot 2612,5W}}{61\frac{V}{m}}\\ &= 4,6m\end{split}$
</right>
</fragment>
