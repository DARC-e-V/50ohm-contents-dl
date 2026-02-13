## Dezibel

* Logarithmische Angabe von Verhältnissen, insbesondere bei Leistungen
* Macht das Arbeiten mit kleinen und großen Leistungen einfacher
* Verstärkungen und Dämpfungen lassen sich einfacher berechnen

--- style="font-size: 0.7em;"
## Leistungspegel

Faktor 10

*Leistung bezogen auf 1 mW*
$p = 10\cdot \log_{10}\left(\frac{P}{1mW}\right)\textrm{dBm}$
<fragment>
&rarr; $0\textrm{dBm}$ liegt bei $P = 1mW$ vor
</fragment>

<fragment>
*Leistung bezogen auf 1 W*
$p = 10\cdot \log_{10}\left(\frac{P}{1W}\right)\textrm{dBW}$
</fragment>
<fragment>
&rarr; $0\textrm{dBW}$ liegt bei $P = 1W$ vor
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

$u = 20\cdot \log_{10}\left(\frac{U}{0,775V}\right)\textrm{dBu}$

<fragment>
*Spannung bezogen auf 0,775 V*
&rarr; $0\textrm{dBu}$ liegt bei $U = 0,775V$ vor
</fragment>
<fragment>
*Spannung bezogen auf 1 V*
&rarr; $0\textrm{dBV}$ liegt bei $U = 1V$ vor
</fragment>
<fragment>
*Spannung bezogen auf 1 µV*
&rarr; $0\textrm{dBµV}$ liegt bei $U = 1µV$ vor
</fragment>

<note>
Details zur Berechnung des Faktor 20 sind im Online-Kurs. Kurzfassung: Im Spannungsverhältnis wird mit Quadraten gerchnet, was als Faktor vor den Logarithmus gezogen werde kann.
</note>
---
[question:AA111]
---
## Berechnungen

---
[question:AA108]
---
### Lösungsweg
* gegeben: $p = 20\textrm{dBW}$
* gesucht: $P$

<fragment>
$\begin{split} p &= 10\cdot \log_{10}\left(\frac{P}{1W}\right)\textrm{dBW}\\ \Rightarrow P &= 10^{\frac{p}{10}} \cdot 1W = 10^{\frac{20\textrm{dBW}}{10}} \cdot 1W = 10^2W \end{split}$
</fragment>
---
[question:AA107]
---
[question:AA109]
---
### Lösungsweg

1W = 1000mW
10 dB = Faktor 10
1000mW &times; 10 = 10000mW = 40dBm
---
[question:AA106]
---
## Lösungsweg
* 16dB = 10dB + 6dB = 10 &times; 4 = 40
* 1W &times; 40 = 40W

<note>
Aus der Tabelle in der Formelsammlung
</note>

---
[question:AA112]
---
### Lösungsweg
* gegeben: $u = 120\textrm{dBµV}/m$
* gesucht: $U$

<fragment>
$\begin{split} u &= 20\cdot \log_{10}\left(\frac{U}{1\textrm{µV}}\right)\textrm{\textrm{dBµV}}\\ \Rightarrow U &= 10^{\frac{u}{20}} \cdot 1\textrm{µV} = 10^{\frac{120\textrm{dBµV}/m}{20}} \cdot 1\textrm{µV} = 1V/m \end{split}$
</fragment>
<fragment>
In der Literatur ist oft zu finden: 120dBµV = 1V
</fragment>
