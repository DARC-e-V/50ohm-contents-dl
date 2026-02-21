## Dezibel

* Logarithmische Angabe von Verhältnissen, insbesondere bei Leistungen
* Macht das Arbeiten mit kleinen und großen Leistungen einfacher
* Verstärkungen und Dämpfungen lassen sich einfacher berechnen

--- style="font-size: 0.7em;"
## Leistungspegel

Faktor 10

*Leistung bezogen auf $\qty{1}{\milli\watt}$*
$p = 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\milli\watt}}\right)\unit{\dBm}$
<fragment>
&rarr; $\qty{0}{\dBm}$ liegt bei $P = \qty{1}{\milli\watt}$ vor
</fragment>

<fragment>
*Leistung bezogen auf \qty{1}{\watt}*
$p = 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\watt}}\right)\unit{\dBW}$
</fragment>
<fragment>
&rarr; $\qty{0}{\dBW}$ liegt bei $P = \qty{1}{\watt}$ vor
</fragment>

---
[question:AA110]
<note>
Nur einsetzen
</note>
---
[question:AA105]

--- style="font-size: 0.7em;"

## Spannungspegel

Faktor 20

$u = 20\cdot \log_{10}\left(\frac{U}{\qty{0,775}{\volt}}\right)\unit{\dBu}$

<fragment>
*Spannung bezogen auf $\qty{0,775}{\volt}$*
&rarr; $\qty{0}{\dBu}$ liegt bei $U = \qty{0,775}{\volt}$ vor
</fragment>
<fragment>
*Spannung bezogen auf $\qty{1}{\volt}$*
&rarr; $\qty{0}{\dBV}$ liegt bei $U = \qty{1}{\volt}$ vor
</fragment>
<fragment>
*Spannung bezogen auf $\qty{1}{\micro\volt}$*
&rarr; $\qty{0}{\dBuV}$ liegt bei $U = \qty{1}{\micro\volt}$ vor
</fragment>

<note>
Details zur Berechnung des Faktor 20 sind im Online-Kurs. Kurzfassung: Im Spannungsverhältnis wird mit Quadraten gerechnet, was als Faktor vor den Logarithmus gezogen werden kann.
</note>
---
[question:AA111]
---
## Berechnungen

---
[question:AA108]
---
### Lösungsweg
* gegeben: $p = \qty{20}{\dBW}$
* gesucht: $P$

<fragment>
$\begin{split} p &= 10\cdot \log_{10}\left(\frac{P}{\qty{1}{\watt}}\right)\unit{\dBW}\\ \Rightarrow P &= 10^{\frac{p}{10}} \cdot \qty{1}{\watt} = 10^{\frac{\qty{20}{\dBW}}{10}} \cdot \qty{1}{\watt} = \qty{10^2}{\watt} \end{split}$
</fragment>
---
[question:AA107]
---
[question:AA109]
---
### Lösungsweg

$\qty{1}{\watt} = \qty{1000}{\milli\watt}$
$\qty{10}{\dB} = \text{Faktor 10}$
$\qty{1000}{\milli\watt} \cdot 10 = \qty{10000}{\milli\watt} = \qty{40}{\dBm}$
---
[question:AA106]
---
## Lösungsweg
* $\qty{16}{\dB} = \qty{10}{\dB} + \qty{6}{\dB} = 10 \cdot 4 = 40$
* $\qty{1}{\watt} \cdot 40 = \qty{40}{\watt}$

<note>
Aus der Tabelle in der Formelsammlung
</note>

---
[question:AA112]
---
### Lösungsweg
* gegeben: $u = \qty{120}{\dBuV\per\meter}$
* gesucht: $U$

<fragment>
$\begin{split} u &= 20\cdot \log_{10}\left(\frac{U}{\qty{1}{\micro\volt}}\right)\unit{\dBuV}\\ \Rightarrow U &= 10^{\frac{u}{20}} \cdot \qty{1}{\micro\volt} = 10^{\frac{\qty{120}{\dBuV\per\meter}}{20}} \cdot \qty{1}{\micro\volt} = \qty{1}{\volt\per\meter} \end{split}$
</fragment>
<fragment>
In der Literatur ist oft zu finden: $\qty{120}{\dBuV} = \qty{1}{\volt}$
</fragment>
