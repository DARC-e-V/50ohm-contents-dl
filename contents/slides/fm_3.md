### Erzeugung

<left>
[picture:155:a_frequenzmodulation_schaltung:Modulator zur Erzeugung von FM]
</left>
<right>
* Kapazität eines Oszillators wird durch die NF geändert
* Bspw. mit einer Kapazitätsdiode
* Die Modulationsfrequenz bestimmt die Häufigkeit der Änderung des HF-Trägers
</right>
<note>
Wird später im Kapitel Sender nochmal betrachtet
</note>

---
[question:AE303]
---
[question:AE301]
---
### Störanfälligkeit

* Die zu übertragende Information ist in der Änderung des Signals enthalten
* Amplitudenschwankungen haben keine Auswirkungen
* Intern wird oft ein Begrenzerverstärker eingesetzt
* Unempfindlich gegenüber impulsförmigen Störungen durch Zündfunken, Elektromotoren o.ä.

---
[question:AE302]
---
### Hub

* Bestimmt, um welchen Betrag sich die Frequenz des Oszillators je nach Amplitude des modulierten Signals ändert
* Größere Amplitude im NF-Signal &harr; größere Auslenkung im Träger
* Größerer Hub &rarr; größere Lautstärke im demodulierten Signal

---
[question:AE305]
--- style="font-size: smaller;"
### Bandbreite

<left>
[picture:910:a_bandbreite_fm:Bandbreite bei FM]
$B \approx 2 \cdot \left(\Delta f_{\textrm{T}} + f_{\textrm{mod max}}\right)$
</left>
<right>
* Belegte Bandbreite: Hub und maximale Modulationsfrequenz
* Bei kleinem Hub und niedriger Modulationsfrequenz &rarr; *Carson-Formel*
* Höhere Modulationsfrequenz oder größerer Hub &rarr; größere Bandbreite
* Nachbarkanalstörungen sind möglich
</right>

<note>
Etwa 99% der Sendeleistung befinden sich in der Bandbreite
</note>
---
[question:AE306]
---
[question:AE307]
---
[question:AE304]
---
[question:AE309]
---
#### Lösungsweg
* gegeben: $f_{\textrm{mod max}} = 2kHz$
* gegeben: $\Delta f_{\textrm{T}} = 1,8kHz$
* gesucht: $B$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ &= 2 \cdot (1,8kHz + 2kHz) = 7,6kHz \end{split}$
</fragment>
---
[question:AE308]
---
#### Lösungsweg
* gegeben: $f_{\textrm{mod max}} = 2,7kHz$
* gegeben: $\Delta f_{\textrm{T}} = 2,5kHz$
* gesucht: $B$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ &= 2 \cdot (2,5kHz + 2,7kHz) = 10,4kHz \end{split}$
</fragment>
---
[question:AE311]
---
#### Lösungsweg
* gegeben: $B = 10kHz$
* gegeben: $\Delta f_{\textrm{T}} = 2,5kHz$
* gesucht: $f_{\textrm{mod max}}$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ \Rightarrow f_{mod max} &= \frac{B}{2} - \Delta f_T\\ &= \frac{10kHz}{2} - 2,5kHz = 2,5kHz \end{split}$
</fragment>
---
[question:AE312]
---
#### Lösungsweg
* gegeben: $B = 10kHz$
* gegeben: $f_{\textrm{mod max}} = 2,7kHz$
* gesucht: $\Delta f_{\textrm{T}}$

<fragment>
$\begin{split} B &\approx 2 \cdot (\Delta f_{\textrm{T}} + f_{\textrm{mod max}})\\ \Rightarrow \Delta f_T &= \frac{B}{2} - f_{mod max}\\ &= \frac{10kHz}{2} - 2,7kHz = 2,3kHz \end{split}$
</fragment>
---
[question:AE310]