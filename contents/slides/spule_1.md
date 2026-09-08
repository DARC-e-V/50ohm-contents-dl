## Spule

<left>
* Drittes passives Bauelement nach Widerstand und Kondensator
* Strom durch die Spule $\rightarrow$ Magnetfeld
* Einfachste Bauform: gerade *Zylinderspule*
</left>
<right>
[photo:207:e_spulen:Verschiedene Bauformen von Spulen]
</right>

---
## Schaltsymbole und Aufbau

<left>
[picture:942:e_schaltsymbole_spulen:Schaltsymbole für unterschiedliche Spulenarten]
</left>
<right>
[picture:948:e_spule_Aufbau:Aufbau einer Spule]
</right>

---
## Induktivität

$L = \dfrac{\mu_0 \cdot \mu_r \cdot N^2 \cdot A_S}{l}$

<left>
* $\mu_0 = \qty{1,2566e-6}{\henry\per\meter}$ = magnetische Feldkonstante (Naturkonstante)
* $\mu_r$ = Materialkonstante des Spulenkerns, kann das Magnetfeld verstärken
</left>
<right>
* $N$ = Windungszahl
* $A_S$ = Querschnittsfläche des Spulenkerns
* $l$ = Spulenlänge
</right>

---
## Einheit der Induktivität

* Formelbuchstabe $L$
* Einheit: $\unit{\volt\second\per\ampere}$ = *Henry* $\unit{\henry}$
* $\qty{1}{\henry}$: Stromänderung von $\qty{1}{\ampere}$ je Sekunde erzeugt eine Selbstinduktionsspannung von $\qty{1}{\volt}$
* Praxis meist $\unit{\milli\henry}$, $\unit{\micro\henry}$, $\unit{\nano\henry}$

<note>
* Henry nach Joseph Henry (1797 - 1878)
* Formelbuchstabe $L$ nach Emil Lenz (1804 - 1864), Lenzsche Regel – Vertiefung auf der Webseite
</note>

---
[question:EA102]
---
## Was die Induktivität vergrößert

* $L$ wächst *quadratisch* mit der Windungszahl $N$
  * doppelt so viele Windungen $\rightarrow$ vierfache Induktivität
* Kürzere Spule (kleineres $l$) $\rightarrow L$ steigt
* Größere Querschnittsfläche $A_S$ $\rightarrow L$ steigt
* Magnetisch leitfähiger Kern, z.B. Eisen $\rightarrow L$ steigt
* Selbst ein gerades Drahtstück hat eine kleine parasitäre Induktivität

---
[question:EC305]
---
[question:EC306]
---
[question:EC307]
---
[question:EC304]
---
## Ferromagnetische Stoffe

* Enthalten atomare Elementarmagnete, richten sich im äußeren Magnetfeld aus
* Erhöhen die magnetische Flussdichte stark
* Unter den reinen Elementen nur *Eisen*, *Kobalt*, *Nickel*

---
[question:EB204]
---
## Metallkern in der Spule

* Ferromagnetischer Kern (Eisen) $\rightarrow$ Magnetfeld verstärkt $\rightarrow L$ steigt
* Kern aus Kupfer oder Aluminium $\rightarrow L$ *sinkt*
  * HF-Magnetfeld induziert Wirbelströme im Kern
  * deren Magnetfelder wirken dem Spulenfeld entgegen
* Prüfungsantwort: Magnetfeld dringt nicht in den Kern ein und verringert den Feldquerschnitt (vereinfacht, so merken)

---
[question:EB205]
---
## Spule im Gleichstromkreis

<left>
* Spule über Vorwiderstand an Gleichspannung
* Einschalten: Strom steigt nur allmählich bis zum Maximum
* Lenzsche Regel: Selbstinduktionsspannung wirkt der Stromänderung entgegen
</left>
<right>
[picture:1016:e_spule_einschalten:Stromkreis zur Untersuchung einer Spule]
</right>

---
## Spannungsverlauf beim Einschalten

<left>
* Anfangs fällt fast die ganze Spannung an der Spule ab
* Mit steigendem Strom nimmt die Spannung an der Spule ab
* Stationär: Spule wirkt wie ein Stück Draht, Spannung $\approx 0$
</left>
<right>
[picture:186:e_spule_einschalten_spannung:Spannungsverlauf beim Einschalten]
</right>

---
[question:EC301]
---
## Ausschaltmoment

<left>
* Selbstinduktionsspannung will den Strom aufrechterhalten
* Spule wirkt als Generator, Spannung mit umgekehrter Polarität
* Genau gegenteiliges Verhalten zum Kondensator
* Spulen daher auch zur Verzögerung nutzbar
</left>
<right>
[photo:257:e_Spulenstrom:Ein- und Ausschaltverhalten von Spulenspannung und Spulenstrom]
</right>

---
[question:EC302]
---
## Verzögerte Lampe

* Lampe 1 über Widerstand, Lampe 2 über Spule mit vielen Windungen und Eisenkern
* Selbstinduktionsspannung lässt den Strom durch Lampe 2 nur langsam ansteigen
* $\rightarrow$ Lampe 1 leuchtet zuerst

---
## Spule im Wechselstrom

* Wechselstromwiderstand $X_L$, obwohl der Draht kaum ohmschen Widerstand hat

$X_L = \omega \cdot L = 2 \cdot \pi \cdot f \cdot L$

* Höhere Frequenz $\rightarrow X_L$ größer
* Niedrigere Frequenz $\rightarrow X_L$ kleiner

---
[question:EC303]
