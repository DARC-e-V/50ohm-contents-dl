## Widerstand von Drähten

<left>
* Leitfähiges Material besteht aus Atomen in einer (Gitter-)Struktur
* Elektronen werden geteilt und sind dadurch frei beweglich
* Je nach Material gibt es mehr oder weniger freie Elektronen, die auf Atome stoßen
</left>
<right>
[picture:713:a_leitermodell:Atome (+) und bewegliche Elektronen (-) in einem metallischen Leiter]
</right>

---
### Spezifischer Widerstand $\rho$
<left>
$R = \frac{\rho\cdot l}{A_{\textrm{Dr}}}$

* $l$: Drahtlänge
* $A_{\textrm{Dr}}$: Drahtquerschnitt
* $\rho$: Spezifischer Widerstand in $\unit{\ohm\cdot\milli\meter\squared\per\meter}$
</left>
<right>
<fragment>
Kupfer: 0,018
Aluminium: 0,028
Gold: 0,022
Silber: 0,016
Zink: 0,11
Eisen: 0,1
Messing: 0,07
</fragment>
</right>
<note>
Damit lässt sich der ohmsche Widerstand eines Drahtes bei bekanntem Material, Länge und dem Querschnitt ausrechnen
</note>

---
[question:AB101]
--- style="font-size: smaller;"
### Lösungsweg
* gegeben: $l = \qty{1,8}{\meter}$
* gegeben: $d = \qty{0,2}{\milli\meter}$
* gegeben: $\rho = \qty{0,018}{\ohm\cdot\milli\meter\squared\per\meter}$
* gesucht: $R$

<fragment>
$$A_{\textrm{Dr}} = \frac{d^2\cdot \pi}{4} = \frac{(\qty{0,2}{\milli\meter})^2 \cdot \pi}{4} = \qty{\frac{\pi}{100}}{\milli\meter\squared} = \qty{0,0314}{\milli\meter\squared}$$
</fragment>
<fragment>
$$R = \frac{\rho\cdot l}{A_{\textrm{Dr}}} = \frac{\qty{0,018}{\ohm\cdot\milli\meter\squared\per\meter} \cdot \qty{1,8}{\meter}}{\qty{0,0314}{\milli\meter\squared}} \approx \qty{1,02}{\ohm}$$
</fragment>
---
[question:AB102]
---
### Lösungsweg
* gegeben: $A_{\textrm{Dr}} = \qty{0,5}{\milli\meter\squared}$
* gegeben: $R = \qty{1,5}{\ohm}$
* gegeben: $\rho = \qty{0,018}{\ohm\cdot\milli\meter\squared\per\meter}$
* gesucht: $l$

<fragment>
$\begin{split} R &= \frac{\rho\cdot l}{A_{\textrm{Dr}}}\\ \Rightarrow l &= \frac{R\cdot A_{\textrm{Dr}}}{\rho} = \frac{\qty{1,5}{\ohm} \cdot \qty{0,5}{\milli\meter\squared}}{\qty{0,018}{\ohm\cdot\milli\meter\squared\per\meter}} \approx \qty{41,7}{\meter} \end{split}$
</fragment>

---
## Temperaturkoeffizient

* Widerstand von Metallen steigt bei zunehemender Temperatur
* Atome bewegen sich bei höherer Temperatur mehr, wodurch es zu mehr Kollisionen mit Elektronen kommt

---
[question:AB103]