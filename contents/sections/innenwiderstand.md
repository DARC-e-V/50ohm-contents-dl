Ein gutes Labornetzgerät oder auch ein Transveiver-Netzgerät beinhalten eine elektronische Spannungsregelung und eine Strombegrenzung. Die Abbildung [ref:a_vsource_schematic] zeigt ein Ersatzschaltbild einer Spannungsquelle.

[picture:1018:a_vsource_schematic:Ersatzschaltbild Spannungsquelle]

Wird eine reale Spannungsquelle mit $R_\text{L}$ belastet, so sinkt die Klemmenspannung $U_\text{k}$. Grund dafür ist der vorhandene Innenwiderstand $R_\text{i}$ dieser Spannungsquelle. Da die Quellenspannung $U_\text{q}$ im Leerlauf, also ohne Belastung $U_\text{q}=U_\text{L}$ ist, nennt man diese auch Leerlaufspannung. Bleibt die Klemmenspannung bei Belastung konstant, dann spricht man von Spannungsanpassung.

Mit einem Multimeter ist der Innenwiderstand nicht messbar, man kann ihn aber rechnerisch ermitteln.
$R_\text{i} = \frac{\Delta U}{\Delta I}$

(siehe Formelsammlung Seite 234 Mitte links -  Stichwort: Innenwiderstand)

Zur Berechnung werden zwei Belastungsfälle benötigt:
1. Leerlauf; $I = \qty{0}{\ampere}$
2. Belastung mit $R_\text{L}$; $I_\text{L} = \frac{U_\text{L}}{R_\text{L}}$
Über die Spannungsveränderung ($\Delta U$) an den Klemmen und die Laststromveränderung ($\Delta I$), kann der Innenwiderstand berechnet werden.

* Ideale Spannungsquellen sollen einen sehr niedrigen Innenwiderstand $R_\text{i} \ll R_\text{L}$ aufweisen, im Idealfall: $\qty{0}{\ohm}$, dann bleibt die Ausgangsspannung bei Belastung unverändert. ($\Delta U = \qty{0}{\volt}$);  $R_\text{i} = \frac{\Delta U}{\Delta I} = \frac{0}{x} = \qty{0}{\ohm}$

% Kommentar von DK1KC: ungünstige Darstellung : In der Abbildung [ref:a_vsource_kennlinie] kann man erkennen, wie sich $U_\text{k}$ zu $I$ in Abhängigkeit vom Innenwiderstand $R_\text{i}$ verhält. Bei  $R_\text{L}=\qty{0}{\ohm}$ fließt an den Klemmen ein Kurzschlussstrom $I_\text{k}$.

% todo ungünstige Darstellung [photo:183:a_vsource_kennlinie:Kennlinie einer Konstantspannungsquelle]

% geändert von DK1KC; vorher: Wir stellen fest das unsere Spannungsquelle einen niedrigen Innenwiderstand hat.


<indepth>
Wechselspannungsquellen, z.B. Sinusgeneratoren besitzen auch einen Innenwiderstand, der an der Ausgangsbuchse angeben ist.
Beispiele:
[photo:292:Sinusgenerator 50 Ohm:Sinusgenerator mit 50 Ohm Innenwiderstand]
[photo:293:Sinusgenerator 200 Ohm:Sinusgenerator mit 200 Ohm Innenwiderstand]
</indepth>


% geändert von DK1KC; vorher: Eine Stromquelle, ist eine Quelle mit einem Quellenstrom $I_q$ und einem dazu parallel liegendem Innenwiderstand $R_\text{i}$. In der Abbildung [ref:a_isource_schematic] ist das Ersatzschaltbild dargestellt.

% todo [photo:184:a_isource_schematic:Ersatzschaltbild Stromquelle]

% geändert von DK1KC; vorher: Bei einem Kurzschluss am Lastausgang ist $I=I_q$ und die Spannung annähernd $U_\text{L}=\qty{0}{\volt}$. Der Stom im Innenwiderstand ist ebenfalls annähernd $I_i=\qty{0}{\ampere}$. Dies liegt daran, dass der $R_\text{i}$ bei einer Stromquelle sehr hochohmig sein soll. Daher gilt auch im Leerlauf $I_i=I_q$ und der Strom $I$ ist ohne Last $\qty{0}{\ampere}$.


Betrachtung einer Konstantstromquelle am Beispiel eines Labornetzgerätes

[photo:298:a_Strombegrenzung:Labornetzgerät mit eingestellter Strombegrenzung auf $\qty{500}{\milli\ampere}$]
Bei Kurzschluss an den Ausgangsklemmen fließt der eingestellte maximale Strom.

In Labornetzgeräten ist eine Strombegrenzung eingebaut, d.h. übersteigt der Laststrom eine maximale Stromstärke, wird die Klemmenspannung so abgesenkt, dass der Laststrom konstant bleibt. Dies entspricht der Funktion einer Konstantstromquelle.

