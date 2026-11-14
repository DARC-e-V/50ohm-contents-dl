## Leistungsberechnung

<left>
* Bekannt aus Klasse N: $P = U \cdot I$
* Mit dem ohmschen Gesetz ($U = R \cdot I$) umstellen:
  * $P = \dfrac{U^2}{R}$
  * $P = I^2 \cdot R$
</left>
<right>
[picture:1013:e_leistung_r:Leistung wird am Widerstand $R$ in Wärme umgesetzt]
</right>

<note>
* Alle hergeleiteten Formeln stehen in der Formelsammlung (https://50ohm.de/hm)
</note>

---
## Herleitung $U = \sqrt{P \cdot R}$

$I = \dfrac{U}{R}$ in $P = U \cdot I$ einsetzen:

<fragment>
$P = \dfrac{U^2}{R} \quad\Rightarrow\quad U^2 = P \cdot R \quad\Rightarrow\quad U = \sqrt{P \cdot R}$
</fragment>

<fragment>
Für den Strom analog aus $P = I^2 \cdot R$: $\quad I = \sqrt{\dfrac{P}{R}}$
</fragment>

---
## Umgestellte Formeln

* Spannung: $U = \sqrt{P \cdot R}$
* Strom: $I = \sqrt{\dfrac{P}{R}}$
* Widerstand: $R = \dfrac{U^2}{P} = \dfrac{P}{I^2}$

---
[question:EB504]
---
[question:EB505]
---
[question:EB506]
---
## Leistung bei Wechselspannung

* Dieselben Formeln gelten, mit den *Effektivwerten* von $U$ und $I$
* $U_\text{eff} = \dfrac{\hat{U}}{\sqrt{2}}$

---
[question:EB503]
---
[question:EB507]
---
### Lösungsweg EB507

$P = \dfrac{U^2}{R} = \dfrac{(\qty{100}{\volt})^2}{\qty{50}{\ohm}} = \qty{200}{\watt}$

---
[question:EB508]
---
### Lösungsweg EB508

$P = I^2 \cdot R = (\qty{2}{\ampere})^2 \cdot \qty{50}{\ohm} = \qty{200}{\watt}$

---
[question:EB509]
---
### Lösungsweg EB509

$P = \dfrac{U^2}{R} = \dfrac{(\qty{10}{\volt})^2}{\qty{100}{\ohm}} = \qty{1}{\watt}$

---
[question:EB510]
---
### Lösungsweg EB510

* Zuerst wird die Leistungsgrenze erreicht, nicht die Spannungsfestigkeit

$U = \sqrt{P \cdot R} = \sqrt{\qty{1}{\watt} \cdot \qty{10000}{\ohm}} = \qty{100}{\volt}$

---
[question:EB511]
---
### Lösungsweg EB511

$U = \sqrt{P \cdot R} = \sqrt{\qty{6}{\watt} \cdot \qty{100000}{\ohm}} \approx \qty{775}{\volt}$

---
[question:EB512]
---
### Lösungsweg EB512

$I = \sqrt{\dfrac{P}{R}} = \sqrt{\dfrac{\qty{23}{\watt}}{\qty{120}{\ohm}}} \approx \qty{438}{\milli\ampere}$

---
[question:EB513]

<note>
* Hier nur ohmsches Gesetz, keine Leistungsberechnung – die Frage passte in Klasse E nirgends anders
</note>
---
### Lösungsweg EB513

$\hat{U} = \dfrac{U_\text{SS}}{2} = \qty{12,5}{\volt}$, dann $U_\text{eff} = \dfrac{\hat{U}}{\sqrt{2}} \approx \qty{8,84}{\volt}$

$I_\text{eff} = \dfrac{U_\text{eff}}{R} = \dfrac{\qty{8,84}{\volt}}{\qty{1000}{\ohm}} \approx \qty{8,8}{\milli\ampere}$

---
## Dummyload aus 11 Widerständen

<left>
* 11 gleiche Widerstände parallel
* Jeder Widerstand trägt $1/11$ der Gesamtleistung
* Zulässige Gesamtleistung $= 11 \cdot$ Einzelbelastbarkeit
* Beispiel: $11 \cdot \qty{5}{\watt} = \qty{55}{\watt}$
</left>
<right>
[picture:1014:e_dummyload_11:Dummyload aus 11 gleich großen Widerständen]
</right>

---
[question:EB514]
