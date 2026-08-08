In der Klasse N haben wir das *S-Meter* bereits sowohl in seiner analogen Variante (Abb. [ref:a_s_meter_analog]) als auch in seiner digitalen Variante (Abb. [ref:a_s_meter_digital]) kennengelernt. Es dient dazu, die Stärke des am Empfängereingang anliegenden HF-Signals anzuzeigen.

Die Skala eines S-Meters reicht üblicherweise von S1 bis S9. Eine Änderung um eine S-Stufe entspricht dabei $\qty{6}{\dB}$. Stärkere Signale oberhalb von S9 werden nicht mehr in weiteren S-Stufen, sondern in Dezibel über S9 angegeben, beispielsweise als „S9 + $\qty{20}{\dB}$“.

Da die Dezibel-Skala logarithmisch ist, entspricht eine Erhöhung um $\qty{6}{\dB}$ einer Verdopplung der Eingangsspannung beziehungsweise einer Vervierfachung der Eingangsleistung. Umgekehrt entspricht eine Verringerung um $\qty{6}{\dB}$ einer Halbierung der Spannung beziehungsweise einer Viertelung der Leistung.

<margin>
[picture:578:a_s_meter_digital:Nummer 2 zeigt das digitale S-Meter eines TRX]
[picture:420:a_s_meter_analog:Analoges S-Meter eines TRX]
</margin>

[question:AF101]
[question:AF104]
[question:AF103]
[question:AA113]
[question:AF102]

---

Im Kurzwellenbereich bis $\qty{30}{\mega\hertz}$ entspricht ein S-Wert von S9 genau $\qty{50}{\micro\volt}$ an $\qty{50}{\ohm}$.
Ab dem VHF-Bereich ($\qty{144}{\mega\hertz}$) entspricht ein S-Wert von S9 genau $\qty{5}{\micro\volt}$ an $\qty{50}{\ohm}$.

<tip>
S-Meter von Kurzwellengeräten zeigen meist nur Werte um S9 halbwegs zuverlässig an, da diese oft nur auf diesen einen Wert kalibriert werden. Insbesondere kleinere S-Werte werden nur sehr ungenau angezeigt. Die logarithmische Charakteristik eines S-Meters wird oft nur unzureichend interpoliert. Einen S-Wert von S0 gibt es hierbei definitionsgemäß nicht, da immer ein Grundrauschen oder Eigenrauschen des Empfängers vorhanden ist. Zeigt das S-Meter keinen Wert im unteren Bereich an, so ist das empfangene Signal sehr schwach, jedoch hat es nie den Wert S0. Dieser sollte daher auch nicht übermittelt werden. 
</tip>

[question:AA114]
[question:AF105]