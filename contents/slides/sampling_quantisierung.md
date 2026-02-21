## Sampling: Von analog zu digital

* Analoge Signale werden mittels Sampling in digitale Werte umgewandelt  
* Abtastung erfolgt in definierten Zeitintervallen – nur Momentanzustände werden gemessen  
* Analoge Signale sind zeitkontinuierlich, da sie keine kleinste zeitliche Auflösung besitzen  
* Digitale Samples sind zeitdiskret, da ein festes Abtastintervall existiert

---

[include:quantisierung_und_sampling]

---

## Wertkontinuität vs. Wertdiskretheit

* Analoge Signale können beliebige Spannungswerte annehmen – sie sind wertkontinuierlich  
* Bei der Digitalisierung gibt es nur begrenzte Abstufungen (z. B. $\num{-128}$ bis $\num{+127}$) – Samples sind wertdiskret
* Zwischen zwei Spannungsstufen muss der A/D-Umsetzer eine Entscheidung treffen (Quantisierung)

---

## Praktisches Beispiel: Dimmer vs. Stufenschalter

* Ein analoger Dimmer erlaubt feine, stufenlose Helligkeitseinstellungen  
* Ein Stufenschalter (z. B. $\num{5}$ Stufen) ermöglicht nur feste Helligkeitswerte – Zwischenstufen sind nicht möglich
* Quantisierung: Auswahl der nächstpassenden Stufe, um den analogen Wert abzubilden

---

[question:AF601]

---

[question:AF603]

---

[question:AF602]

---

[question:AF604]