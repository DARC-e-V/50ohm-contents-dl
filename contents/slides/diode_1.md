## Anwendung

<left>
* Eine Diode lässt den Stromfluss nur in eine Richtung durch
* In die andere Richtung wirkt sie wie ein hoher Widerstand
* Dioden werden u.a. zur Gleichrichtung von Wechselspannung eingesetzt
</left>
<right>
[picture:689:e_led:Diverse LED in verschiedenen Bauformen und Farben]
</right>
<note>
* Eine spezielle Bauform haben wir schon als LED kennengelernt
</note>

---
[question:EC501]
---
[question:EC502]
---

## Schwellenspannung

<left>
* Damit eine Diode in Durchlassrichtung leitet, muss eine bestimmte Spannung &ndash; die Schwellenspannung oder Durchlassspannung &ndash; überschritten werden
* Je nach Basis des chemischen Elements ist die Schwellenspannung unterschiedlich hoch
</left>
<right>
* Germanium: $\qtyrange{0,2}{0,4}{\volt}$
* Silizium: $\qtyrange{0,6}{0,8}{\volt}$
* LED (Rot): $\qtyrange{1,6}{2,2}{\volt}$
* LED (Gelb, Grün): $\qtyrange{1,9}{2,5}{\volt}$
* LED (Blau, Weiß): $\qtyrange{2,7}{3,5}{\volt}$
</right>

---
[question:EC503]
---

## Schottky-Diode

* Erlaubt eine hohe Schaltfrequenz
* Nur eine sehr niedrige Schwellenspannung von $\qty{0,4}{\volt}$ bis unter $\qty{0,1}{\volt}$ ist nötig

---
[question:EC504]
---

## Kennlinien

---
[question:EC506]
---
[question:EC507]
---
[question:EC508]
---
[question:EC505]
---

## Leitende Diode

<left>
* Eine Diode leitet immer dann, wenn die Spannung an der Anode um die Schwellenspannung positiver ist als an der Kathode
* Gilt auch für negative Spannungen
* In der Prüfung kommen nur Siliziumdioden mit $\qty{0,7}{\volt}$ Schwellenspannung vor
</left>
<right>
[picture:113:e_leitende_siliziumdiode:Spannungen an einer leitenden Siliziumdiode]
</right>

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

## LED Anwendung 

<left>
* Eine LED dient als Leuchtanzeige
</left>
<right>
[picture:324:e_led_schaltung:LED mit Vorwiderstand]
</right>

---
[question:EC514]
---
### Vorwiderstand

<left>
* Da die LED selbst kaum einen Widerstand hat, würde sie bei einem direkten Anschluss an eine Spannungsquelle wie ein Kurzschluss wirken
* Mit einem Vorwiderstand wird der Durchlassstrom begrenzt
</left>
<right>
[picture:324:e_led_schaltung:LED mit Vorwiderstand]
</right>

---
* Berechnung: $R = \dfrac{U_q - U_{LED}}{I_D}$
* $U_q$: Spannungsquelle
* $U_{LED}$: Schwellenspannung LED
* $I_D$: Durchlassstrom

---
[question:EC515]
---
[question:EC516]
---

## Z-Diode

<left>
* Normalerweise liegt die maximale Sperrspannung einer Diode bei ca. $\qty{1000}{\volt}$
* Bei Z-Dioden erfolgt ein Spannungsdurchbruch je nach Bauart zwischen $\qty{3}{\volt}$ und $\qty{100}{\volt}$
* Dienen zur Spannungsstabilisierung
</left>
<right>
[picture:560:_e_z_diode:Schaltzeichen Z-Diode]
</right>
<note>
* Früher nach Clarence Melvin Zener benannt
* Heute sind andere Effekte ausschlaggebend, aber Z-Diode blieb als Name
</note>

---
### Polung

<left>
* Z-Dioden werden mit Vorwiderstand in Sperrrichtung betrieben
</left>
<right>
[picture:549:e_z_diode_polung:Z-Diode korrekt in Sperrichtung eingesetzt]
</right>

---
[question:EC517]
---
[question:EC518]
---
[question:EC519]
---
[question:EC520]
---

### Vorwiderstand

<left>
[picture:753:e_z_diode_spannungsstabilisierung:Z-Diode zur Spannungsstabilisierung]
</left>
<right>
* $U_Z$ ist die Spannung, auf die die Z-Diode stabiliert
* $U_V = U_1 - U_Z = \qty{13,8}{\volt} - \qty{5}{\volt} = \qty{8,8}{\volt}$
* $R_V = \frac{U_V}{I} = \frac{\qty{8,8}{\volt}}{\qty{30}{\milli\ampere}} \approx \qty{293}{\ohm}$
</right>
---
[question:EC521]
---
[question:EC522]

<note>
* Ströme am Vorwiderstand addieren sich
* Kirchhoff'sche Regeln war noch nicht Thema
</note>