--- style="font-size: 0.7em;"
## Dezibel einfach erklärt

| l:Was | r:Leistung in $\unit{\milli\watt}$ |
| effektive Leistung EME-Station | 100 000 000 | 
| Standard Transceiver | 100 000 |
| Kleine Handfunke | 1 000 |
| Lautsprechersignal (Zimmerlautstärke) | 100 |
| Kopfhörersignal | 1 |
| Lautes KW-Signal | 0,000 001 |
| Leises KW-Signal (Antenneneingang RX) | 0,000 000 000 001 |
[table:e_dezibel_leistungen_mw:Leistungen in $\unit{\milli\watt}$]

Wer mit diesen Zahlen umgeht, fängt automatisch an, die Nullen zu zählen.

--- style="font-size: 0.7em;"
Wir zählen die Nullen (und nennen das Ergebnis "Bel")

| l:Was | r:Leistung in $\unit{\milli\watt}$ | r:Bel |
| effektive Leistung EME-Station | 100 000 000 | 8 |
| Standard Transceiver | 100 000 | 5 |
| Kleine Handfunke | 1 000 | 3 |
| Lautsprechersignal (Zimmerlautstärke) | 100 | 2 |
| Kopfhörersignal | 1 | 0 |
| Lautes KW-Signal | 0,000 001 | -6 |
| Leises KW-Signal (Antenneneingang RX) | 0,000 000 000 001 | -12 |
[table:e_dezibel_leistungen_bel:Leistungen in $\unit{\milli\watt}$ und Bel]

<note>
Nach Alexander Graham Bell
</note>
--- style="font-size: 0.7em;"
$\unit{\dBm}$ = Dezibel bezogen auf $\unit{\milli\watt}$

| l:Was | r:Leistung in $\unit{\milli\watt}$ | r:Bel | r:$\unit{\dBm}$ |
| effektive Leistung EME-Station | 100 000 000 | 8 | 80 |
| Standard Transceiver | 100 000 | 5 | 50 |
| Kleine Handfunke | 1 000 | 3 | 30 |
| Lautsprechersignal (Zimmerlautstärke) | 100 | 2 | 20 |
| Kopfhörersignal | 1 | 0 | 0 |
| Lautes KW-Signal | 0,000 001 | -6 | -60 |
| Leises KW-Signal (Antenneneingang RX) | 0,000 000 000 001 | -12 | -120 |
[table:e_dezibel_leistungen_bel:Leistungen in $\unit{\milli\watt}$ und Bel]

<note>
* Faktor 10
* dezi wie in dezimeter
</note>
---
### Leistungsverstärkung

*Empfänger*
* Eingangssignal: $\qty{0,000000000001}{\milli\watt}$
* Ausgangssignal: $\qty{100}{\milli\watt}$
* Benötigte Verstärkung: $\num{100000000000000}$
 
*Sender*
* Frequenzerzeugende Stufe (Oszillator): $\qty{10}{\milli\watt}$
* Ausgangssignal: $\qty{100000}{\milli\watt}$
* Benötigte Verstärkung: $\num{10000}$
 
---
### Leistungsverstärkung mit dB
*Empfänger*
* Eingangssignal: $\qty{0,000000000001}{\milli\watt} = \qty{-120}{\dBm}$
* Ausgangssignal: $\qty{100}{\milli\watt} = \qty{20}{\dBm}$
* Benötigte Verstärkung: $\num{100000000000000} = \qty{140}{\dB}$
 
*Sender*
* Frequenzerzeugende Stufe (Oszillator): $\qty{10}{\milli\watt} = \qty{10}{\dBm}$
* Ausgangssignal: $\qty{100000}{\milli\watt} = \qty{50}{\dBm}$
* Benötigte Verstärkung: $\num{10000} = \qty{40}{\dB}$

<note>
* Differenz ist die Verstärkung
* Verstärkung ist ein Faktor und nicht auf das $\unit{mW}$ bezogen, deshalb nur $\unit{\dB}$
</note>

--- style="font-size: 0.7em;"
## Wichtige Leistungsfaktoren

| c:$\unit{dB}$ | c:≈ Leistungsfaktor |
| $0$ | $1$ |
| $1,5$ | $\sqrt{2} = 1,41$ |
| $2,15$ | $1,64$ |
| $3$ | $2$ |
| $5$ | $\sqrt{10} = 3,16$ |
| $6$ | $4$ |
| $10$ | $10$ |
| $20$ | $100$ |
[table:e_dezibel_leistungsfaktoren:Wichtige Leistungsfaktoren in $\unit{\dB}$]

<note>
* Erinnerung: 1,64 ist der Faktor zwischen Dipol und isotropen Kugelstrahler
</note>

---
### Berechnung mit Taschenrechner

Ältere Modelle
* Faktor-Wert &rarr; *log*-Taste &rarr; &times;10 &rarr; dB
* $\unit{\dB}$-Wert &rarr; &div;10 &rarr; *10<sup>x</sup>*-Taste &rarr; Faktor

Neuere Modelle
* *log*-Taste &rarr; Faktor-Wert &rarr; *)*-Taste &rarr; &times;10 &rarr; *=*-Taste &rarr; dB
* *10<sup>x</sup>*-Taste &rarr; $\unit{\dB}$-Wert &rarr; &div;10 &rarr; *=*-Taste &rarr; Faktor

---
[question:EA107]