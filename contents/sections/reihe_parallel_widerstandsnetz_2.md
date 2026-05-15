Die folgenden Aufgaben erfordern mehrere Rechenschritte bis zur Lösung. Dazu zerlegt man die Aufgabe in Teilbereiche, die zuerst berechnet und danach zusammengefasst werden. Bei dieser Vorgehensweise benötigt man keine großen Formeln  und gelangt zuverlässig zu dem richtigen Ergebnis. 

---
[question:AD106]

<margin>
Wenn alle Widerstände gleich groß sind und durch $R_3$ ein Strom von 1mA fließt, dann muss durch $R_2$ auch der gleiche Strom fließen, also auch 1mA. Beide Ströme müssen in der Summe durch $R_1$ fließen.
Alles klar?
Wie komme ich nun auf die Gesamtspannung $U$?
Diese Spannung muss so groß sein, dass durch den Gesamtwiderstand auch der Gesamtstrom fließen kann. Der Gesamtstrom entspricht dem Strom durch $R_1$.
Eine kleine Formel hilft nun bei der Berechnung. $U = I \cdot R = \qty{2}{\milli\ampere} \cdot \qty{15}{\kilo\ohm}$
</margin>
---
[question:AD107]

<margin>
Dieses Mal ist die Gesamtspannung angegeben und der Strom durch $R_3$ ist gesucht. Da alle Widerstände wieder $\qty{10}{\kilo\ohm}$ betragen, ergibt sich ein Gesamtwiderstand wie in der vorherigen Aufgabe.
Der Gesamtstrom lässt sich mit der bekannten Formel $I = \frac{U}{R}$ ermitteln.
Durch $R_3$ fließt wieder die Hälfte des Gesamtstroms, da $R_2$ und $R_3$ gleich groß sind.
</margin>

---
[question:AD108]
Achtung: Hier werden Kiloohm mit Milliampere multipliziert. Die Lösung ist aber in Milliwatt angegeben.
Hinweis: $\qty{1}{\milli\watt} = \qty{\frac{1}{1000}}{\watt} = \qty{0,001}{\watt}$; $\qty{1}{\watt} = \qty{1000}{\milli\watt}$
<margin>
Jetzt wird es etwas schwieriger, da nach der Leistung an $R_2$ gefragt wird.
Die Gesamtspannung und die Widerstandswerte entsprechen der vorherigen Aufgabe, deshalb fließt durch $R_2$ der gleiche Strom wie durch $R_3$ und entspricht dem halben Strom wie durch $R_1$.
Es ist zuerst der Gesamtstrom zu berechnen. $I = \frac{U}{R_{\mathrm{ges}}}$; danach $I_2 = \frac{I}{2}$
Die Leistung berechnet man mit der Formel $P = U \cdot I$. Hier müssen die Werte, wie sie an dem gesuchten Widerstand auftreten, eingesetzt werden.
Also $P_2 = U_2 \cdot I_2$
Oh, eines neues Problem. $U_2$ ist noch nicht bekannt, lässt sich aber berechnen. $U_2 = R_2 \cdot I_2 = \qty{10}{\kilo\ohm} \cdot \qty{0,5}{\milli\ampere}$
$P_2 = \qty{10}{\kilo\ohm} \cdot \qty{0,5}{\milli\ampere} \cdot \qty{0,5}{\milli\ampere}$; Da steckt doch die bekannte Formel $P = I^2 \cdot R$ dahinter.
(siehe Formelsammlung Seite 235 Mitte links -  Stichwort: Leistung)

</margin>

In der folgenden Widerstandsschaltung ist ein veränderbarer Widerstand (Potenziometer) eingebaut.
Der Widerstandswert kann von $\qty{0}{\kilo\ohm}$ bis auf maximal $\qty{1}{\kilo\ohm}$ verändert werden. Egal in welcher Stellung sich der Schleifer des Potenziometers befindet, der Gesamtwiderstand muss immer kleiner als $\qty{300}{\ohm}$ sein!

---
[question:AD109]
Lösung mit Rechnung:
$\qty{100}{\ohm}$ mit $\qty{200}{\ohm}$ parallel (Potenziometer steht auf $\qty{0}{\ohm}$) ergibt einen Gesamtwiderstand von $(\qty{100}{\ohm} \cdot \qty{200}{\ohm}) / (\qty{100}{\ohm} + \qty{200}{\ohm}) = \qty{67}{\ohm}$

