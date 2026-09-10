## Reihen- und Parallelschaltung von Widerständen

* Gewünschter Widerstandswert oft nicht in der Normreihe
* Oder: nötige Verlustleistung übersteigt den Einzelwiderstand
* Andere Werte durch Reihen- oder Parallelschaltung
* Herleitung aus dem Ohmschen Gesetz $U = R \cdot I$

---
## Reihenschaltung

<left>
* $R_1$ und $R_2$ vom gleichen Strom $I$ durchflossen
* $U_1 = R_1 \cdot I$, $U_2 = R_2 \cdot I$
* Gesamtspannung $U_g = U_1 + U_2 = R_{\mathrm{ges}} \cdot I$
* $I$ kürzt sich heraus
</left>
<right>
[picture:819:e_spannungsteiler:Reihenschaltung zweier Widerstände]
</right>

---
## Reihenschaltung

$R_{\mathrm{ges}} = R_1 + R_2 + R_3 + R_4 + \dots$

* Gesamtwiderstand immer *größer* als der größte Einzelwiderstand

---
## Parallelschaltung

<left>
* An $R_1$ und $R_2$ liegt die gleiche Spannung $U$
* $I_1 = \dfrac{U}{R_1}$, $I_2 = \dfrac{U}{R_2}$
* Gesamtstrom $I = I_1 + I_2$
</left>
<right>
[picture:945:e_parallelschaltung:Parallelschaltung zweier Widerstände mit allen Spannungen und Strömen]
</right>

---
## Parallelschaltung

$\dfrac{1}{R_{\mathrm{ges}}} = \dfrac{1}{R_1} + \dfrac{1}{R_2} + \dfrac{1}{R_3} + \dots$

* Kehrwert des Gesamtwiderstands = Summe der Kehrwerte
* Gesamtwiderstand immer *kleiner* als der kleinste Einzelwiderstand
* Gleiche Widerstände parallel: Einzelwert durch die Anzahl teilen

---
## Zwei Widerstände parallel

$R_{\mathrm{ges}} = \dfrac{R_1 \cdot R_2}{R_1 + R_2}$

---
## Einheiten beachten

* In der Rechnung immer die gleiche Einheit, am besten die Grundeinheit $\unit{\ohm}$
* $\qty{1}{\kilo\ohm}$ und $\qty{10}{\ohm}$ in Reihe: $\qty{1000}{\ohm} + \qty{10}{\ohm} = \qty{1010}{\ohm}$

---
[question:ED104]
---
[question:ED105]
---
[question:ED106]
---
## Gemischte Netzwerke

* Enthalten Reihen- *und* Parallelschaltung
* Erst eine erkennbare Teilschaltung zu einem Ersatzwiderstand zusammenfassen
* Dann mit dem Rest weiterrechnen, je nach Schaltbild

---
## Methode des scharfen Hinsehens

<left>
* $R_1 = \qty{1}{\kilo\ohm}$ in Reihe mit $R_2$ parallel $R_3$
* $R_2 = \qty{2000}{\ohm}$, $R_3 = \qty{2}{\kilo\ohm}$ – gleich groß
* $R_2$ parallel $R_3 = \qty{1}{\kilo\ohm}$ (halber Wert)
* mit $R_1$ in Reihe $\rightarrow R_{\mathrm{ges}} = \qty{2}{\kilo\ohm}$
</left>
<right>
[picture:305:e_tipp_aufgabe:Beispielschaltung]
</right>

---
[question:ED111]
---
[question:ED110]
---
[question:ED112]
---
[question:ED113]
---
[question:ED108]
---
[question:ED109]
---
## Belastbarkeit

* Ausgangspunkt: $P = U \cdot I$
* Reihenschaltung: gleicher Strom, Spannung teilt sich auf
* Parallelschaltung: gleiche Spannung, Strom teilt sich auf
* 3 gleiche Widerstände $\rightarrow$ Schaltung verträgt das *Dreifache* der Einzelleistung, in Reihe wie parallel

---
[question:ED107]
