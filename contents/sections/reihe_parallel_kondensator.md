Kondensatoren werden in vielen Anwendungen in Reihenschaltung, Parallelschaltung oder auch gemischter Schaltungstechnik eingesetzt. Die Parallelschaltung ist einfacher zu verstehen, deshalb betrachten wir sie zuerst.

Durch die Parallelschaltung stehen sich mehr Platten gegenüber und somit erhöht sich die Plattenoberfläche proportional. Entsprechend erhöht sich auch die Kapazität in der Gesamtschaltung.

<margin>
[picture:822:e_3C-parallel: Parallelschaltung von 3 Kondensatoren]
</margin>

---

Bei einer Parallelschaltung von gleich großen Kondensatoren verdoppelt sich die Kapazität, die Spannungsfestigkeit bleibt gleich. Selbstverständlich kann man die Gesamtkapazität berechnen. Die Formel finden wir in der Formelsammlung:

$C_{\mathrm{ges}} = C_{1} + C_{2} + C_{3} + \dots$

<tip>
Die Gesamtkapazität ist bei der Parallelschaltung immer größer als die kleinste Einzelkapazität.
</tip>

Bei der folgenden Aufgabe ist eine zusätzliche Schwierigkeit zu finden, da die Vorsilben der Kapazitätswerte unterschiedlich sind. Man muss zuerst alle Werte auf eine gemeinsame Vorsilbe umwandeln. Die Zahlen sollen  nicht zu groß und nicht zu klein werden, deshalb empfiehlt es sich, die Vorsilbe nano ($\unit{\nano}$) zu wählen. 

$\begin{split} \qty{0,1}{\micro\farad} &= \qty{100}{\nano\farad} \\ \qty{50000}{\pico\farad} &= \qty{50}{\nano\farad}\end{split}$

Jetzt muss man nur noch alle Werte in $\unit{\nano\farad}$ addieren.

[question:ED117]

<margin>
[photo:262:a_Netzteil BEKO PA $7 \times \qty{10000}{\micro\farad}$ parallel: Parallelschaltung von $7 \times \qty{10000}{\micro\farad}$ in einem Endstufennetzteil]
</margin>

Als Verständnistest kann die nächste Aufgabe verwendet werden.

[question:ED118]


---

Bei einer Reihenschaltung von Kondensatoren, wie in Abbildung [ref:e_3C-parallel] gezeigt, erhöht sich die Spannungsfestigkeit, allerdings verringert sich die Kapazität. Selbstverständlich kann man wieder die Gesamtkapazität berechnen. Diese ist sehr ähnlich zur Parallelschaltung von Widerstanden:

$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{C_{1}} + \frac{1}{C_{2}} + \frac{1}{C_{3}}$

<margin>
[picture:823:e_3C-parallel:Reihenschaltung von 3 Kondensatoren] 
</margin>

<tip>
Die Gesamtkapazität ist bei der Reihenschaltung immer kleiner als die kleinste Einzelkapazität.
</tip>

<tip>
Bei der Lösung der Aufgaben empfiehlt sich folgende Vorgehensweise:
  
1. Skizziere die Schaltung
2. Schreibe die Kapazitätswerte zu den Bauteilen.
3. Wandle in gleiche Vorsilben um.
4. Vereinfache die Schaltung durch Zusammenführung von gleichartigen Schaltungsgruppen
5. Berechne schrittweise die Gesamtkapazität
</tip>

Wenn alle Kondensatoren gleiche Kapazitätswerte haben, dann kann man die Gesamtkapazität leicht berechnen, indem eine Einzelkapazität durch 3 dividiert wird. In der folgenden Aufgabe rechnet man $\qty{0,33}{\micro\farad} / 3 = \qty{0,11}{\micro\farad}$.

[question:ED119]

Bei der Reihenschaltung von Kondensatoren in der folgenden Aufgabe findet man $\unit{\micro\farad}$ und $\unit{\nano\farad}$ als Vorsilbe. Es ist sehr sinnvoll, $\qty{200000}{\nano\farad}$ zuerst in $\qty{200}{\micro\farad}$ umzuwandeln. Bei einer Reihenschaltung kann man nun die Formel aus der Formelsammlung anwenden.


$C_{\mathrm{ges}} =\frac{1}{\frac{1}{\qty{100}{\micro\farad}} + \frac{1}{\qty{200}{\micro\farad}} + \frac{1}{\qty{200}{\micro\farad}}}$

[question:ED120]

---
  
Bei der nächsten Frage werden 3 Kondensatoren in Reihen- und Parallelschaltung kombiniert. 

[question:ED121]

Welcher Schaltungsteil kann zuerst vereinfacht werden? Richtig: die Reihenschaltung.
Diese Teilgruppe hat als Gesamtkapazität die Hälfte von $\qty{10}{\nano\farad}$, also $\qty{5}{\nano\farad}$. Jetzt ist es einfacher weiterzurechnen, da bei einer Parallelschaltung die Kapazitätswerte addiert werden. Gratulation zum Ergebnis von $\qty{10}{\nano\farad}$.

Die weiteren Aufgaben sind ähnlich und leicht lösbar.

[question:ED122]
[question:ED123]
[question:ED124]

%<margin>
%
%Lösungshilfen:
%
%*ED 118:* Reihenschaltung von $\qty{22}{\nano\farad}$, $\qty{0,033}{\micro\farad} = \qty{33}{\nano\farad}$ und $\qty{15000}{\pico\farad} = \qty{15}{\nano\farad}$.
%$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{\qty{22}{\nano\farad}} + \frac{1}{\qty{33}{\nano\farad}} + \frac{1}{\qty{15}{\nano\farad}}$
%Eigentlich muss man nicht rechnen, denn es gibt nur ein Ergebnis, das kleiner als $\qty{15}{\nano\farard}$ ist.
%*ED 120:* $\qty{50}{\micro\farad}$ 
%*ED 122:* $C_2 = \qty{1}{\micro\farad}$ und $C_3 = \qty{1}{\micro\farad}$ in Parallelschaltung ergibt zusammen $\qty{2}{\micro\farad}$. Dazu $C_1 = \qty{2}{\micro\farad}$ in Reihe %ergibt die Hälfte , also $\qty{1}{\micro\farad}$.
% 
%*ED 123:* $C_2 = \qty{4}{\nano\farad}$ und $C_3 = \qty{4}{\nano\farad}$ in Parallelschaltung ergibt zusammen $\qty{8}{\nano\farad}$. Dazu $C_1 = \qty{8}{\nano\farad}$ in Reihe %ergibt die Hälfte , also $\qty{4}{\nano\farad}$.
%  
%*ED 124:* $C_2 = \qty{100}{\nano\farad}$ und $C_3 = \qty{100000}{\pico\farad} = \qty{100}{\nano\farad}$ in Parallelschaltung ergibt zusammen $\qty{200}{\nano\farad}$. Dazu %$C_1 = \qty{200}{\nano\farad}$ in Reihe ergibt die Hälfte , also $\qty{100}{\nano\farad}$.
%</margin>
