Ein gutes Labornetzgerät oder auch ein Transveiver-Netzgerät beinhalten eine elektronische Spannungsregelung und eine Strombegrenzung. Die Abbildung [ref:a_vsource_schematic] zeigt ein Ersatzschaltbild einer Spannungsquelle.

[picture:1018:a_vsource_schematic:Ersatzschaltbild Spannungsquelle]

Wird eine reale Spannungsquelle mit $R_L$ belastet, so sinkt die Klemmenspannung $U_k$. Grund dafür ist der vorhandene Innenwiderstand $R_i$ dieser Spannungsquelle. Da die Quellenspannung $U_q$ im Leerlauf, also ohne Belastung $U_q$=$U_L$ ist, nennt man diese auch Leerlaufspannung. Bleibt die Klemenspannung bei Belastung konstant, dann spricht man von Spannungsanpassung.

Mit einem Multimeter ist der Innenwiderstand nicht messbar, man kann ihn aber rechnerisch ermitteln.
$R_i$ = $\frac{\Delta U}{\Delta I}$

(siehe Formelsammlung Seite 234 Mitte links -  Stichwort: Innenwiderstand)

Zur Berechnung werden zwei Belastungsfälle benötigt:
1. Leerlauf; I = 0 A
2. Belastung mit $R_L \  $;  $I_L$ =$\frac{U_L}{R_L}$
Über die Spannungsveränderung ($\Delta U$) an den Klemmen und die Laststromveränderung ($\Delta I$) , kann der Innenwiderstand berechnet werden. 

* Ideale Spannungsquellen sollen einen sehr niedrigen Innenwiderstand $R_i$$\ll$$R_L$ aufweisen, im Idealfall: 0 Ohm, dann bleibt die Ausgangsspannung bei Belastung unverändert. ($\Delta U$ = 0 V);  $R_i$ = $\frac{\Delta U}{\Delta I}$ = $ \frac {0} {xxx} = 0 \ \Omega$

% Kommentar von DK1KC: ungünstige Darstellung : In der Abbildung [ref:a_vsource_kennlinie] kann man erkennen, wie sich $U_k$ zu $I$ in Abhängigkeit vom Innenwiderstand $R_i$ verhält. Bei  $R_L$=0 Ohm fließt an den Klemmen ein Kurzschlußstrom $I_k$. 

% todo ungünstige Darstellung [photo:183:a_vsource_kennlinie:Kennlinie einer Konstantspannungsquelle]

% geändert von DK1KC; vorher: Wir stellen fest das unsere Spannungsquelle einen niedrigen Innenwiderstand hat.


<indepth>
Wechselspannungsquellen, z.B. Sinusgeneratoren besitzen auch einen Innenwiderstand, der an der Ausgangsbuchse angeben ist.
Beispiele:
[photo:292:Sinusgenerator 50 Ohm:Sinusgenerator mit 50 Ohm Innenwiderstand]
[photo:293:Sinusgenerator 200 Ohm:Sinusgenerator mit 200 Ohm Innenwiderstand]  
</indepth>


% geändert von DK1KC; vorher: Eine Stromquelle, ist eine Quelle mit einem Quellenstrom $I_q$ und einem dazu parallel liegendem Innenwiderstand $R_i$. In der Abbildung [ref:a_isource_schematic] ist das Ersatzschaltbild dargestellt.

% todo [photo:184:a_isource_schematic:Ersatzschaltbild Stromquelle]

% geändert von DK1KC; vorher: Bei einem Kurzschluss am Lastausgang ist $I$=$I_q$ und die Spannung annähernd $U_L$=0 V. Der Stom im Innenwiderstand ist ebenfalls annähernd $I_i$=0 A. Dies liegt daran, dass der $R_i$ bei einer Stromquelle sehr hochohmig sein soll. Daher gilt auch im Leerlauf $I_i$=$I_q$ und der Strom $I$ ist ohne Last 0 A.


Betrachtung einer Konstantstromquelle am Beispiel eines Labornetzgerätes

[photo:298:a_Strombegrenzung:Labornetzgerät mit eingestellter Strombegrenzung auf 500 mA]
Bei Kurzschluss an den Ausgangsklemmen fließt der eingestellte maximale Strom.

In Labornetzgeräten ist eine Strombegrenzung eingebaut, d.h. übersteigt der Laststrom eine maximale Stromstärke, wird die Klemmenspannung so abgesenkt, dass der Laststrom konstant bleibt. Dies entspricht der Funktion einer Konstantstromquelle.

