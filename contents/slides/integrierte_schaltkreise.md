* *Integrated Circuit (IC)*: Integrierte Schaltungen
* Komplexe Schaltung auf einem Halbleitersubstrat
* Erleichtern den Aufbau von elektronischen Schaltungen

---
[question:AC601]
---
## Monolithic Microwave Integrated Circuit (MMIC)

* Breitbandiger Verstärker mit wenigen Bauteilen
* Typischerweise $\qty{50}{\ohm}$ Ein- und Ausgangsimpedanz
* Vereint aktive und passive Bauelemente

---
[question:AC602]
---
[question:AC603]
---
[question:AC604]
---
### MMIC Beschaltung

<left>
[picture:773:a_mmic:MMIC-Schaltung]
</left>
<right>
* Arbeitspunkt wird über $R_{\textrm{BIAS}}$ eingestellt
* Kondensatoren isolieren Gleichspannung
* Anschluss 2 und 4 liegen auf Masse gegenüber $U_{\textrm{CC}}$
* Anschluss 1 ist offen
* $U_{\textrm{CC}}$ fällt über $R_{\textrm{BIAS}}$ und MMIC ab
</right>
<note>
</note>

---
[question:AF425]
---
#### Lösungsweg
* gegeben: $U_{\textrm{D}} = \qty{4}{\volt}$
* gegeben: $U_{\textrm{CC}} = \qty{13,5}{\volt}$
* gegeben: $I_{\textrm{D}} = \qty{10}{\milli\ampere}$
* gesucht: $R_{\textrm{BIAS}}$

<fragment>
$R_{\textrm{BIAS}} = \frac{U_{\textrm{CC}} - U_{\textrm{D}}}{I_{\textrm{D}}} = \frac{\qty{13,5}{\volt} - \qty{4}{\volt}}{\qty{10}{\milli\ampere}} = \qty{950}{\ohm}$
</fragment>

---
[question:AF426]
---
#### Lösungsweg
* gegeben: $U_{\textrm{D}} = \qty{4}{\volt}$
* gegeben: $U_{\textrm{CC}} = \qty{13,8}{\volt}$
* gegeben: $I_{\textrm{D}} = \qty{15}{\milli\ampere}$
* gesucht: $R_{\textrm{BIAS}}$

<fragment>
$R_{\textrm{BIAS}} = \frac{U_{\textrm{CC}} - U_{\textrm{D}}}{I_{\textrm{D}}} = \frac{\qty{13,8}{\volt} - \qty{4}{\volt}}{\qty{15}{\milli\ampere}} = \qty{653,3}{\ohm} \rightarrow \qty{680}{\ohm}$
</fragment>

---
[question:AF427]
---
#### Lösungsweg
* gegeben: $U = \qty{9}{\volt}$
* gegeben: $R_{\textrm{BIAS}} = \qty{470}{\ohm}$
* gegeben: $U_{\textrm{D}} = \qty{4}{\volt}$
* gesucht: $P$
* Ansatz: Strom durch $R_{\textrm{BIAS}}$ ist überall gleich, weil kein anderer ohmschmer Verbraucher in der Schaltung vorhanden ist

<fragment>
$I_{\textrm{D}} = \frac{U_{\textrm{BIAS}}}{R_{\textrm{BIAS}}} = \frac{U-U_{\textrm{D}}}{R_{\textrm{BIAS}}} = \frac{\qty{9}{\volt}-\qty{4}{\volt}}{\qty{470}{\ohm}} = \qty{10,64}{\milli\ampere}$
</fragment>
<fragment>
$P = U_{\textrm{D}} \cdot I_{\textrm{D}} = \qty{4}{\volt} \cdot \qty{10,64}{\milli\ampere} \approx \qty{43}{\milli\watt}$
</fragment>
