## Spannungsteiler

<left>
* Reihenschaltung aus zwei Widerständen
* Klasse E: nur der *unbelastete* Spannungsteiler
* Spannungen verhalten sich proportional zu den Widerständen
* Hochohmiger Widerstand $\rightarrow$ größere Teilspannung, niederohmiger $\rightarrow$ kleinere
</left>
<right>
[picture:819:e_spannungsteiler:Spannungsteiler aus zwei Widerständen]
</right>

---
## Formeln aus der Formelsammlung

$\dfrac{U_1}{U_2} = \dfrac{R_1}{R_2}$

$\dfrac{U_2}{U_g} = \dfrac{R_2}{R_1 + R_2} \qquad\Rightarrow\qquad U_2 = \dfrac{R_2}{R_1 + R_2} \cdot U_g$

---
## Belasteter Spannungsteiler

* Sobald am Ausgang eine Last hängt, gelten diese Formeln *nicht* mehr
* Fragen dazu erst in Klasse A

<note>
* Wichtiges Beispiel: Basis-Spannungsteiler am Transistor – Vertiefung im Kapitel Verstärker
</note>

---
## Fragen erkennen

* "Wie teilt sich die Spannung an zwei in Reihe geschalteten Widerständen auf …?" $\rightarrow$ Spannungsteiler
* Ohne konkrete Werte: Ergebnis als allgemeine Formel angeben

---
[question:ED101]
---
### Lösungsweg ED101

$R_1 = 5 \cdot R_2 \quad\Rightarrow\quad \dfrac{U_1}{U_2} = \dfrac{5 \cdot R_2}{R_2} = 5$

$U_1 = 5 \cdot U_2$

---
[question:ED102]
---
### Lösungsweg ED102

$R_1 = \dfrac{R_2}{6} \quad\Rightarrow\quad \dfrac{U_1}{U_2} = \dfrac{1}{6}$

$U_1 = \dfrac{U_2}{6}$

---
[question:ED103]
---
### Lösungsweg ED103

* $R_1 : R_2 = \qty{10}{\kilo\ohm} : \qty{20}{\kilo\ohm} = 1 : 2$
* Gesamtwiderstand $\qty{30}{\kilo\ohm}$, $U_g = \qty{9}{\volt}$

$U_2 = \dfrac{R_2}{R_1 + R_2} \cdot U_g = \dfrac{20}{30} \cdot \qty{9}{\volt} = \qty{6}{\volt}$
