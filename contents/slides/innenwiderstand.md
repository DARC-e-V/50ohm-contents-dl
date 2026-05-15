### Spannungsquelle
<left>
[picture:1018:a_vsource_schematic:Ersatzschaltbild Spannungsquelle]
</left>
<right>
* Reale Spannungsquelle wird mit $R_\text{L}$ belastet $\rightarrow$ Klemmenspannung $U_\text{k}$ sinkt
* Grund ist der Innenwiderstand
* Ohne Belastung / im Leerlauf: $U_\text{q} = U_\text{L}$
</right>
<note>
</note>

---
### Innenwiderstand

<left>
* Nicht messbar mit einem Multimeter
* Rechnerisch ermitteln: <br/>$R_\text{i} = \frac{\Delta U}{\Delta I}$
</left>
<right>
* Leerlauf: $I = \qty{0}{\ampere}$
* Belastung mit $R_\text{L}$: <br/>$I_\text{L} = \frac{U_\text{L}}{R_\text{L}}$
</right>

---
### Innenwiderstand Spannungsquelle

$(\Delta U = \qty{0}{\volt})$;  $R_\text{i} = \frac{\Delta U}{\Delta I} = \frac{0}{x} = \qty{0}{\ohm}$

<fragment>
Ideale Spannungsquellen sollen einen sehr niedrigen Innenwiderstand $R_\text{i} \ll R_\text{L}$ aufweisen

Idealfall: $\qty{0}{\ohm}$, dann bleibt die Ausgangsspannung bei Belastung unverändert.
</fragment>

---

### Strombegrenzung

* In Labornetzteilen eingebaut
* Laststrom übersteigt eine maximale Stromstärke
* $\rightarrow$ Klemmenspannung wird abgesenkt
* $\rightarrow$ Laststrom bleibt konstant
* Funktion der Konstantstromquelle

---
### Innenwiderstand Stromquelle

$R_\text{i} = \frac{\Delta U}{\Delta I}$; $(\Delta I \to \qty{0}{\ampere})$;  $R_\text{i} = \frac{\Delta U}{\Delta I} \to \qty{\infty}{\ohm}$

<fragment>
Ideale Stromquellen sollen einen sehr hohen Innenwiderstand $R_\text{i} \gg R_\text{L}$ aufweisen.

Idealfall: $\qty{\infty}{\ohm}$, dann bleibt der Laststrom bei Änderung des  Lastwiderstandes konstant, deshalb spricht man auch von Stromanpassung.
</fragment>

---
[question:AB201]
---
### Leistungsanpassung

* Optimale Leistungsabgabe von Sender zu Antenne
* $R_\text{i} = R_\text{L}$

--- style="font-size: 0.7em;"

|c: Zusammenfassung Innenwiderstand | c: Innenwiderstand |
| Spannungsanpassung bei einer Konstantspannungsquelle| $R_\text{i}$ ist sehr niederohmig; theoretisch $\qty{0}{\ohm}$; $R_\text{i} \ll R_\text{L}$ identisch mit $R_\text{L} \gg R_\text{i}$|
|Stromanpassung bei einer Konstantstromquelle|$R_\text{i}$ ist sehr hochohmig; $R_\text{i} \gg R_\text{L}$ identisch mit $R_\text{L} \ll R_\text{i}$ |
| Leistungsanpassung bei Verstärkern| $R_\text{L} = R_\text{i}$|
[table:a_Innenwiderstand Zusammenfassung:Zusammenfassung zum Innenwiderstand]

---
[question:AG401]
---
[question:AB202]
---
[question:AB203]
---
[question:AB204]
---
[question:AB207]
---
#### Lösungsweg
* gegeben: $U_0 = \qty{13,5}{\volt}$
* gegeben: $U_\text{Kl} = \qty{13}{\volt}$
* gegeben: $I = \qty{2}{\ampere}$
* gesucht: $R_\text{i}$

<fragment>
$R_\text{i} = \frac{U_\text{i}}{I} = \frac{U_0-U_\text{Kl}}{I} = \frac{\qty{13,5}{\volt} - \qty{13}{\volt}}{\qty{2}{\ampere}} = \qty{0,25}{\ohm}$
</fragment>
---
[question:AB208]
---
#### Lösungsweg
* gegeben: $U_0 = \qty{13,8}{\volt}$
* gegeben: $U_\text{Kl} = \qty{13,6}{\volt}$
* gegeben: $I = \qty{20}{\ampere}$
* gesucht: $R_\text{i}$

<fragment>
$R_\text{i} = \frac{U_\text{i}}{I} = \frac{U_0-U_\text{Kl}}{I} = \frac{\qty{13,8}{\volt} - \qty{13,6}{\volt}}{\qty{20}{\ampere}} = \qty{10}{\milli\ohm}$
</fragment>
---
[question:AB206]
---
#### Lösungsweg
* gegeben: $U_0 = \qty{13,5}{\volt}$
* gegeben: $U_\text{Kl} = \qty{12,4}{\volt}$
* gegeben: $I = \qty{0,9}{\ampere}$
* gesucht: $R_\text{i}$

<fragment>
$R_\text{i} = \frac{U_\text{i}}{I} = \frac{U_0-U_\text{Kl}}{I} = \frac{\qty{13,5}{\volt} - \qty{12,4}{\volt}}{\qty{0,9}{\ampere}} = \qty{1,22}{\ohm}$
</fragment>
---
[question:AB205]
---
#### Lösungsweg
* gegeben: $U_0 = \qty{5,0}{\volt}$
* gegeben: $U_\text{Kl} = \qty{4,8}{\volt}$
* gegeben: $R_\text{L} = \qty{1,2}{\ohm}$
* gesucht: $R_\text{i}$

<fragment>
$I = \frac{U_\text{Kl}}{R_\text{L}} = \frac{\qty{4,8}{\volt}}{\qty{1,2}{\ohm}} = \qty{4}{\ampere}$
</fragment>
<fragment>
$R_\text{i} = \frac{U_\text{i}}{I} = \frac{U_0 - U_\text{Kl}}{I} = \frac{\qty{5,0}{\volt} - \qty{4,8}{\volt}}{\qty{4}{\ampere}} = \qty{0,05}{\ohm}$
</fragment>

