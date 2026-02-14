Die folgenden Aufgaben erfordern mehrere Rechenschritte bis zur Lösung. Dazu zerlegt man die Aufgabe in Teilbereiche, die zuerst berechnet und danach zusammengefasst werden. Bei dieser Vorgehensweise benötigt man keine großen Formeln  und gelangt zuverlässig zu dem richtigen Ergebnis. 

---
[question:AD106]

<margin>
Wenn alle Widerstände gleich groß sind und durch $R_3$ ein Strom von 1mA fließt, dann muss durch $R_2$ auch der gleiche Strom fließen, also auch 1mA. Beide Ströme müssen in der Summe durch $R_1$ fließen.
Alles klar?
Wie komme ich nun auf die Gesamtspannung U?
Diese Spannung muss so groß sein, dass durch den Gesamtwiderstand auch der Gesamtstrom fließen kann. Der Gesamtstrom entspricht dem Strom durch $R_1$.
Eine kleine Formel hilft nun bei der Berechnung. U = I * R = 2mA * 15 kOhm
</margin>
---
[question:AD107]

<margin>
Dieses Mal ist die Gesamtspannung angegeben und der Strom durch $R_3$ ist gesucht. Da alle Widerstände wieder 10 kOhm betragen, ergibt sich ein Gesamtwiderstand wie in der vorherigen Aufgabe.
Der Gesamtstrom lässt sich mit der bekannten Formel $I = \frac {U}{R}$ ermitteln.
Durch $R_3$ fließt wieder die Hälfte des Gesamtstroms, da $R_2$ und $R_3$ gleich groß sind.
</margin>

---
[question:AD108]
Achtung: Hier werden KiloOhm mit Milliampere multipliziert. Die Lösung ist aber in Milliwatt angegeben.
Hinweis: 1mW = 1/1000 W = 0,001 W; 1 W = 1000 mW
<margin>
Jetzt wird es etwas schwieriger, da nach der Leistung an $R_2$ gefragt wird.
Die Gesamtspannung und die Widerstandswerte entsprechen der vorherigen Aufgabe, deshalb fließt durch $R_2$ der gleiche Strom wie durch $R_3$ und entspricht dem halben Strom wie durch $R_1$.
Es ist zuerst der Gesamtstrom zu berechnen. $I = \frac {U}{R_{ges}}$ ;  danach $I_2 = \frac {I}{2}$
Die Leistung berechnet man mit der Formel P = U x I. Hier müssen die Werte, wie sie an dem gesuchten Widerstand auftreten, eingesetzt werden.
Also $P_2$ = $U_2$ * $I_2$ 
Oh, eines neues Problem. $U_2$ ist noch nicht bekannt, läßt sich aber berechnen. $U_2$ = $R_2$ * $I_2$ = 10 kOhm * 0,5 mA
$P_2$ = 10 kOhm * 0,5mA * 0,5 mA;  Da steckt doch die bekannte Formel $P = I^2 * R$ dahinter.
(siehe Formelsammlung Seite 235 Mitte links -  Stichwort: Leistung)

</margin>

In der folgenden Widerstandsschaltung ist ein veränderbarer Widerstand (Potenziometer) eingebaut.
Der Widerstandswert kann von 0 kOhm bis auf maximal 1 kOhm verändert werden. Egal in welcher Stellung sich der Schleifer des Potenziometers befindet, der Gesamtwiderstand muss immer kleiner als 300 Ohm sein!

---
[question:AD109]
Lösung mit Rechnung:
100 Ohm mit 200 Ohm  parallel  (Potenziometer steht auf 0 Ohm) ergibt einen Gesamtwiderstand von (100 Ohm * 200 Ohm)  / (100 Ohm + 200 Ohm) = 67 Ohm

100 Ohm mit 1200 Ohm (Potenziometer steht auf 1 kOhm) in Parallelschaltung ergibt einen Gesamtwiderstand von $\frac {100 Ohm * 200 Ohm}{(100 Ohm + 200 Ohm)} = 92 Ohm . Zum Ergebnis muss noch der vorgeschaltete Widerstand mit 200 Ohm addiert werden.
<margin>
Begründung gewünscht?
Die Parallelschaltung von 100 Ohm mit 200 Ohm (Potenziometer steht auf 0 Ohm) oder 100 Ohm mit 1,2 kOhm (Potenziometer steht auf 1 kOhm) ergibt immer einen Wert kleiner als 100 Ohm. Wenn noch 200 Ohm addiert werden, wird er Gesamtwiderstand nicht größer als 300 Ohm sein.
Es gibt nur eine Lösung, bei der dies erfüllt ist.
Ganz ohne Rechnung gelöst, UFB ! 
</margin>


Nun untersuchen wir eine Widerstandsschaltung mit 4 Widerständen, die oft verwendet wird. Jeweils zwei Spannungsteiler in Parallelschaltung ergeben eine sogenannte Brückenschaltung.
Brückenschaltungen werden z.B. in Widerstandsmessgeräten nach dem Prinzip einer Wheatstone Messbrücke angewendet.

-----
[question:AD110]
<margin>
Der Gesamtwiderstand lässt sich schrittweise ermitteln.
Zuerst wird die Reihenschaltung berechnet und ergibt einen Gesamtwiderstand von 220 Ohm + 2,2 kOhm = 2,42 kOhm.
2,42 kOhm liegen auch zwei Mal parallel, deshalb muss der Gesamtwiderstand die Hälfte betragen.
</margin>
<attention>
Das Ergebnis ist in Ohm angegeben.
</attention>

[picture:199:a_Widerstandsnetzwerk2:belasteter Spannungsteiler]
%todo Diese Frage gehört zum Abschnitt Spannungsteiler 2
In der Praxis ist ein Spannungsteiler oft durch $R_L$ belastet, wie es im Schaltbild zu sehen ist.


---
[question:AD114]
<margin>
 Die Spannung $U_2$ muss dann im Vergleich zum unbelasteten Spannungsteiler kleiner werden .
 $U_2$ kann man ermitteln, indem zuerst der Gesamtwiderstand $ R_{2L}$ der Parallelschaltung von $R_2$ und $R_L$ berechnet wird. Danach berechnet man den Gesamtwiderstand $R_{ges}$ der Schaltung und mit I = $\frac {U}{R_{ges}}$ den Gesamtstrom.  Dieser Strom fließt auch durch den $R_{2L}$ und bewirkt den Spannungsfall $U_2$. 

 Lösungshilfen:
AD 106: 30 V
AD 107: 0,5 mA
AD 108: 2,5 mW
AD 109: 267 - 292 Ohm
AD 110: 1210 Ohm
AD 114: 1,8 V
</margin>
<tip>
  Es gibt auch ein Experiment.
</tip>

<margin>
| Zusammenfassung |
|Aufgabe in Teilbereiche zerlegen  |
|Teilbereiche berechnen |
|Kontrollüberlegung, ob das Ergenis stimmen kann |
[table:a_Widerstandsnetzwerke 2:Zusammenfassung]
</margin>
