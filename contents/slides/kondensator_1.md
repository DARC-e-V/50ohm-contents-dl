## Kondensator

<left>
* Sehr wichtiges Bauteil in Funktechnik und Elektronik
* Zwei leitende Flächen (Platten, Schichten, Elektroden)
* Dazwischen ein Isolator = *Dielektrikum*
</left>
<right>
[picture:922:e_kondensator_aufbau:Prinzipieller Aufbau eines Kondensators]
</right>

---
## Kapazität

* *Kapazität* $C$ = Fähigkeit, Ladung zu speichern
* Größeres $C$ $\rightarrow$ mehr Ladung $Q$ speicherbar
* Höhere Spannung $\rightarrow$ mehr Ladung
* $Q = C \cdot U$ (nicht in der Formelsammlung, nicht prüfungsrelevant)
* Einheit von $Q$: $\unit{\ampere\second}$
* Einheit von $C$: $\unit{\ampere\second\per\volt}$ = *Farad* $\unit{\farad}$

<note>
* Farad zu Ehren von Michael Faraday (1791 - 1867)
* $\qty{1}{\farad}$: bei $\qty{1}{\volt}$ wird eine Ladung von $\qty{1}{\ampere\second}$ gespeichert
</note>

---
[question:EA101]
---
## Feld im Kondensator

* Spannung angelegt $\rightarrow$ elektrisches Feld $E$ zwischen den Platten
* Höhere Spannung oder kleinerer Abstand $\rightarrow$ stärkeres Feld
* Bereits aus dem Kapitel zum elektrischen Feld bekannt

$E = \dfrac{U}{d}$

---
## Kapazität aus den Abmessungen

$C = \dfrac{\varepsilon_0 \cdot \varepsilon_r \cdot A}{d}$

<left>
* $A$ = gegenüberstehende Plattenfläche
* $d$ = Plattenabstand
* $\varepsilon_0$ = elektrische Feldkonstante (Naturkonstante)
</left>
<right>
* $\varepsilon_0 = \qty{0,855e-11}{\ampere\second\per\volt\meter}$
* $\varepsilon_r$ = relative Dielektrizitätszahl des Dielektrikums (ohne Einheit)
</right>

---
## Relative Dielektrizitätszahl

| Material | $\varepsilon_r$ |
| Luft (trocken) | 1,00059 |
| Voll-PE (Polyäthylen) | 2,29 |
| Schaum-PE | 1,5 |
| PTFE (Teflon) | 2,0 |
[table:e_dielektrizitaetszahl:Relative Dielektrizitätszahl]

---
## Folgerungen aus der Formel

* Spannung $U$ kommt in der Formel *nicht* vor
* Größerer Plattenabstand $d$ $\rightarrow$ kleinere Kapazität
* Größere Fläche $A$ oder größeres $\varepsilon_r$ $\rightarrow$ größere Kapazität
* Formel und Materialtabelle stehen in der Formelsammlung

---
[question:EC205]
---
[question:EC204]
---
[question:EC203]
---
## Kondensator im Gleichstromkreis

[picture:1015:e_stromkreis_kondensator:Stromkreis zum Aufladen eines Kondensators]

---
## Aufladung

* $C$ über Widerstand $R$ an Gleichspannung, Schalter schließt
* Elektronen vom Minuspol auf eine Platte $\rightarrow$ Überschuss
* Von der anderen Platte zum Pluspol $\rightarrow$ Mangel
* Kein Strom durchs Dielektrikum, Aufladung nur durch Ladungstrennung

---
## Lade- und Entladevorgang

<left>
* Anfangs hoher Strom (nur durch $R$ begrenzt), dann fällt er ab
* $U_C$ steigt verzögert nach einer Exponentialfunktion, dann kein Strom mehr
* Größerer Widerstand $\rightarrow$ längere Ladezeit
* Entladen: Strom umgekehrt, Spannung baut sich langsam ab
</left>
<right>
[picture:185:e_ladekurve_c:Ladespannung eines Kondensators]
</right>

---
## Lade- und Entladespannung am Oszilloskop

[photo:247:e_lade_entladespannung_mit_oszilloskop:Lade- und Entladespannung an einem Kondensator]

---
[question:EC201]
---
## Kondensator im Wechselstrom

* Frequenzabhängiger Widerstand = *kapazitiver Blindwiderstand* $X_C$

$|X_C| = \dfrac{1}{\omega \cdot C} = \dfrac{1}{2 \cdot \pi \cdot f \cdot C}$

* $X_C$ umgekehrt proportional zur Frequenz
* Kleinere Frequenz $\rightarrow X_C$ größer
* Höhere Frequenz $\rightarrow X_C$ kleiner
* Hintergründe erst in Klasse A

---
[question:EC202]
---
## Bauformen

<left>
Dielektrikum:
* Luft: Drehkondensator, Trimmer
* Kunststofffolie: Wickelkondensator
* Keramik: HF-Kondensatoren, SMD
* Metalloxid: Elektrolytkondensator
</left>
<right>
[photo:206:e_kondensatorvarianten:Kondensatorvarianten]
</right>

---
## Bauformen nach Aufbau

* *Festkondensatoren*: Keramik-, Folien-, Elektrolytkondensatoren
* *Veränderliche Kondensatoren*: Dreh- und Trimmkondensatoren

---
## Luft- und Keramikkondensatoren

<left>
* Gerne für HF-Filter verwendet
</left>
<right>
[picture:923:e_aufbau_keramik_c:Keramikkondensator]
</right>

---
[question:ED216]
---
## Elektrolytkondensator (ELKO)

* Aufgeraute Alu-Folie in einem Elektrolyt (z.B. Borax), chemische Oxidation
* Sehr dünne Oxidschicht $\rightarrow$ hohe Kapazität bei kleiner Baugröße
* Begrenzte Spannungsfestigkeit, auf dem ELKO angegeben
* Nur an Gleichspannung, Polung beachten
  * falsche Polung $\rightarrow$ Oxidschicht baut ab $\rightarrow$ ELKO wird zerstört
* Alle anderen Kondensatoren auch an Wechselspannung betreibbar

---
[question:EC207]
---
## Folien-Wickelkondensator

<left>
* Kunststoff als extrem dünne Folie, mit Elektroden versehen
* Aufgewickelt oder aus Lagen geschichtet
* Neben Keramik und ELKO am häufigsten eingesetzt
</left>
<right>
[picture:49:e_aufbau_wickel_c:Folien-Wickelkondensator]
</right>

---
## Drehkondensator

<left>
* In Endstufen und Anpassnetzwerken
* Platten auf isolierter Achse rotieren zwischen feststehenden Platten
* Ändert die wirksame Überlappungsfläche $\rightarrow$ Kapazität einstellbar
* *Trimmkondensator*: gleiches Prinzip, nur für gelegentlichen Abgleich
</left>
<right>
[picture:840:e_drehkondensator:Aufbau eines Drehkondensators]
</right>

---
[question:EC206]
---
## Schaltzeichen

<left>
* a) Festkondensator
* b) gepolter Kondensator / Elektrolytkondensator (ELKO) / Tantalkondensator
* c) Drehkondensator (Drehko)
* d) Trimmkondensator für Abgleichzwecke
</left>
<right>
[picture:924:e_kondensator_schaltzeichen:Schaltzeichen verschiedener Kondensatorarten]
</right>
