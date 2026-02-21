## Funktion des A/D-Umsetzers

* Wandelt analoge Eingangssignale in digitale Samples um  
* Essentiell für die Digitalisierung und Weiterverarbeitung von Signalen

---

### Aliasing und Antialiasing

* Abtasttheorem: Für fehlerfreie Rekonstruktion muss die Abtastrate $\gt 2 \cdot f_{max}$ betragen  
* Signale oberhalb der maximal verarbeitbaren Frequenz können als fehlerhafte Aliases erscheinen  
* Antialiasing-Filter (Tiefpass- oder Bandpassfilter) unterdrücken unerwünschte hohe Frequenzen  
* Schützen den A/D-Umsetzer vor fehlerhaften Aliasing-Effekten

---

[question:AF620]

---

### Taktgenerator (Abtastratengenerator)

* Erzeugt den exakten zeitlichen Takt für die Abtastung  
* Bestimmt, wie oft pro Sekunde ein Sample erfasst wird  
* Kann fest eingestellt oder durch Steuerung (z. B. Mikrocontroller) geregelt werden

---

### Quantisierung und Quantisierungsfehler

* Bei der A/D-Umsetzung werden analoge Amplitudenwerte in feste Stufen abgebildet  
* Dies führt zu einer wertdiskreten Darstellung des ursprünglich kontinuierlichen Signals  
* Quantisierungsfehler entstehen, da nicht alle Zwischenwerte exakt erfasst werden können

---

[question:AF607]

---

## Auflösung des A/D-Umsetzers

* Anzahl der möglichen digital darstellbaren Stufen  
* Wird in Bit angegeben (z. B. $\qty{8}{\bit} = \num{256}$ Stufen, $\qty{16}{\bit} = \num{65536}$ Stufen)
* Häufig wird die Hälfte der Werte für den positiven und die andere Hälfte für den negativen Bereich verwendet

---

[question:AF608]

---

### Jitter: Timing-Instabilitäten

* Jitter beschreibt kleine, zufällige Schwankungen in den Abtastzeitpunkten  
* Ein instabiler Abtastratengenerator führt zu zusätzlichen Rauscheffekten im digitalen Signal  
* Hoher technischer Aufwand ist nötig, um einen präzisen Takt zu gewährleisten

---

[question:AF621]
