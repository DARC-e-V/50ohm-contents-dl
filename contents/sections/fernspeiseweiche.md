An den Antennen montierte, abgesetzte Vorverstärker oder Empfangskonverter benötigen eine Gleichspannungsversorgung.
Um eine zusätzliche Gleichspannungsversorgungsleitung einzusparen, kann die Versorgungsspannung auch über das Koaxialkabel, parallel zum HF-Signal, übertragen werden, ohne dass sich die beiden Signale gegenseitig stören. Zur Einspeisung der Gleichspannung in das Koaxialkabel wird deshalb eine Fernspeiseweiche oder englisch BIAS-T eingesetzt.
Die übersichtliche Schaltung enthält neben den Anschlüssen nur 3 Bauteile.

[picture:399:a_Bias T:BIAS - T]

[question:AD323]
Schaltungsbeschreibung:
Ein BIAS-T erkennt man daran, dass auf einer Seite ein Signal zum Empfänger (Rx) führt und auf der anderen Seite ein Signal von einem Vorverstärker oder Empfangskonverter (LNA) eingekoppelt wird. Die Versorgungsgleichspannung des LNA  (DC-Signal) wird über eine Induktivität auf den Innenleiter des Koaxialkabels geführt.
%todo Induktivität ist im Bild 399 nicht bezeichnet. sollte L1 sein
Der Koppelkondensator $C_1$ soll das Gleichspannungssignal vom Rx-Eingang fernhalten. Der Rx-Eingang ist zur Vermeidung statischer Aufladungen bei manchen Geräten über eine Drosselspule mit Masse (Null Volt) verbunden. Würde der Kondensator $C_1$ fehlen, könnte die Gleichspannung gegen Masse kurzgeschlossen werden.

---
[question:AD322]

<margin>
[photo:288:a_Bias T Platine:BIAS - T Platine - mit KiCAD erstellt]
So könnte die praktische Umsetzung des abgebildeten Schaltbildes in eine Platine aussehen. $C_2$ und $C_3$ sind Abblockkondensatoren für unterschiedliche Frequenzbereiche, damit die Funktion über einen großen Frequenzbereich gewährleistet ist. $L_1$ dient zur Zuführung der Gleichspannung und muss für den Laststrom gezielt dimensioniert werden.
</margin>

---
[question:AD324]
<margin>
Der Abblockkondensator $C_2$ auf der Gleichspannungseite soll HF-Spannung unterdrücken. Er muss so gewählt werden, dass er bei der HF-Nutzfrequenz einen Blindwiderstand kleiner 1 Ohm darstellt.
</margin>
---
[question:AD325]
<margin>
Die Spule zwischen DC-Seite (Gleichspannungsseite z.B. $\qty{12}{\volt}$) und der HF-Seite (z.B. $\qty{10}{\giga\hertz}$ Empfangssignal) soll  Hochfrequenzanteile nicht zur DC-Seite durchlassen. Es handelt sich deshalb um eine Drosselspule, die bei der Nutzfrequenz hochohmig wirken muss (z.B. $X_\text{L} = \qty{10}{\kilo\ohm}$). Durch diese Drosselspule fließt der Versorgungstrom für den Vorverstärker oder Konverter (LNA). Der Drahtdurchmesser der Drosselspule muss so groß sein, dass der Versorgungsgleichstrom keine Erwärmung der Drosselspule bewirkt
</margin>

<margin>
| Zusammenfassung |
|DC und AC über eine Leitung |
|Trennkondensator für DC notwendig |
[table:a_Fernspeiseweiche:Zusammenfassung]
</margin>