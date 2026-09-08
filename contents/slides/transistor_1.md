## Transistor

* Altes Sprichwort: der beste HF-Verstärker ist die Antenne – lange gab es keine verstärkende Elektronik
* 1907 die Elektronenröhre – erfolgreich, aber groß und wenig effizient
* 1947/1948 der *Bipolartransistor*: alles läuft im Festkörper (Halbleiter) ab
* Überwiegend Gegenstand der Klasse-E-Prüfungsfragen

---
[question:EC602]
---
## Ideale Funktion

* *Spannungsgesteuerte Stromquelle*
* Kleine Spannungsänderung am Eingang $\rightarrow$ große Stromänderung am Ausgang
* Gilt für alle Transistortypen und die Elektronenröhre

---
## Aufbau des Bipolartransistors

* Drei Anschlüsse: *Emitter*, *Basis*, *Kollektor*
* Emitter sendet Ladungsträger in die Basis
  * NPN-Transistor: Elektronen
  * PNP-Transistor: Löcher (Defektelektronen)
* Ladungsträger durchqueren die Basis, der Kollektor sammelt sie wieder ein

---
## Schaltzeichen

<left>
* Emitter am Pfeil erkennbar
  * NPN: Pfeil von der Basis weg
  * PNP: Pfeil zur Basis hin
* Merksatz: PNP $\rightarrow$ *P*feil *N*ach *P*latte
</left>
<right>
[picture:864:e_npn_pnp_symbol:Symbole NPN- und PNP-Transistor]
</right>

---
[question:EC605]
---
[question:EC606]
---
[question:EC607]
---
[question:EC608]
---
[question:EC609]
---
## Zwei Dioden im Transistor

* Zusammengesetzt aus Emitter-Basis-Diode und Basis-Kollektor-Diode
* Aktiver Betrieb: Emitter-Basis-Diode in *Flussrichtung*
  * NPN: Basis positiver als Emitter, PNP: Basis negativer
* Basis-Kollektor-Diode in *Sperrrichtung*
  * NPN: Kollektor positiver als Basis, PNP: Kollektor negativer

---
## Basis-Emitter-Spannung

* Transistorfunktion nur, wenn die Basiszone wenige Mikrometer breit ist
* Nicht aus zwei zusammengelöteten Dioden herstellbar
* Minimale $U_\mathrm{BE}$ hängt vom Halbleiter ab
* Silizium-NPN: Basis $\approx \qty{0,6}{\volt}$ positiver als Emitter
* Silizium-PNP: Basis $\approx \qty{0,6}{\volt}$ negativer als Emitter

---
[question:EC610]
---
## Schaltet der NPN-Transistor durch?

$U_\mathrm{BE} = U_\mathrm{B} - U_\mathrm{E}$

* NPN leitet bei $U_\mathrm{BE} \approx +\qty{0,6}{\volt}$
* Auf die Vorzeichen achten
* Basis $\qty{+2}{\volt}$, Emitter $\qty{+1,4}{\volt}$ $\rightarrow U_\mathrm{BE} = +\qty{0,6}{\volt}$
* Basis $\qty{-5,6}{\volt}$, Emitter $\qty{-6,2}{\volt}$ $\rightarrow U_\mathrm{BE} = +\qty{0,6}{\volt}$

---
[question:EC612]
---
[question:EC613]
---
## Schaltet der PNP-Transistor durch?

* PNP leitet bei $U_\mathrm{BE} \approx -\qty{0,6}{\volt}$
* Basis $\qty{+5,6}{\volt}$, Emitter $\qty{+6,2}{\volt}$ $\rightarrow U_\mathrm{BE} = -\qty{0,6}{\volt}$
* Basis $\qty{-2}{\volt}$, Emitter $\qty{-1,4}{\volt}$ $\rightarrow U_\mathrm{BE} = -\qty{0,6}{\volt}$

---
[question:EC614]
---
[question:EC615]
---
## Ströme und Spannungen am NPN-Transistor

<left>
* Spannungen: $U_\mathrm{BE}$, $U_\mathrm{CB}$, $U_\mathrm{CE}$
* Kollektorstrom hängt exponentiell von $U_\mathrm{BE}$ ab

$I_\mathrm{C} = I_\mathrm{S}\ e^{\frac{U_\mathrm{BE}}{U_\mathrm{T}}}$

* $U_\mathrm{T} \approx \qty{26}{\milli\volt}$ bei Raumtemperatur
</left>
<right>
[picture:863:e_npn_i_u:Ströme und Spannungen an einem NPN-Transistor]
</right>

---
## Stromverstärkung

* Basisstrom $I_\mathrm{B}$ hat die gleiche Spannungsabhängigkeit wie $I_\mathrm{C}$

$\dfrac{I_\mathrm{C}}{I_\mathrm{B}} = B$

* $B$ = Stromverstärkung (in Emitterschaltung), praktisch $50 \dots 350$
* Praktische Vorstellung: der Transistor ist stromgesteuert (physikalisch nicht exakt)

---
## Analogie: Wasserkanal

<left>
* Ein Steuerkanal betätigt über eine Klappe ein Wehr im Hauptkanal
* Kein Wasser im Steuerkanal $\rightarrow$ Wehr geschlossen, kein Fluss im Hauptkanal
</left>
<right>
[picture:835:e_transistor_wehr_geschlossen:Steuerkanal schließt das Wehr komplett]
</right>

--- data-transition="none"
## Analogie: Wasserkanal

<left>
* Etwas Wasser im Steuerkanal $\rightarrow$ Klappe hebt sich, Wehr öffnet zur Hälfte
</left>
<right>
[picture:837:e_transistor_wehr_halb_offen:Steuerkanal öffnet das Wehr halb]
</right>

--- data-transition="none"
## Analogie: Wasserkanal

<left>
* Mehr Wasser im Steuerkanal $\rightarrow$ Wehr öffnet komplett
</left>
<right>
[picture:836:e_transistor_wehr_geoeffnet:Steuerkanal öffnet das Wehr komplett]
</right>

---
[question:EC603]
---
## Emitterstrom

$I_\mathrm{E} = I_\mathrm{C} + I_\mathrm{B}$

* Durch den Emitter fließt der größte Strom

---
[question:EC611]
---
## Arbeitspunkt und Feldeffekttransistor

* Spannungsarbeitspunkt meist über die Kollektor-Emitter-Spannung

$U_\mathrm{CE} = U_\mathrm{CB} + U_\mathrm{BE}$

* *Feldeffekttransistoren* (FET): physikalisch anders, gleiche Grundfunktion, spannungsgesteuert (kein Steuerstrom)
* MOSFETs stecken milliardenfach in integrierten Schaltkreisen – Details in Klasse A

---
[question:EC604]
---
## Einsatz

* Als *Verstärker*: Transistor wird stufenlos gesteuert
* Als *Schalter*: Transistor sperrt oder steuert voll durch (Schalttransistor)
* Als *steuerbarer Widerstand* bei kleinen Ausgangsspannungen (vor allem FET)

---
[question:EC601]
