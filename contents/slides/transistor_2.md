## Bipolarer Transistor


[picture:864:a_bauelemente_bipolartransistor:Schaltbild eines npn- und pnp-Bipolartransistors mit Kollektor (C), Basis (B) und Emitter (E)]

* Drei Halbleiterzonen
* Abwechselnd n- und p-dotiert
* npn-Transistor und pnp-Transistor

---
[question:AC503]
---
[question:AC504]
---
### Stromsteuerung und Faktor

* Basis-Emitter-Spannung $U_{\textrm{BE}}$ steuert Kollektorstrom $I_{\textrm{C}}$ exponentiell
* Beim Bipolartransistor fließt immer ein exponentiell von $U_{\textrm{BE}}$ abhängiger Basisstrom $I_{\textrm{B}}$
* Faktor $B$ ist der *Stromverstärkungsfaktor* des Transistors
* Liegt bei ca. 20 bis 500

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}}$
</fragment>

<note>
Höherer Faktor benötigt kleineren Basistrom zur Steuerung eines größeren Kollektorstroms
</note>
---
[question:AC501]
---
### Leitender Bipolartransistor

* Signifikanter Kollektorstrom fließt
* Basis-Emitter-Diode in Durchlassrichtung
* Kollektor-Basis-Diode sperrt, damit keine Ladungsträger aus dem Kollektor in die Basis gelangen

---
[question:AC505]
---
### Rechnungen

---
[question:AC515]
---
#### Lösungsweg
* Die Größe von $R_1$ stellt den Basisstrom $I_B$ ein
* $I_B$ ist um 298 kleiner als $I_C$
* Für die Spannung an $R_1$ muss der Transistorverlust abgezogen werden

---
* gegeben: $U = \qty{12}{\volt}$
* gegeben: $I_{\textrm{C}} = \qty{5}{\milli\ampere}$
* gegeben: $B = 298$
* gegeben: $U_{\textrm{BE}} = \qty{0,6}{\volt}$
* gesucht: $R_1$

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{5}{\milli\ampere}}{298} = \qty{16,779}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U-U_{\textrm{BE}}}{I_{\textrm{B}}} = \frac{\qty{12}{\volt} - \qty{0,6}{\volt}}{\qty{16,779}{\micro\ampere}} \approx \qty{680}{\kilo\ohm}$
</fragment>

<note>
Nachteil der Schaltung ist eine schlecht kontrollierte Stromverstärkung
</note>
---
[question:AC518]
---
### Arbeitspunktstabilisation

<left>
[picture:361:a_bauteile_arbeitspunkteinstellung:Transistorschaltung mit Basisspannungsteiler]
</left>
<right>
* Arbeitspunkt wird über den Spannungsteiler eingestellt
* Querstrom durch $R_2$ soll so hoch sein, damit der Basisstrom keinen großen Einfluss auf den Arbeitspunkt hat
</right>
<note>
Kollektorstrom hängt exponentiell von der Basis-Emitter-Spannung ab; Toleranz der Widerstände kann große Auswirkungen auf den Kollektorstrom haben. Starke Temperaturabhängigkeit im Transistor kann Kollektorstrom beeinflussen.
</note>

