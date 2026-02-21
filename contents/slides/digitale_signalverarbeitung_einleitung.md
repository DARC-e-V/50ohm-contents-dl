* Im Bereich der Funktechnik spricht man bei Geräten, die mittels digitaler Signalverarbeitung arbeiten von sogenannten SDR-Geräten.
* *SDR* steht dabei  für Software Defined Radio.
* In diesen Geräten ist zumindest ein Teil der Signalverarbeitung in Software realisiert.
* Dieses hat einen Kostenvorteil und bringt eine große Flexibilität mit sich.

---
[question:EF603]
---
## A/D-Umsetzer

* Damit die Daten digital verarbeitet werden können, müssen sie zunächst digitalisiert werden.
* Dazu wird das analoge Signal mittels eines Analog-Digital Umsetzers (A/D-Umsetzer) in digitale Werte umgesetzt.

---
<left>
* Hierbei wird das analoge Signal in festen Zeitintervallen abgetastet und in einem digitalen Wertebereich (z.B. von $\num{-128}$ bis $\num{+127}$) abgebildet.
* Die einzelnen gemessenen Signalwerte werden als Samples (Proben) bezeichnet.
</left>
<right>
[picture:411:e_digitale_signalverarbeitung:Einfache Darstellung einer Sinuswelle aus $\num{16}$ Samples und $\num{7}$ Werten]
</right>
<note>
* Mehr dazu in Klasse A
</note>

---
[question:EF602]
---
## D/A-Umsetzer

* Nach der digitalen Verarbeitung des Signals wird es in einem Digital-Analog-Umsetzer (D/A-Umsetzer) wieder in ein analoges Signal verwandelt.

---
[question:EF601]