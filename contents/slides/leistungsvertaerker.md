## HF-Leistungsverstärker

* Verstärken das HF-Signal aus vorherigen Stufen
* Ziel: Erreichen der gewünschten Ausgangsleistung
* Zwei Typen: Breitbandige und selektive HF-Verstärker

---
### Breitbandige HF-Verstärker

<left>
[picture:491:a_verstaerker_breitband_gegentaktverstaerker:Breitband-Gegentaktverstärker]
</left>
<right>
* Gleichmäßige Verstärkung über einen weiten Frequenzbereich (z. B. $\qtyrange{1}{30}{\mega\hertz}$)
* Erkennbar an breitbandigen Koppeltransformatoren
* Keine Parallel- oder Serienkapazitäten als Schwingkreis
</right>

---
[question:AF412]

---
### Selektive HF-Verstärker


<left>
[picture:778:a_verstaerker_selektiver_hf_verstaerker:Selektiver HF-Verstärker]
</left>
<right>
* Verstärkungsmaximum nur in einem schmalen Bereich (z. B. ein Amateurband)
* Frequenzselektive Auslegung
* Verwendung von Serien- oder Parallel-Schwingkreisen im HF-Signalpfad
</right>

---
[question:AF408]

---
# Mehrstufige Verstärker


<left>
[picture:764:a_verstaerker_zweistufiger_breitband_hf_verstaerker:Zweistufiger Breitband-HF-Verstärker]
</left>
<right>
* Verstärker können mehrstufig durch Verkettung einzelner Stufen ausgeführt sein
</right>

---
[question:AF413]

---
## Impedanzanpassung zwischen Verstärkerstufen

* Notwendig für maximale Verstärkung, minimale Verzerrung und optimalen Wirkungsgrad
* Verhindert Reflexionen und Nichtlinearitäten

---
### Methoden der Impedanzanpassung

* Breitbandige Anpassung durch Transformator mit geeignetem Übersetzungsverhältnis
* Frequenzselektive Anpassung durch angezapften Schwingkreis

---

[picture:765:a_anpassung_breitbandige_anpassung:Breitbandige Anpassung zwischen zwei Stufen mittels Transformator mit geeignetem Übersetzungsverhältnis]

---
[question:AF414]

---

[picture:786:a_anpassung_mosfet:Breitbandige Ein- und Ausgangs-Anpassung auf niederohmige MOSFETs mittels Transformatoren]

---
[question:AF417]

---

[picture:779:a_anpassung_induktiver_spannungsteiler:Frequenzselektive Anpassung mit Spule als induktiver Spannungsteiler]

---
[question:AF409]

---

[picture:780:a_anpassung_kapazitiver_spannungsteiler:Frequenzselektive Anpassung mit Kondensator als kapazitiver Spannungsteiler]


---
[question:AF410]

---

[picture:768:a_anpassung_eingang_schwingkreis:Schwingkreis mit veränderbaren Kondensatoren zur Anpassung der Eingangsimpedanz]

---
[question:AF407]

---

[picture:769:a_anpassung_ausgang_schwingkreis:Schwingkreis mit veränderbaren Kondensatoren zur Anpassung der Ausgangsimpedanz]

---
[question:AF406]

---
### Pi-Filter zur Impedanzanpassung

* Passt Ein- und Ausgangsimpedanzen durch Verhältnis der Kapazitäten an
* Spule definiert mit den Kapazitäten die Auslegungsfrequenz
* Tiefpass-Charakter unterdrückt Oberwellen

---
[question:AF405]

---
### LC-Schaltung hinter HF-Leistungsverstärker

* Dient zur Impedanzanpassung und gleichzeitiger Unterdrückung von Oberwellen

---
[question:AF404]

---
## Wirkungsgrad eines HF-Leistungsverstärkers

* Verhältnis zwischen abgegebener HF-Ausgangsleistung und zugeführter Gleichstrom-Versorgungsleistung

---
[question:AF401]

---
## BIAS-Spannung in Leistungsverstärkern

<left>
[picture:786:a_verstaerker_bias_arbeitspunkt:Arbeitspunktverstellung in einem Verstärker durch ein Poti]
</left>
<right>
* Betriebsspannungseinstellung durch Spannungsteiler
* Feineinstellung über Trimmpotentiometer
* Gleichspannungsbetrachtung: Kondensatoren ignorieren, Spulen als Kurzschluss betrachten
</right>

---
[question:AF420]

---
[question:AF423]