---
[question:AC516]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $U = \qty{10}{\volt}$
* gegeben: $I_{\textrm{C}} = \qty{2}{\milli\ampere}$
* gegeben: $B = 200$
</left>
<right>
* gegeben: $U_{\textrm{R2}} = \qty{0,6}{\volt}$
* gegeben: $I_{\textrm{R2}} = 10 \cdot I_{\textrm{B}}$
* gesucht: $R_1$
</right>

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere}$
</fragment>
<fragment>
$U_{\textrm{R1}} = U - U_{\textrm{R2}} = \qty{10}{\volt} - \qty{0,6}{\volt} = \qty{9,4}{\volt}$
</fragment>
<fragment>
$I_{\textrm{R1}} = I_{\textrm{B}} + I_{\textrm{R2}} = I_{\textrm{B}} + 10 \cdot I_{\textrm{B}} = \qty{110}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U_{\textrm{R1}}}{I_{\textrm{R1}}} = \frac{\qty{9,4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{85,5}{\kilo\ohm}$
</fragment>

---
[question:AC517]
---
#### Lösungsweg

* $U_{\textrm{R2}}$ ist gleich groß wie $U_{\textrm{BE}} + U_{\textrm{RE}}$
* Kollektorstrom wird vor allem durch $R_{\textrm{E}}$ festgelegt
* Sehr stabile Schaltung

--- style="font-size: smaller;"
<left>
* gegeben: $U = \qty{10}{\volt}$
* gegeben: $I_{\textrm{C}} = \qty{2}{\milli\ampere}$
* gegeben: $B = 200$
</left>
<right>
* gegeben: $U_{\textrm{BE}} = \qty{0,6}{\volt}$
* gegeben: $U_{\textrm{RE}} = \qty{1}{\volt}$
* gegeben: $I_{\textrm{R2}} = 10 \cdot I_{\textrm{B}}$
</right>
* gesucht: $R_1$

<fragment>
$B = \frac{I_{\textrm{C}}}{I_{\textrm{B}}} \Rightarrow I_{\textrm{B}} = \frac{I_{\textrm{C}}}{B} = \frac{\qty{2}{\milli\ampere}}{200} = \qty{10}{\micro\ampere}$
</fragment>
<fragment>
$U_{\textrm{R2}} = U_{\textrm{BE}} + U_{R_{\textrm{E}}} = \qty{0,6}{\volt} + \qty{1}{\volt} = \qty{1,6}{\volt}$
</fragment>
<fragment>
$U_{\textrm{R1}} = U - U_{\textrm{R2}} = \qty{10}{\volt} - \qty{1,6}{\volt} = \qty{8,4}{\volt}$
</fragment>
<fragment>
$I_{\textrm{R1}} = I_{\textrm{B}} + I_{\textrm{R2}} = I_{\textrm{B}} + 10 \cdot I_{\textrm{B}} = \qty{110}{\micro\ampere}$
</fragment>
<fragment>
$R_1 = \frac{U_{\textrm{R1}}}{I_{\textrm{R1}}} = \frac{\qty{8,4}{\volt}}{\qty{110}{\micro\ampere}} \approx \qty{76,4}{\kilo\ohm}$
</fragment>

---
[question:AC519]
---
#### Lösungsweg

* Kein Strom durch $R_1$ &rarr; keine Spannung über $R_2$
* Basis liegt auf Massepotential &rarr; Transistor ist stromlos
* Kein Spannungsabfall an $R_{\textrm{C}}$ &rarr; Kollektorpotential steigt auf Betriebsspannung

---
[question:AC520]
---
#### Lösungsweg

* $R_2$ ist stromlos &rarr; Basis ist über $R_1$ ist mit der Betriebsspannung verbunden
* Aufgrund der Dimensionierung ist der Basisstrom nun 11-fach höher als geplant
* Kollektorstrom wird stark ansteigen &rarr; Spannungsabfall an $R_{\textrm{C}}$ steigt stark
* $U_{\textrm{CE}}$ sinkt auf den Sättigungswert von ca. $\qty{0,1}{\volt}$

---
## Feldeffekttransistor (FET)

[picture:271:a_bauelemente_fet:Schaltbilder für Feldeffekttransistoren]

* Anderer Aufbau
* Es besteht ein Halbleiterkanal
* Der Stromfluss wird über ein elektrisches Feld gesteuert
* Dadurch spannungsgesteuert

<note>
Senkrechte Linie symbolisiert den Kanal, die Drain (oben) und Source (unten) kontaktiert; links ist das Gate und der Pfeil erinnert an eine Diode
</note>
---
[question:AC502]
---
[question:AC506]
---
### Anschlüsse des FET

* *Source* Quelle für die Ladungsträger im Kanal
* *Drain* Abfluss der Ladungsträger im Kanal
* *Gate* steuert den Fluss der Ladungsträger im Kanal

---
[question:AC513]
---
[question:AC512]
---
[question:AC514]

<note>
Besser wäre: steuert den Kanalstrom statt Widerstand, da dieses Widerstand-Verhalten nur bei kleinen Drain-Source-Spannungen auftritt
</note>
---
### Bauarten FET

* *selbstleitend*: Ohne Gate-Source-Spannung ist der FET leitend
* *selbstsperrend*: Ohne Gate-Source-Spannung ist der FET sperrend
* *n-Kanal-FET*: Strom im Kanal wird von Elektronen getragen
* *p-Kanal-FET*: Strom im Kanal wird von Löchern getragen
* *Sperrschicht-FET*: Gate ist eine Diode
* *Isolierschicht-FET*: Gate ist eine Kondensator-Struktur (z.B. MOSFET)

<note>
MOSFET: metal oxide semiconductor FET
</note>
---
### Schaltzeichen FET

<left>
[picture:273:a_bauelemente_selbstleitender_p_kanal_mosfet:Selbstleitender p-Kanal MOSFET]
[picture:276:a_bauelemente_selbstsperrender_n_kanal_mosfet:Selbstsperrender n-Kanal MOSFET]
</left>
<right>
* *selbstleitend*/*selbstsperrend*: Gate durchgehend/gestrichelt
* *n-*/*p-Kanal*: Pfeil zeigt weg von/hin zu Kanal
* *Isolierschicht* (MOSFET): Gate und Kanal als Kondensator
</right>

---
[question:AC507]
---
[question:AC508]
---
[question:AC509]
---
[question:AC510]
---
[question:AC511]
---
### Rechnungen

---
[question:AC521]
---
#### Lösungsweg

<left>
* gegeben: $U_{\textrm{B}} = \qty{44}{\volt}$
* gegeben: $R_1 = \qty{10}{\kilo\ohm}$
* gegeben: $R_2 = \qty{1}{\kilo\ohm}$
* gegeben: $R_3 = \qty{2,2}{\kilo\ohm}$
* gesucht: $U_{\textrm{GS}}$
* Ansatz: Unbelasteter Spannungsteiler über $R_1$ und $R_2$, mit $U_{\textrm{GS}} = U_{\textrm{R2}}$
</left>
<right>
<fragment>
$\begin{split} \frac{U_{\textrm{R2}}}{U_{\textrm{B}}} &= \frac{R_2}{R_1+R_2}\\ \Rightarrow U_{\textrm{R2}} &= \frac{R_2}{R_1+R_2} \cdot U_{\textrm{G}}\\ &= \frac{\qty{1}{\kilo\ohm}}{\qty{10}{\kilo\ohm}+\qty{1}{\kilo\ohm}} \cdot \qty{44}{\volt}\\ &= \frac{1}{11} \cdot \qty{44}{\volt} = \qty{4}{\volt} \end{split}$
</fragment>
</right>

---
[question:AC522]
---
#### Lösungsweg

<left>
* gegeben: $U_{\textrm{B}} = \qty{44}{\volt}$
* gegeben: $R_1 = \qty{10}{\kilo\ohm}$
* gegeben: $R_3 = \qty{2,2}{\kilo\ohm}$
* gegeben: $U_{\textrm{GS}} = U_{\textrm{R2}} = \qty{2,8}{\volt}$
* gegeben: $U_{\textrm{B}} = U_{\textrm{R1}} + U_{\textrm{R2}}$
* gesucht: $R_2$
</left>
<right>
<fragment>
$\begin{split} \frac{U_{\textrm{R1}}}{U_{\textrm{R2}}} &= \frac{R_1}{R_2}\\ \Rightarrow R_2 &= R_1 \cdot \frac{U_{\textrm{R2}}}{U_{\textrm{R1}}}\\ &= R_1 \cdot \frac{U_{\textrm{R2}}}{U_{\textrm{B}}-U_{\textrm{GS}}}\\ &= \qty{10}{\kilo\ohm} \cdot \frac{\qty{2,8}{\volt}}{\qty{44}{\volt}-\qty{2,8}{\volt}}\\ &\approx \qty{680}{\ohm} \end{split}$
</fragment>
</right>
---
[question:AC523]
---
#### Lösungsweg

* gegeben: $R_{\textrm{DSon}} = \qty{4}{\milli\ohm}$
* gegeben: $I = \qty{25}{\ampere}$
* gesucht: $P$

<fragment>
$P = I^2 \cdot R = (\qty{25}{\ampere})^2 \cdot \qty{4}{\milli\ohm} = \qty{2,5}{\watt}$
</fragment>

<note>
MOSFET verhält sich wie ein ohmscher Widerstand
</note>

---
### Freilaufdiode

* Relais wird über einen in Serie geschalteten Bipolartransistor betrieben
* Transistor schaltet ein &rarr; Strom fließt durch die Relaisspule
* Transistor schaltet ab &rarr; Strom in der Spule induziert negative Spannung am Transistor
* Kann zur Zerstörung des Transistors führen
* Verhindern: *Freilaufdiode* parallel zum Relais in Sperrichtung verbauen
* Induktionsspannung wird auf Diodenspannung begrenzt

---
[question:AC524]