$\qty{100}{\ohm}$ mit $\qty{1200}{\ohm}$ (Potenziometer steht auf $\qty{1}{\kilo\ohm}$) in Parallelschaltung ergibt einen Gesamtwiderstand von $\frac{\qty{100}{\ohm} \cdot \qty{200}{\ohm}}{\qty{100}{\ohm} + \qty{200}{\ohm}} = \qty{92}{\ohm}$. Zum Ergebnis muss noch der vorgeschaltete Widerstand mit $\qty{200}{\ohm}$ addiert werden.
<margin>
Begründung gewünscht?
Die Parallelschaltung von $\qty{100}{\ohm}$ mit $\qty{200}{\ohm}$ (Potenziometer steht auf $\qty{0}{\ohm}$) oder $\qty{100}{\ohm}$ mit $\qty{1,2}{\kilo\ohm}$ (Potenziometer steht auf $\qty{1}{\kilo\ohm}$) ergibt immer einen Wert kleiner als $\qty{100}{\ohm}$. Wenn noch $\qty{200}{\ohm}$ addiert werden, wird er Gesamtwiderstand nicht größer als $\qty{300}{\ohm}$ sein.
Es gibt nur eine Lösung, bei der dies erfüllt ist.
Ganz ohne Rechnung gelöst, UFB ! 
</margin>


Nun untersuchen wir eine Widerstandsschaltung mit 4 Widerständen, die oft verwendet wird. Jeweils zwei Spannungsteiler in Parallelschaltung ergeben eine sogenannte Brückenschaltung.
Brückenschaltungen werden z.B. in Widerstandsmessgeräten nach dem Prinzip einer Wheatstone Messbrücke angewendet.

-----
[question:AD110]
<margin>
Der Gesamtwiderstand lässt sich schrittweise ermitteln.
Zuerst wird die Reihenschaltung berechnet und ergibt einen Gesamtwiderstand von $\qty{220}{\ohm} + \qty{2,2}{\kilo\ohm} = \qty{2,42}{\kilo\ohm}$.
$\qty{2,42}{\kilo\ohm}$ liegen auch zwei Mal parallel, deshalb muss der Gesamtwiderstand die Hälfte betragen.
</margin>
<attention>
Das Ergebnis ist in Ohm angegeben.
</attention>

[picture:199:a_Widerstandsnetzwerk2:belasteter Spannungsteiler]
%todo Diese Frage gehört zum Abschnitt Spannungsteiler 2
In der Praxis ist ein Spannungsteiler oft durch $R_\text{L}$ belastet, wie es im Schaltbild zu sehen ist.


---
[question:AD114]
<margin>
 Die Spannung $U_2$ muss dann im Vergleich zum unbelasteten Spannungsteiler kleiner werden .
 $U_2$ kann man ermitteln, indem zuerst der Gesamtwiderstand $R_{2L}$ der Parallelschaltung von $R_2$ und $R_\text{L}$ berechnet wird. Danach berechnet man den Gesamtwiderstand $R_{\mathrm{ges}}$ der Schaltung und mit $I = \frac{U}{R_{\mathrm{ges}}}$ den Gesamtstrom.  Dieser Strom fließt auch durch den $R_{2L}$ und bewirkt den Spannungsfall $U_2$.

 Lösungshilfen:
AD 106: $\qty{30}{\volt}$
AD 107: $\qty{0,5}{\milli\ampere}$
AD 108: $\qty{2,5}{\milli\watt}$
AD 109: $\qtyrange{267}{292}{\ohm}$
AD 110: $\qty{1210}{\ohm}$
AD 114: $\qty{1,8}{\volt}$
</margin>
<tip>
  Es gibt auch ein Experiment.
</tip>

<margin>
| Zusammenfassung |
|Aufgabe in Teilbereiche zerlegen  |
|Teilbereiche berechnen |
|Kontrollüberlegung, ob das Ergebnis stimmen kann |
[table:a_Widerstandsnetzwerke 2:Zusammenfassung]
</margin>
