---
## Dummy-Load im HF-Bereich

<left>
[picture:47:a_dummy_load:Dummy-Load aus mehreren Widerstandsketten]
</left>
<right>
* Besteht oft aus mehreren Teilwiderständen für bessere Kühlung und Belastbarkeit
* Widerstände können parallel, in Reihe oder kombiniert geschaltet werden
</right>
---

* Identische Widerstandswerte sorgen für gleichmäßige Verteilung der Verlustleistung
* Berechnung erfolgt nach dem Ohmschen Gesetz und den Regeln für Reihen- und Parallelschaltungen

---
[question:AI601]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $R = \qty{150}{\ohm}$
* gegeben: $R_S = 4\cdot \qty{150}{\ohm} = \qty{600}{\ohm}$
</left>
<right>
* gegeben: $R_{ges} = \qty{50}{\ohm}$
* gegeben: $P_\text{R} = \qty{1}{\watt}$
* gesucht: $n$ Widerstände, $P$
</right>

<fragment>
Reihen mit je 4 Widerständen:
$\frac{1}{R_{ges}} = n_S \cdot \frac{1}{R_S} \Rightarrow n_S = \frac{R_S}{R_{ges}} = \frac{\qty{600}{\ohm}}{\qty{50}{\ohm}} = 12$
$n = 4 \cdot n_S = 4 \cdot 12 = 48$ 
</fragment>
<fragment>
$P = n \cdot P_\text{R} = 48 \cdot \qty{1}{\watt} = \qty{48}{\watt}$
</fragment>

---
### Dummy-Load mit Messausgang

* Kann zur indirekten Messung der Ausgangsleistung eines Senders verwendet werden
* Spitzenwertgleichrichter wandelt HF-Spannung in Gleichspannung um

---
[question:AI602]

---
### Messung der HF-Ausgangsleistung über Spannungsteiler

* Dummy-Load mit Anzapfung ermöglicht grobe Leistungsbestimmung
* HF-Teilspannung wird über Spannungsteiler-Verhältnis berechnet
* Messung mit HF-Tastkopf und Multimeter möglich

---
[question:AI603]

