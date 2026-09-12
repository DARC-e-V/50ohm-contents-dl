## Widerstandsmaterialien

Widerstände lassen sich aus unterschiedlichen Materialien realisieren:

* Drahtwiderstände
* Kohleschichtwiderstände
* Metallschichtwiderstände
* Metalloxidschichtwiderstände
* …

--- style="font-size: 0.8em;"

| l: Material | X: Eigenschaft |
| Drahtwiderstände | Hochlastwiderstände für niedrige Frequenzen |
| Metallschichtwiderstände | Geringe Fertigungstoleranz und Temperaturabhängigkeit, Präzisionswiderstände |
| Metalloxidschichtwiderstände | Für Frequenzen oberhalb von $\qty{30}{\mega\hertz}$ |
[table:e_eigenschaften_widerstaende:Übersicht der Eigenschaften]

---
## Drahtwiderstände

* Widerstandsdraht (Manganin, Konstantan) auf Keramik gewickelt
* Hohe Überlastbarkeit, kleiner Temperaturkoeffizient
* Gewickelt → wirkt auch als Spule (Induktivität) → nur für Gleichstrom / niedrige Frequenzen

---
[question:EC101]
---
## Metalloxidschichtwiderstände

* Dünne Schicht auf einem Träger
* Weitgehend induktionsarm, gute Temperaturstabilität
* Für höhere Frequenzen oberhalb $\qty{30}{\mega\hertz}$ geeignet

---
[question:EC103]
---
## Metallschichtwiderstände

* Sehr geringe Fertigungstoleranz → *Präzisionswiderstände*
* Temperaturunabhängig, aber weniger induktionsarm

---
[question:EC102]
---
## Kohleschichtwiderstände

* Kohleschicht auf einem Träger, kostengünstig
* Große Fertigungstoleranz
* Induktionsarm, für HF nur eingeschränkt geeignet

---
## Dummyload (künstliche Antenne)

* Widerstand soll frequenzunabhängig ca. $\qty{50}{\ohm}$ sein
* *Keine* Windungen (Eigeninduktivität), geringe Eigenkapazität
* Ausreichend temperaturbeständig (setzt Leistung in Wärme um)
* *Keine* Drahtwiderstände verwenden

---
## Dummyload – Bauteilwahl

* VHF/UHF: ungewendelte Metalloxidschichtwiderstände
* $\qty{28}{\mega\hertz}$, $\qty{50}{\mega\hertz}$: auch Kohleschichtwiderstände
* $10 \cdot \qty{500}{\ohm}$ parallel ergeben $\qty{50}{\ohm}$

<note>
Parallelschaltung von Widerständen kommt in einem späteren Kapitel
</note>

---
[question:EC107]
---
[question:EC104]

<note>
* Der Sinn (Eigeninduktivität/-kapazität) wird nach der Vorstellung von Kondensatoren und Spulen klarer
</note>
---
[question:EC106]
---
[question:EC105]
