<left>
[picture:978:a_swr:Stehende Welle]
</left>
<right>
* Das Stehwellenverhältnis (SWR) kann oft direkt anhand des Speisewiderstands einer Antenne angegeben werden
* Bei einem reinen Wirkwiderstand (ohne induktive oder kapazitive Anteile) berechnet sich das SWR aus dem Verhältnis von Lastwiderstand zu Kabelwellenwiderstand (sodass SWR ≥ $\num{1}$ ist)
</right>

---

* Beispiel: Eine Antenne mit $\qty{100}{\ohm}$ an einem $\qty{50}{\ohm}$ Kabel führt zu einem SWR von $\num{2}$, während eine mit $\qty{10}{\ohm}$ zu einem SWR von $\num{5}$ führt
* Zur Erinnerung: Der Widerstand eines Faltdipols liegt bei knapp $\qty{300}{\ohm}$

---
[question:AG405]
---
#### Lösungsweg
* gegeben: $Z = \qty{75}{\ohm}$
* gegeben: $R_2 \approx \qty{300}{\ohm}$ Widerstand Faltdipol
* gesucht: $s$

<fragment>
$s = \frac{R_2}{Z} = \frac{\qty{300}{\ohm}}{\qty{75}{\ohm}} = 4$
</fragment>
---

### Einfluss der Leitungsdämpfung auf das Stehwellenverhältnis

* Leitungsdämpfung reduziert sowohl die vorlaufende als auch die rücklaufende Leistung
* Selbst wenn am Kabelende $\qty{100}{\percent}$ der Energie reflektiert werden, kann am Sender ein niedrigeres (besseres) SWR gemessen werden
* Beispiel: Geht in Hin- und Rürichtung jeweils die Hälfte der Leistung verloren, so verbleibt nur ein Viertel der ursprünglichen Leistung – dies entspricht einem gemessenen SWR von $\num{3}$ ($\qty{25}{\percent}$ reflektierte Leistung)

---
[question:AG402]
---
[question:AG403]
---

### Auswirkung von Leitungsdämpfung auf gemessenes SWR

* Bei einer Leitungsdiämpfung von $\qty{5}{\dB}$ in Hin- und Rürichtung (insgesamt $\qty{10}{\dB}$) entspricht die rücklaufende Leistung nur einem Zehntel der vorlaufenden
* Das gemessene SWR lässt sich mit der Formel berechnen:
  
<fragment>
$s = \frac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}}$
</fragment>

---
[question:AG404]
---

#### Lösungsweg
* gegeben: $P_V = \qty{10}{\watt}$
* gegeben: $a = \qty{5}{\dB}$
* gesucht: $s$

<fragment>
Dämpfung auf gesamtes Kabel für Hin- und Rückweg: $\qty{10}{\dB}$
$P_R = \qty{-10}{\dB} \cdot P_V = \dfrac{\qty{10}{\watt}}{10} = \qty{1}{\watt}$
</fragment>
<fragment>
$s = \dfrac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}} = \dfrac{\sqrt{\qty{10}{\watt}}+\sqrt{\qty{1}{\watt}}}{\sqrt{\qty{10}{\watt}}-\sqrt{\qty{1}{\watt}}} = 1,92$
</fragment>
