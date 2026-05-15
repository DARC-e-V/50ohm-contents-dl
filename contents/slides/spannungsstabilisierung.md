* Eingangsspannung kann variieren
* Beispielsweise bei durch Akku betriebenen Geräten
* Empfindliche Baugruppen (z.B. Oszillatoren) würden die Frequenz ändern
* Abhilfe: Spannungsstabilisierung

---
## Stabilisierung mit Z-Diode
<left>
[picture:323:a_Stabilisierung mit Z-Diode:Spannungsstabilisierung mit Z-Diode]
</left>
<right>
* Sehr einfache Schaltung
* Kann die Ausgangsspannung in Grenzen stabil halten
</right>
<note>
</note>
---
[question:AD321]
--- style="font-size: 0.7em;"
#### Lösungsweg
* gegeben: $R_\text{L} = \qty{470}{\ohm}$
* gegeben: $I_\text{L} = \qty{10}{\milli\ampere}$
* gegeben: $I_\text{Z} = \qty{15}{\milli\ampere}$
* gegeben: $U_{\mathrm{in}} = \qty{13,8}{\volt}$
* gesucht: $\eta = \frac{P_\text{L}}{P_{\mathrm{in}}}$

<fragment>
$P_\text{L} = I_\text{L}^2 \cdot R_\text{L} = (\qty{10}{\milli\ampere})^2 \cdot \qty{470}{\ohm} = \qty{47}{\milli\watt}$
</fragment>
<fragment>
$P_{\mathrm{in}} = U_{\mathrm{in}} \cdot I_{\mathrm{in}} = U_{\mathrm{in}} \cdot (I_\text{Z} + I_\text{L}) = \qty{13,8}{\volt} \cdot (\qty{15}{\milli\ampere} + \qty{10}{\milli\ampere}) = \qty{345}{\milli\watt}$
</fragment>
<fragment>
$\eta = \frac{P_\text{L}}{P_{\mathrm{in}}} = \frac{\qty{47}{\milli\watt}}{\qty{345}{\milli\watt}} \approx \num{0,14}$
</fragment>
---
## Linarer Spannungsregler

<left>
[picture:985:a_spannungsregler_linear:Schaltbild eines linearen Spannungsreglers]
</left>
<right>
* Leistungstransistor wird als veränderlicher Widerstand betrieben
* Bildet zusammen mit dem Lastwiderstand einen Spannungsteiler
* Wirkungsgrad ist oft sehr niedrig
</right>

---
[question:AD315]
---
[question:AD319]
---
#### Lösungsweg
* gegeben: $U_{\mathrm{in}} = \qty{13,8}{\volt}$
* gegeben: $U_{\mathrm{out}} = \qty{9}{\volt}$
* gegeben: $I = \qty{900}{\milli\ampere}$
* gesucht: $P_\text{V}$

<fragment>
$U_{IC1} = U_{\mathrm{in}} - U_{\mathrm{out}} = \qty{13,8}{\volt} - \qty{9}{\volt} = \qty{4,8}{\volt}$
</fragment>
<fragment>
$P_\text{V} = U_{IC1} \cdot I = \qty{4,8}{\volt} \cdot \qty{900}{\milli\ampere} = \qty{4,32}{\watt}$
</fragment>
---
[question:AD320]
---
#### Lösungsweg
* gegeben: $U_{\mathrm{in}} = \qty{13,8}{\volt}$
* gegeben: $U_{\mathrm{out}} = \qty{5}{\volt}$
* gegeben: $I_{\mathrm{in}} = \qty{455}{\milli\ampere}$
* gegeben: $I_{\mathrm{out}} = \qty{450}{\milli\ampere}$
* gesucht: $\eta$

<fragment>
$\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} = \frac{U_{\mathrm{out}} \cdot I_{\mathrm{out}}}{U_{\mathrm{in}} \cdot I_{\mathrm{in}}} = \frac{\qty{5}{\volt} \cdot \qty{450}{\milli\ampere}}{\qty{13,8}{\volt} \cdot \qty{455}{\milli\ampere}} \approx \num{0,36}$
</fragment>
---
## Festspannungsregler
<left>
[picture:200:a_Festspannungsregler:Festspannungsregler]
</left>
<right>
* Ausgelegt als IC
* Arbeiten wie linare Spannungsregler mit sehr genauer Spannungsreferenzquelle und optimaler elektronischer Regelung
* Auch bei starker Schwankung auf der Eingangsseite ist die Ausgangsseite sehr stabil
</right>

---
[question:AD317]
---
[question:AD316]
---
[question:AD318]
---
#### Lösungsweg
* gegeben: $U_{\mathrm{in}} = \qty{13,8}{\volt}$
* gegeben: $U_{\mathrm{out}} = \qty{5}{\volt}$
* gegeben: $R_\text{L} = \qty{10}{\ohm}$
* gesucht: $P_\text{V}$

<fragment>
$I = \frac{U_{\mathrm{in}}}{R_\text{L}} = \frac{\qty{5}{\volt}}{\qty{10}{\ohm}} = \qty{500}{\milli\ampere}$
</fragment>
<fragment>
$U_\text{IC1} = U_{\mathrm{in}} - U_{\mathrm{out}} = \qty{13,8}{\volt} - \qty{5}{\volt} = \qty{8,8}{\volt}$
</fragment>
<fragment>
$P_\text{V} = U_\text{IC1} \cdot I = \qty{8,8}{\volt} \cdot \qty{500}{\milli\ampere} = \qty{4,4}{\watt}$
</fragment>
