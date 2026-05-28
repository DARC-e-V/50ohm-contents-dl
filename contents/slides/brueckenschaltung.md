<left>
[picture:343:a_Brückenschaltung:Typische Brückenschaltung mit 4 Widerständen]
  
$\frac{R_1}{R_2} = \frac{R_3}{R_4}$
</left>
<right>
* Schaltung aus 4 Widerständen zur Widerstandsmessung
* Zwei parallel geschaltete Spannungsteiler
* Bei gleich großen Spannungsteilerverhältnissen fließt kein Strom über die Brücke
</right>
<note>
Messbrücke nach Wheatstone
</note>

---
[question:AD111]
---
[question:AD112]
---
[question:AD113]
--- style="font-size: 0.7em;"
#### Lösungsweg
* gegeben: $R_1 = R_4 = \qty{1}{\kilo\ohm}$
* gegeben: $R_2 = R_3 = \qty{10}{\kilo\ohm}$
* gegeben: $U = \qty{11}{\volt}$
* gesucht: $U_{AB}$

<fragment>
$\frac{U_A}{U} = \frac{R_1}{R_1 + R_2} \Rightarrow U_A = \frac{R_1}{R_1 + R_2} \cdot U = \frac{\qty{1}{\kilo\ohm}}{\qty{1}{\kilo\ohm} + \qty{10}{\kilo\ohm}} \cdot \qty{11}{\volt} = \qty{1}{\volt}$
</fragment>
<fragment>
$\frac{U_B}{U} = \frac{R_3}{R_3 + R_4} \Rightarrow U_B = \frac{R_3}{R_3 + R_4} \cdot U = \frac{\qty{10}{\kilo\ohm}}{\qty{10}{\kilo\ohm} + \qty{1}{\kilo\ohm}} \cdot \qty{11}{\volt} = \qty{10}{\volt}$
</fragment>
<fragment>
$U_{AB} = U_B - U_A = \qty{10}{\volt} - \qty{1}{\volt} = \qty{9}{\volt}$
</fragment>
