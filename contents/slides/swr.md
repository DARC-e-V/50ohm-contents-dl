* Antennen haben einen Speise- oder Fußpunktwiderstand, abhängig von der genauen Anordnung der Antennenelemente
* Passt dieser nicht zum Wellenwiderstand der Zuleitung, kommt es zu einer *Reflexion*
* Sendeleistung wird zum Funkgerät zurück reflektiert $\rightarrow$ kann nicht an der Antenne abgestrahlt werden
* Stimmen Speisewiderstand der Antenne und Wellenwiderstand der Speiseleitung überein, liegt *Anpassung* vor

---

## Stehwellenverhältnis (SWR)

* Messwert für die Güte der Antennenanpassung
* Gibt vereinfacht an, wie viel Sendeleistung von der Antenne reflektiert wird
* Abkürzung SWR vom englischen "standing wave ratio"
* Gemessen mit einem *Stehwellenmessgerät*, kurz *SWR-Meter*

<note>
Genaue Berechnung: $\text{SWR} = \frac {\sqrt{P_\text{V}}+\sqrt{P_\text{R}}} { \sqrt{P_\text{V}}-\sqrt{P_\text{R}}}$ mit $P_\text{V}$ vorlaufender und $P_\text{R}$ rücklaufender Leistung -- für die Prüfung der Klasse N nicht erforderlich
</note>

---

## SWR-Meter

Misst gleichzeitig die Sendeleistung zur Antenne und die reflektierte, rücklaufende Leistung

<left>
[photo:144:swr_meter:Ein einfaches SWR-Meter zum Bestimmen des Stehwellenverhältnisses]
</left>
<right>
[photo:143:swr_meter_kreuzzeiger:SWR-Meter mit Kreuzzeiger, linker Zeiger für die vorlaufende und rechter Zeiger für die rücklaufende Leistung; um das SWR abzulesen wird der grünen Linie am Schnittpunkt beider Zeiger nach unten gefolgt]
</right>
---
Wird zwischen Transceiver und Antenne eingeschleift oder ist bereits im Transceiver eingebaut

<left>
[picture:670:n_trx_kabel_swr_antenne:Prinzipbild SWR-Meter zwischen Transceiver  und Antenne]
</left>
<right>
[photo:67:n_swr_display:Display eines Transceivers]
</right>
<note>
SWR-Meter und S-Meter klingen ähnlich, sind aber verschieden: Das SWR-Meter misst das Stehwellenverhältnis beim Senden, das S-Meter die Signalstärke beim Empfang
</note>

---
[question:NI201]

---

[question:NF101]

---
[question:NI202]

---
## Gute Anpassung

* Bei perfekter Anpassung wird der Wert $\num{1}$ angezeigt
* Der beste erreichbare Wert
* Die gesamte Leistung wird von der Antenne aufgenommen
* Keine Leistung wird zurück in den Sender reflektiert

---
[question:NG301]

---
[question:NI203]

---
## Schlechte Anpassung

* Bei schlechter Anpassung wird nahe unendlich ($\infty$) angezeigt
* Keine Antenne angeschlossen, Übertragungsleitung unterbrochen oder kurzgeschlossen
* Schlechte Anpassung der Antenne oder beschädigte Übertragungsleitung
* Kann im schlimmsten Fall den Sender zerstören

---

* Bei SWR $\num{2}$ werden $\qty{11}{\percent}$ der Sendeleistung reflektiert
* Bei SWR $\num{3}$ werden $\qty{25}{\percent}$ der Sendeleistung reflektiert
* Moderne Transceiver reduzieren die Sendeleistung automatisch, um den Sender zu schützen

---
[question:NG302]

---

[question:NG303]

---
## Hohe Kabeldämpfung

* Verringert das reflektierte Signal
* Führt zur Verfälschung der Messung
* Beispielsweise bei langem Kabel
* Signal wird auf dem Hin- und Rückweg verringert

---
[question:NG208]

<note>
* SWR wird scheinbar besser, aber nur die reflektierte Leistung wird gedämpft
</note>