---
[question:AF424]

---
### Berechnung der BIAS-Spannung

* Anwendung des Ohmschen Gesetzes
* Berücksichtigung von Parallel- und Serienschaltungen von Widerständen
* Gate-Anschlüsse der Transistoren sind kapazitiv und bei Gleichspannungsbetrachtung vernachlässigbar

---
[question:AF421]

--- style="font-size: smaller;"
#### Lösungsweg
<left>
* gegeben: $U_\text{Z} = \qty{6,2}{\volt}$
* gegeben: $R_2 = \qty{270}{\ohm}$
* gegeben: $R_3 = \qty{220}{\ohm}$
</left>
<right>
* gegeben: $R_4 = \qty{6,8}{\kilo\ohm}$
* gegeben: $R_6 = \qty{150}{\ohm}$
* gesucht: $U_{GS}$
</right>

<left>
<fragment>
$\begin{split}R_\text{E} &= \frac{(R_3+R_6) \cdot R_4}{(R_3 + R_6) + R_4}\\ &= \frac{(\qty{220}{\ohm} + \qty{150}{\ohm}) \cdot \qty{6,8}{\kilo\ohm}}{\qty{220}{\ohm} + \qty{150}{\ohm} + \qty{6,8}{\kilo\ohm}}\\ &= \frac{\qty{2,516}{\mega\ohm}^2}{\qty{7170}{\ohm}}\\ &= \qty{351}{\ohm}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}\frac{U_\text{Z}}{U_{GS}} &= \frac{R_2 + R_\text{E}}{R_\text{E}}\\ \Rightarrow \frac{\qty{6,2}{\volt}}{U_{GS}} &= \frac{\qty{270}{\ohm}+\qty{351}{\ohm}}{\qty{351}{\ohm}}\\ &= 1,77\\ \Rightarrow U_{GS} &= \frac{\qty{6,2}{\volt}}{1,77}\\ &= \qty{3,50}{\volt}\end{split}$
</fragment>
</right>

---
## HF-Entkopplung der Betriebsspannung

* Verhindert Rückwirkungen zwischen Verstärkerstufen (z. B. Schwingneigung)
* Umsetzung durch in Serie geschaltete Induktivitäten und Abblock-Kondensatoren
* Tiefpass-Charakter: DC-Spannung bleibt erhalten, HF wird abgeblockt

---

[picture:781:a_entkopplung_drossel:Drossel zur Entkopplung der HF von der Betriebsspannung]

---
[question:AF411]

---
[question:AF422]

---

[picture:786:a_entkopplung_abblock_kondensatoren:Abblock-Kondensatoren zur Entkopplung der HF von der Betriebsspannung mit Tiefpass-Charakter]

---
[question:AF419]

---
[question:AF418]

---
## HF-Eigenschaften von Kondensatoren

* Große Kapazitäten (z. B. Elektrolytkondensatoren) nur bei niedrigen Frequenzen einsetzbar
* Für HF-Anwendungen Kombination verschiedener Kapazitätswerte zur Abdeckung eines breiten Frequenzbereichs

---
[question:AF415]

---
## Gesamtverstärkung eines Leistungsverstärkers

<left>
[picture:470:a_verstaerker_gesamtverstaerkung:Blockschaltbild eines Verstärkers mit Gewinn und Verlust je Stufe]
</left>
<right>
* Ermittelt durch Differenz zwischen Ausgangs- und Eingangsleistung
* Berechnung über vorzeichenrichtige Subtraktion der dBm-Werte
</right>

---
[question:AF428]
---
#### Lösungsweg

* gegeben: $P_1 = \qty{0,3}{\milli\watt}$ oder $\qty{-5}{\dBm}$
* gegeben: $P_2 = \qty{20}{\watt}$ oder $\qty{43}{\dBm}$
* gesucht: $g$

<left>
<fragment>
$\begin{split}g &= P_2 - P_1\\ &= \qty{43}{\dBm} - (\qty{-5}{\dBm})\\ &= \qty{43}{\dBm} + \qty{5}{\dBm}\\ &= \qty{48}{\dB}\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}g &= \qty{10 \cdot \log_{10}{\left(\frac{P_2}{P_1}\right)}}{\dB}\\ &= \qty{10 \cdot \log_{10}{\left(\frac{\qty{20}{\watt}}{\qty{0,3}{\milli\watt}}\right)}}{\dB} \\ &\approx \qty{48}{\dB}\end{split}$
</fragment>
</right>