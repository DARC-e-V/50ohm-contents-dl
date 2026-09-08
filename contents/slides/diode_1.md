## Grundfunktion der Diode

<left>
* Aus Klasse N bekannt: Strom fließt nur in *einer* Richtung
* In Sperrrichtung wirkt sie wie ein hoher Widerstand
* Leitet nur, wenn die Anodenspannung größer als die Kathodenspannung ist: $U_d = U_a - U_k > 0$
</left>
<right>
[picture:859:e_diode_u_i:Spannungen und Strom an einer Diode mit Vorwiderstand]
</right>

---
## Exponentielle Kennlinie

* Ist $U_d$ nur wenig größer als 0 $\rightarrow$ noch kein merkbarer Strom

$I_d = I_S \left(e^{\frac{U_d}{U_T}} - 1\right)$

* $e \approx 2,718$ (Euler'sche Zahl), $U_T \approx \qty{26}{\milli\volt}$ bei Raumtemperatur

---
## Sperrsättigungsstrom

* $I_S$ = kleiner Strom, der bei negativer Spannung fließt
* Hängt vom Halbleitermaterial ab
* Germanium (kleine Energiebandlücke) $\rightarrow I_S$ groß
* Größere Energiebandlücke $\rightarrow I_S$ klein

---
[question:EC501]
---
## Schwellspannung

<left>
* Bei positiver $U_d$ steigt der Strom ab einer gewissen Spannung steil an
* *Schwellspannung* $U_{th}$ folgt aus $I_S$: kleineres $I_S$ $\rightarrow$ höhere Schwellspannung
* Germanium: $\qtyrange{0,2}{0,3}{\volt}$
* Silizium: $\qtyrange{0,6}{0,7}{\volt}$
</left>
<right>
[picture:861:e_diode_kennlinie_iu:Kennlinie einer Diode]
</right>

---
## Leuchtdioden (LED)

* Ebenfalls pn-Dioden, senden in Flussrichtung Licht aus
* Nur mit bestimmten Materialien, nicht mit Silizium oder Germanium
* Lichtfarbe durch die Energiebandlücke bestimmt
* Größere Bandlücke $\rightarrow$ kurzwelligeres Licht, kleineres $I_S$, höhere Schwellspannung
* Rote LED $\approx \qty{1,7}{\volt}$, grüne LED $\approx \qty{2,5}{\volt}$

---
## Wann leitet eine Siliziumdiode?

* Diode leitet, wenn $U_a - U_k$ mindestens die Schwellspannung erreicht
* Für Silizium in der Prüfung: $\approx \qty{0,7}{\volt}$
* Nur die Differenz zählt, gilt auch bei negativen Potenzialen an Anode und Kathode

---
[question:EC513]
---
[question:EC510]
---
[question:EC509]
---
[question:EC511]
---
[question:EC512]
---
## Kennlinien verschiedener Dioden

<left>
* Je kleiner $I_S$ (größere Bandlücke), desto weiter rechts die Kennlinie
* Reihenfolge der Schwellspannung: Schottky < Germanium < Silizium < LED
</left>
<right>
[picture:858:e_diode_kennlinien:Kennlinien verschiedener Dioden]
</right>

---
[question:EC503]
---
[question:EC506]
---
[question:EC507]
---
[question:EC508]
---
## LED mit Vorwiderstand

* LED wird in Flussrichtung betrieben
* Vorwiderstand $R_V$ zwischen Spannungsquelle $U$ und LED nötig
* $R_V$ stellt den gewünschten Strom $I$ ein, Schwellspannung $U_{th}$ berücksichtigen

$I = \dfrac{U - U_{th}}{R_V}$

---
[question:EC514]
---
[question:EC515]
---
### Lösungsweg EC515

$R_V = \dfrac{U - U_{th}}{I} = \dfrac{\qty{5,0}{\volt} - \qty{1,4}{\volt}}{\qty{20}{\milli\ampere}} = \dfrac{\qty{3,6}{\volt}}{\qty{0,02}{\ampere}} = \qty{180}{\ohm}$

---
[question:EC516]
---
### Lösungsweg EC516

$R_V = \dfrac{\qty{5,5}{\volt} - \qty{1,75}{\volt}}{\qty{25}{\milli\ampere}} = \dfrac{\qty{3,75}{\volt}}{\qty{0,025}{\ampere}} = \qty{150}{\ohm}$

$P_{R_V} = (U - U_{th}) \cdot I = \qty{3,75}{\volt} \cdot \qty{0,025}{\ampere} \approx \qty{0,1}{\watt}$

---
## Sperrdurchbruch

<left>
* Normal fließt für negative $U_d$ nur ein kleiner Sperrstrom
* Bei sehr negativer Spannung "bricht" die Diode "durch", der Rückwärtsstrom steigt extrem stark an
* Diese Spannung heißt *Zener-Spannung* $U_z$
</left>
<right>
[picture:862:n_diode_kennlinie_uz:Kennlinie einer Z-Diode]
</right>

---
## Zenerdiode

<left>
* Wird zur *Spannungsstabilisierung* eingesetzt
* Durchbruchstrom mit einem Vorwiderstand begrenzen
* Schaltsymbol: Kathodenstrich mit Fortsetzung unter $\qty{90}{\degree}$ – erinnert an das Abknicken der Kennlinie
</left>
<right>
[picture:860:e_zener_symbol:Schaltsymbol einer Zenerdiode]
</right>

---
[question:EC517]
---
[question:EC520]
---
[question:EC521]
---
### Lösungsweg EC521

Unbelastet, daher fließt nur der Z-Strom durch den Vorwiderstand:

$U_V = U_1 - U_Z = \qty{13,8}{\volt} - \qty{5}{\volt} = \qty{8,8}{\volt}$

$R_V = \dfrac{U_V}{I_Z} = \dfrac{\qty{8,8}{\volt}}{\qty{30}{\milli\ampere}} \approx \qty{293}{\ohm}$

---
[question:EC522]
---
### Lösungsweg EC522

Der Vorwiderstand führt Z-Strom *und* Laststrom:

$I_V = I_Z + I_{Last} = \qty{25}{\milli\ampere} + \qty{20}{\milli\ampere} = \qty{45}{\milli\ampere}$

$R_V = \dfrac{U_1 - U_Z}{I_V} \approx \qty{202}{\ohm}$

---
## Schottky-Diode

* Diodeneigenschaft durch einen *Metall-Halbleiter-Übergang* (statt pn-Übergang)
* Schwellspannung etwa halb so groß wie bei einer pn-Diode aus gleichem Material, oder kleiner
* Einsatz: wenn geringe Schwellspannung gefragt ist, oder als sehr schnelle Schaltdiode
* Älteste Halbleiter-Gleichrichter: Ferdinand Braun entdeckte den Effekt 1874

---
[question:EC504]
---
[question:EC505]
---
## Zusammenfassung

* Dioden lassen Strom nur in eine Richtung $\rightarrow$ *Gleichrichtung* von Wechselstrom
* Hohe Sperrspannung ($U_d < U_z$) $\rightarrow$ Rückwärtsstrom steigt stark $\rightarrow$ *Spannungsstabilisierung* (Zenerdiode)
* In Sperrrichtung auch als spannungsgesteuerte Kapazität nutzbar (erst Klasse A)

---
[question:EC502]
---
[question:EC518]
---
[question:EC519]
