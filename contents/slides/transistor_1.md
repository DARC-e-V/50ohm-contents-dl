--- data-transition="none"
## Von der Diode zum Transistor
<left>
Die Funktion kann man sich so vorstellen:
* Mittels eines Steuerkanals wird der Durchfluss eines Wehrs geregelt
* Fließt kein Wasser im Steuerkanal ist das Wehr geschlossen
</left>
<right>
[picture:835:e_transistor_wehr_geschlossen:Steuerkanal schließt Wehr komplett]
</right>

--- data-transition="none"

## Von der Diode zum Transistor
<left>
Die Funktion kann man sich so vorstellen:
* Fließt etwas Wasser im Steuerkanal, öffnet das Wehr zur Hälfte
</left>
<right>
[picture:837:e_transistor_wehr_halb_offen:Steuerkanal öffnet Wehr halb]
</right>

--- data-transition="none"

## Von der Diode zum Transistor
<left>
Die Funktion kann man sich so vorstellen:
* Fließt mehr Wasser im Steuerkanal, ist das Wehr ganz geöffnet
</left>
<right>
[picture:836:e_transistor_wehr_geoeffnet:Steuerkanal öffnet Wehr komplett]
</right>

---

[question:EC602]

---

[question:EC608]

---

### Bipolarer Transistor und Schaltbild

<left>
Merksatz für PNP &rarr; Pfeil Nach Platte
</left>
<right>
[picture:374:e_schaltbild_npn_transistor:Schaltbild NPN-Transistor]
[picture:375:e_schaltbild_pnp_transistor:Schaltbild PNP-Transistor]
</right>

---

[question:EC607]

---

[question:EC606]

---

[question:EC605]

---

[question:EC609]

---

### Schalter oder Verstärker?
* Die Ansteuerung kann so eingestellt werden, dass der Transistor sperrt oder voll durchsteuert, dann spricht man von einem Schalttransistor.
* Die Ansteuerung kann so eingestellt werden, dass der Transistor stufenlos gesteuert wird, dann spricht man von einem Verstärker.

---

[question:EC601]

---
[question:EC603]

---

## Ansteuerspannung und deren Polarität
Je Art des bipolaren Transistor hat man verschiedene Polaritäten.

* Bei einem NPN-Transistor benötigt man zum Durchschalten eine positive Steuerspannung.
* Bei einem PNP-Transistor benötigt man zum Durchschalten eine negative Steuerspannung.

Die Steuerspannung liegt wie bei einer Siliziumdiode bei etwa $\qty{0,6}{\volt}$.

---

[question:EC610]

---

Da neben dem Kollektorstrom auch der Basisstrom durch den Transistor fließt, fließt durch den Emitteranschluss der größte Strom.

---

[question:EC611]

--- style="font-size: smaller;"

###  Wann schaltet der NPN Transistor durch?
Ist die Basis-Emitter-Spannung ausreichend und liegt sie im positiven Potential vor?
Hier muss man auf die Vorzeichen achten und bei negativen Vorzeichen umdenken, Beispiele:

* Basis $\qty{+2}{\volt}$ und Emitter $\qty{+1,4}{\volt}$<br/> &rArr; Die Basis-Emitter-Spannung ist positiv und beträgt $\qty{+0,6}{\volt}$
* Basis $\qty{-5,6}{\volt}$ und Emitter $\qty{-6,2}{\volt}$<br/> &rArr; Die Basis-Emitter-Spannung ist positiv und beträgt $\qty{+0,6}{\volt}$

---

Entweder erkennet man das intuitiv oder man rechnet es (unter Beachtung der Vorzeichen) aus.

$U_{ BE } = U_{ B } - U_{ E }$

---

[question:EC612]

---

[question:EC613]

--- style="font-size: smaller;"

### Wann schaltet der PNP Transistor durch?
Ist die Basis-Emitter-Spannung ausreichend und liegt sie im negativen Potential vor?
Hier muss man auf die Vorzeichen achten und bei negativen Vorzeichen umdenken, Beispiele:

* Basis $\qty{+5,6}{\volt}$ und Emitter $\qty{+6,2}{\volt}$<br/> &rArr; Die Basis-Emitter-Spannung ist ist negativ und beträgt $\qty{-0,6}{\volt}$
* Basis $\qty{-2}{\volt}$ und Emitter $\qty{-1,4}{\volt}$<br/> &rArr; Die Basis-Emitter-Spannung ist negativ und beträgt $\qty{-0,6}{\volt}$

---

Entweder erkennet man das intuitiv oder man rechnet es (unter Beachtung der Vorzeichen) aus.

$U_{ BE } = U_{ B } - U_{ E }$

---

[question:EC614]

---

[question:EC615]

---

## Typen von Transistoren
Die bisher behandelten Transistoren nennt man *Bipolare Transistoren*. Sie sind die Art der Transistoren, die in den 50er Jahren eine technische Revolution einläuteten und die Elektronenröhre ablösten. Im Gegensatz zu den stromgesteuerten Bipolartransistoren sind *Feldeffekttransistoren (FET)* spannungsgesteuert, es fließt also kein Steuerstrom in ihn hinein. Mit diesen werden wir uns im Klasse A Kurs intensiver auseinandersetzen.

---

[question:EC604]