$R_i$ = $\frac{\Delta U}{\Delta I}$; ($\Delta I$ = "Null" A);   $R_i$  =  $\frac{\Delta U}{"Null"}$ = "unendlich"  $\ \Omega$
* Ideale Stromquellen sollen einen sehr hohen Innenwiderstand $R_i$$\gg$$R_L$ aufweisen. Idealfall: "unendlich" Ohm, dann bleibt der Laststrom bei Änderung des  Lastwiderstandes konstant, deshalb spricht man auch von Stromanpassung.
---
[question:AB201]

Soll ein Sender die optimale Leistung an die Antenne abgeben, dann spricht man von Leistungsanpassung.
% ungünstig formuliert (DK1KC)in einer Quelle die gleiche Leistung wie an der Last umgesetzt werden, muss Innen- und Lastwiderstand gleich sein. Wir sprechen bei $R_i$$\gg$$R_L$ von einer Lastanpassung. Dies wird uns bei der Sender- und Antennentechnik nochmal beschäftigen.

Hierbei gilt: $R_i$ = $R_L$ 


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
 AG 401:  $R_i$ = $R_L$ = 50 Ohm
 AB 202:  $R_L$ =$R_i$  
 AB 203: $R_i$$\ll$$R_L$
 AB 204: $R_i$$\gg$$R_L$
  
</margin>

<margin>
|c: Zusammenfassung | c: Innenwiderstand |
| Spannungsanpassung bei einer Konstantspannungsquelle| $R_i$ =  "sehr niederhohmig" ; theoretisch  $0\ \Omega$;  $R_i$$\ll$$R_L$ identisch mit $R_L$$\gg$$R_i$| 
|Stromanpassung bei einer Konstantstromquelle|$R_i$ =  "sehr hochohmig" ;  $R_i$$\gg$$R_L$ identisch mit $R_L$$\ll$$R_i$ |
| Leistungsanpassung bei Verstärkern| $R_L$ = $R_i$|
[table:a_Innenwiderstand Zusammenfassung:Zusammenfassung zum Innenwiderstand]
</margin>

  
---

Nun wollen wir einmal anhand eines Beispieles den Innenwiderstand einer Gleichspannungsquelle berechnen. 
[question:AB206]

Die Leerlaufspannung $U_L$, also ohne Belastung unseres Netzteils, beträgt 13,5 V. Dabei fließt kein Laststrom $I_L$. Beim Senden mit unserem Funkgerät wird ein Strom  $I_L$ von 0,9 A abgegeben und die Ausgangsspannung  $U_L$  sinkt nun, wegen des Innenwiderstandes, auf 12,4 V ab.

$R_i$ = $\frac{\Delta U_L}{\Delta I_L}$ = $ \frac {13,5\ V - 12,4\ V}{0,9\ A - 0\ A} $ = $ \frac {1,1\ V}{0,9\ A}$ = $1,22 \  \Omega$ Dieser Wert ist in der Praxis noch zu hoch. 
Praxisnäher sind die Ergebnisse der folgenden Aufgaben.

---
[question:AB205]

<tip>
Hier ist der Laststrom  $I_L$ zuerst zu berechnen!
$I_L = \frac{U_L}{R_L}$
</tip>


[question:AB207]

---
[question:AB208]

<margin>
 Lösungshinweis:
AB 205:   $I_L=\frac{U_L}{R_L}$ =  $ \frac {4,8\  V}{1,2\  \Omega}$ = 4 A
  $R_i$ = $\frac{\Delta U}{\Delta I}$ = $ \frac {5,0\ V - 4,8\ V}{4\ A - 0\ A} $ = $ \frac {0,2\ V}{4\ A}$ = $0,05 \  \Omega$ = $50 \ m\Omega$
AB 206:  siehe Beispielrechnung
AB 207:  $R_i$ = $\frac{\Delta U}{\Delta I}$ = $ \frac {13,5\ V - 13,0\ V}{2,0\ A - 0\ A} $ = $ \frac {0,5\ V}{2,0\ A}$ = $0,25 \  \Omega$ = $250 \ m\Omega$
AB 208: $R_i$ = $\frac{\Delta U}{\Delta I}$ = $ \frac {13,8\ V - 13,6\ V}{20,0\ A - 0\ A} $ = $ \frac {0,2\ V}{20,0\ A}$ = $0,01 \  \Omega$  = $10 \ m\Omega$
  
</margin>