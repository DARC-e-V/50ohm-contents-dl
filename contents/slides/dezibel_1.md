## Wozu Dezibel?

* Leistungsverhältnisse überall: Antennengewinn, Verstärkung, Kabeldämpfung
* Werte reichen über viele Größenordnungen (KW-Empfänger: Faktor $10^{12}$)
* Logarithmus macht daraus handliche Zahlen (Multiplikation → Addition)

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
[table:e_dezibel_leistungen_dbm:Leistungen in $\unit{\milli\watt}$, Bel und dBm]

* $\unit{\dB}$ ist der zehnte Teil eines $\unit{\bel}$ (dezi wie in Dezimeter)
  * $\unit{\dBm}$-Wert $= 10 \cdot$ Bel-Wert

---
## Leistungsverhältnis in dB

* $g = 10 \cdot \log_{10}\!\left(\dfrac{P_2}{P_1}\right) \unit{\dB}$
  * $P_1$ = Eingangsleistung, $P_2$ = Ausgangsleistung
* Beispiel: $\qty{50}{\watt}$ auf $\qty{100}{\watt}$ (Faktor $2$)
  * $g = 10 \cdot \log_{10}(2) \approx \qty{3}{\dB}$
* Für Klasse E genügt: Leistungsfaktor $2$ → $\qty{3}{\dB}$

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
 
--- style="font-size: 0.7em;"
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
## Abschätzen ohne Taschenrechner

* dB-Werte, die auf $0$ enden: letzte Null zuhalten
  * die Ziffer davor gibt die Anzahl der Nullen des Verhältnisfaktors an
  * Beispiel: $\qty{30}{\dB}$ → $3$ → $3$ Nullen → Faktor $1000$

--- style="font-size: 0.8em;"
### Berechnung mit Taschenrechner

* *log* / *lg* = Zehnerlogarithmus, *ln* = natürlicher (Basis $e$) – nicht verwechseln

Ältere Modelle
* Faktor → *log* → $\cdot 10$ → $\unit{\dB}$
* $\unit{\dB}$ → $\div 10$ → *$10^x$* → Faktor

Neuere Modelle
* *log* → Faktor → *)* → $\cdot 10$ → *=* → $\unit{\dB}$
* *$10^x$* → $\unit{\dB}$ → $\div 10$ → *=* → Faktor

---
### dBi und dBd

* Zusätze geben die Bezugsgröße an
* In Klasse E: $\unit{\dBi}$ und $\unit{\dBd}$ im Antennenkapitel
* $\unit{\dBm}$, $\unit{\dBW}$ erst in Klasse A

---
[question:EA107]