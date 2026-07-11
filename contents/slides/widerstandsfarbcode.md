<left>
* Statt Zahlenwert wird eine Codierung aus Farbringen auf Widerständen aufgedruckt
* Jede Farbe entspricht einem Zahlenwert
  1. Farbring für 1. Ziffer
  2. Farbring für 2. Ziffer
  3. Farbring für Multiplikator
</left>
<right>
[picture:665:n_widerstandsfarbcodes: Ein Widerstand mit 4 Farbringen]
</right>

--- style="font-size: 0.6em;"
| X:Farbe | l:Wert | l:Multiplikator | l:Toleranz |
| Silber | - | $\num{0,01}$ | $\qty{\pm 10}{\percent}$ |
| Gold | - | $\num{0,1}$ | $\qty{\pm 5}{\percent}$ |
| Schwarz | 0 | $\num{1}$ | - |
| Braun | 1 | $\num{10}$ | $\qty{\pm 1}{\percent}$ |
| Rot | 2 | $\num{100}$ | $\qty{\pm 2}{\percent}$ |
| Orange| 3 | $\num{1000}$ | - |
| Gelb | 4 | $\num{10000}$ | - |
| Grün | 5 | $\num{100000}$ | - |
| Blau | 6 | $\num{1000000}$ | $\qty{\pm 0,25}{\percent}$ |
| Violett | 7 | $\num{10000000}$ | $\qty{\pm 0,1}{\percent}$ |
| Grau | 8 | $\num{100000000}$ | - |
| Weiß | 9 | $\num{1000000000}$ | - |
| Keine | - | - | $\qty{\pm 20}{\percent}$ |
[table:n_widerstandsfarbcodes_tabelle:Widerstandsfarbcodes Tabelle]

<note>
* Tabelle ist in der Formelsammlung
</note>

---

<left>
* In diesem Beispiel:
  1. Farbring 4
  2. Farbring 7
  3. Farbring $\cdot \num{1000}$
* $\begin{split}&47 \cdot \qty{1000}{\ohm}\\ &= \qty{47000}{\ohm}\\ &= \qty{47}{\kilo\ohm}\end{split}$
</left>
<right>
[picture:665:n_widerstandsfarbcodes: Ein Widerstand mit 4 Farbringen]
</right>

---
## Toleranz

* Abweichung vom tatsächlichen Wert
* Beispiel: silber bedeutet $\qty{\pm 10}{\percent}$
* $\qty{10}{\percent} \cdot \qty{47}{\kilo\ohm} = \qty{4,7}{\kilo\ohm}$
* Widerstandswert zwischen $\qty{42,3}{\kilo\ohm}$ und $\qty{51,7}{\kilo\ohm}$

---

[question:NC107]
---
[question:NC105]
---
[question:NC106]
---
[question:NC104]
---
[question:NC103]
---
[question:NC102]
---
[question:NC108]
---
[question:NC109]
---
[question:NC110]