$R_\text{i} = \frac{\Delta U}{\Delta I}$; ($\Delta I \to \qty{0}{\ampere}$);   $R_\text{i} = \frac{\Delta U}{\Delta I} \to \qty{\infty}{\ohm}$
* Ideale Stromquellen sollen einen sehr hohen Innenwiderstand $R_\text{i} \gg R_\text{L}$ aufweisen. Idealfall: "unendlich" Ohm, dann bleibt der Laststrom bei Änderung des  Lastwiderstandes konstant, deshalb spricht man auch von Stromanpassung.
---
[question:AB201]

Soll ein Sender die optimale Leistung an die Antenne abgeben, dann spricht man von Leistungsanpassung.
% ungünstig formuliert (DK1KC)in einer Quelle die gleiche Leistung wie an der Last umgesetzt werden, muss Innen- und Lastwiderstand gleich sein. Wir sprechen bei $R_\text{i} \gg R_\text{L}$ von einer Lastanpassung. Dies wird uns bei der Sender- und Antennentechnik nochmal beschäftigen.

Hierbei gilt: $R_\text{i} = R_\text{L}$


----
[question:AG401]
<margin>
[picture:937:a_Leistungsanpassung:Optimale Ausgangsleistung bei 50 Ohm Lastwiderstand]
</margin>
  

[question:AB202]
[question:AB203]
[question:AB204]
<margin>
 Lösungshilfe
 AG 401: $R_\text{i} = R_\text{L} = \qty{50}{\ohm}$
 AB 202: $R_\text{L} = R_\text{i}$
 AB 203: $R_\text{i} \ll R_\text{L}$
 AB 204: $R_\text{i} \gg R_\text{L}$
  
</margin>

<margin>
|c: Zusammenfassung | c: Innenwiderstand |
| Spannungsanpassung bei einer Konstantspannungsquelle| $R_\text{i}$ ist sehr niederohmig ; theoretisch  $\qty{0}{\ohm}$;  $R_\text{i} \ll R_\text{L}$ identisch mit $R_\text{L} \gg R_\text{i}$|
|Stromanpassung bei einer Konstantstromquelle|$R_\text{i}$ ist sehr hochohmig;  $R_\text{i} \gg R_\text{L}$ identisch mit $R_\text{L} \ll R_\text{i}$ |
| Leistungsanpassung bei Verstärkern| $R_\text{L} = R_\text{i}$|
[table:a_Innenwiderstand Zusammenfassung:Zusammenfassung zum Innenwiderstand]
</margin>

  
---

Nun wollen wir einmal anhand eines Beispieles den Innenwiderstand einer Gleichspannungsquelle berechnen. 
[question:AB206]

Die Leerlaufspannung $U_\text{L}$, also ohne Belastung unseres Netzteils, beträgt $\qty{13,5}{\volt}$. Dabei fließt kein Laststrom $I_\text{L}$. Beim Senden mit unserem Funkgerät wird ein Strom  $I_\text{L}$ von $\qty{0,9}{\ampere}$ abgegeben und die Ausgangsspannung  $U_\text{L}$  sinkt nun, wegen des Innenwiderstandes, auf $\qty{12,4}{\volt}$ ab.

$R_\text{i} = \frac{\Delta U_\text{L}}{\Delta I_\text{L}} = \frac{\qty{13,5}{\volt} - \qty{12,4}{\volt}}{\qty{0,9}{\ampere} - \qty{0}{\ampere}} = \frac{\qty{1,1}{\volt}}{\qty{0,9}{\ampere}} = \qty{1,22}{\ohm}$ Dieser Wert ist in der Praxis noch zu hoch.
Praxisnäher sind die Ergebnisse der folgenden Aufgaben.

---
[question:AB205]

<tip>
Hier ist der Laststrom  $I_\text{L}$ zuerst zu berechnen!
$I_\text{L} = \frac{U_\text{L}}{R_\text{L}}$
</tip>


[question:AB207]

---
[question:AB208]

<margin>
 Lösungshinweis:
AB 205:   $I_\text{L}=\frac{U_\text{L}}{R_\text{L}} = \frac{\qty{4,8}{\volt}}{\qty{1,2}{\ohm}} = \qty{4}{\ampere}$
  $R_\text{i} = \frac{\Delta U}{\Delta I} = \frac{\qty{5,0}{\volt} - \qty{4,8}{\volt}}{\qty{4}{\ampere} - \qty{0}{\ampere}} = \frac{\qty{0,2}{\volt}}{\qty{4}{\ampere}} = \qty{0,05}{\ohm} = \qty{50}{\milli\ohm}$
AB 206:  siehe Beispielrechnung
AB 207:  $R_\text{i} = \frac{\Delta U}{\Delta I} = \frac{\qty{13,5}{\volt} - \qty{13,0}{\volt}}{\qty{2,0}{\ampere} - \qty{0}{\ampere}} = \frac{\qty{0,5}{\volt}}{\qty{2,0}{\ampere}} = \qty{0,25}{\ohm} = \qty{250}{\milli\ohm}$
AB 208: $R_\text{i} = \frac{\Delta U}{\Delta I} = \frac{\qty{13,8}{\volt} - \qty{13,6}{\volt}}{\qty{20,0}{\ampere} - \qty{0}{\ampere}} = \frac{\qty{0,2}{\volt}}{\qty{20,0}{\ampere}} = \qty{0,01}{\ohm} = \qty{10}{\milli\ohm}$
  
</margin>