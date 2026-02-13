<left>
[picture:342:daempfungsglied_pi:Dämpfungsglied in PI-Konfiguration mit Quelle und Lastwiderstand]
</left>
<right>
* Schwächen Signalpegel definiert ab
* Vermeidung von Übersteuerung oder Beschädigung von Messgeräten
* Eingangspegel für Verstärker und Empfänger auf ein definiertes Maß reduzieren
</right>
<note>
Der Name PI-Konfiguration stammt vom Aufbau der Widerstände als &Pi;
</note>

---
<left>
[picture:342:daempfungsglied_pi:Dämpfungsglied in PI-Konfiguration mit Quelle und Lastwiderstand]
</left>
<right>
* Dämpfung über Widerstände und Umwandlung in Wärme
* Bei symmetrischen Dämpfungsgliedern sind Ein- und Ausgangsimpedanzen gleich
* Üblicherweise 50 Ω
</right>

---
<left>
[picture:341:daempfungsglied_t:Dämpfungsglied in T-Konfiguration mit Quelle und Lastwiderstand]
</left>
<right>
* Dämpfung wird in dB angegeben
* z.B 20dB = Faktor 100
* 100 W Eingangsleistung &rArr; 1 W Ausgangsleistung
</right>
<note>
Der Name T-Konfiguration stammt vom Aufbau der Widerstände als T
</note>

---
[question:AD806]
--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $P_1 = 100W$
* gegeben: $a = 20dB$
* gesucht: $\Delta P = P_2 - P_1$

<fragment>
$\begin{split} a &= 10 \cdot \log_{10}{(\frac{P_1}{P_2})}dB\\ \Rightarrow \frac{a}{10} &= \log_{10}{(\frac{P_1}{P_2})}dB\\ \Rightarrow 10^{\frac{a}{10}} &= \frac{P_1}{P_2}\\ \Rightarrow P_2 &= \frac{P_1}{10^{\frac{a}{10}}}\end{split}$
</fragment>
---
<fragment>
$P_2 = \frac{P_1}{10^{\frac{a}{10}}} = \frac{100W}{10^{\frac{20}{10}}} = 1W$
</fragment>
<fragment>
$\Delta P = P_2 - P_1 = 100W - 1W = 99W$
</fragment>
---
[question:AD803]
---
#### Lösungweg

* 20dB entsprechen einer Leistungdämpfung mit dem Faktor 100

---
[question:AD804]
---
#### Lösungsweg

* 6dB entsprechen einer Leistungsdämpfung mit dem Faktor 4

---
[question:AD805]
---
#### Lösungsweg

* Die Impedanz für die Gesamtschaltung ändert sich nicht – also 50Ω


---
[question:AD801]
---
[question:AD802]