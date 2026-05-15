In Parallelschwingkreisen werden Spulen und Kondensatoren kombiniert. Zur genauen Berechnung der Resonanzfrequenz, müssen "unsichtbare" Kapazitäten, wie Wicklungskapazität und Schaltungskapazität,  berücksichtigt werden. Die folgende Aufgabe beschreibt die wirksamen Kapazitäten sehr praxisnah.

[question:AD103]
Das Hauptproblem bei der Lösung der Aufgaben ist die Beachtung und Umwandlung der unterschiedlichen Vorsilben auf eine einheitliche, sinnvolle Vorsilbe, um nicht zu große oder zu kleine Zahlenwerte zu bekommen. Im Abschnitt "Kondensatoren  in Reihen- und Parallelschaltung "   der Klasse E wurde dies schon ausführlich erklärt. 
Als gemeinsame Vorsilbe sollten bei der folgenden Frage alle Kapazitätswerte in Picofarad (pF) umgewandelt werden, da auch das Ergebnis in Picofarad angegeben ist. Die Eigenkapazität der Spule (Kapazität der Windungen gegeneinander) muss zusätzlich addiert werden.

Schwieriger ist die Berechnung einer Reihenschaltung von 3 Kondensatoren.

Bei der folgenden Aufgabe hat die kleinste Kapazität den Wert $\qty{22}{\pico\farad}$.
Die Gesamtkapazität muss deshalb kleiner als $\qty{22}{\pico\farad}$ sein. Da in der Lösung zwei Ergebnisse unter $\qty{22}{\pico\farad}$ zu finden sind, ist keine Abschätzung möglich, sondern es ist eine Rechnung notwendig.
$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{C_{1}} + \frac{1}{C_{2}} + \frac{1}{C_{3}}$
(siehe Formelsammlung Seite 236 unten -  Stichwort: Kondensatoren in Reihenschaltung )


---
[question:AD101]

<tip>
 Man gibt die Kapazitätswerte immer mit der 1/x - Taste in den Taschenrechner ein und muss am Schluss nochmals 1/x drücken.
</tip>
$C_1$ mit $\qty{0,1}{\nano\farad}$ muss in Picofarad umgewandelt werden. Dies ergibt $\qty{100}{\pico\farad}$.
$\frac{1}{C_{\mathrm{ges}}} = \frac{1}{\qty{100}{\pico\farad}} + \frac{1}{\qty{47}{\pico\farad}} + \frac{1}{\qty{22}{\pico\farad}}$

---
[question:AD104]
<indepth>
% Widerstandsdreieck R - XC in Latex erstellen
[photo:301:a_R-C Widerstandsdreieck:Widerstandsdreieck für die Reihenschaltung von $R$ und $X_\text{C}$]
Das Widerstandsdreieck für die Reihenschaltung von $R$ und $X_\text{C}$ veranschaulicht grafisch die Berechnung mit der Formel $|Z| = \sqrt{R^2 + {X_\text{C}}^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{159}{\ohm})^2}$
  Zusätzlich sieht man auch den Phasenverschiebungswinkel $\varphi$ zwischen $U$ und $I$ und das $I$ voreilend ist.
</indepth>


Zur Berechnung eines Scheinwiderstandes benutzen wir die Formel
$|Z| = \sqrt{R^2 + X^2}$
(siehe Formelsammlung Seite 235 unten rechts - Stichwort: Wechselspannung -> Scheinwiderstand)
Zur Anwendung dieser Formel muss der Blindwiderstand $X_\text{C}$ des Kondensators bei $\qty{1}{\mega\hertz}$ zuerst berechnet werden.
Die Formel für $X_\text{C}$ lautet:
$X_\text{C} = \frac{1}{\omega \cdot C}$
(siehe Formelsammlung Seite 236 unten links - Stichwort: Kapazität -> kapazitiver Blindwiderstand )

Bei der Eingabe der Bauteilwerte in den Taschenrechner müssen die Zehnerpotenzen sorgfältig hinzugefügt werden.
$\qty{1}{\mega\hertz} = \qty{1e6}{\hertz}$; $\qty{1}{\nano\farad} = \qty{1e-9}{\farad}$
$X_\text{C}$ ergibt sich dann für den $\qty{1}{\nano\farad}$ Kondensator bei $\qty{1}{\mega\hertz}$ zu $\qty{159}{\ohm}$.
Nun kann der Scheinwiderstand $|Z|$ berechnet werden.
$|Z| = \sqrt{R^2 + {X_\text{C}}^2}$

---
[question:AD105]
Der Rechenweg ist der Gleiche wie vorher beschrieben und die Zehnerpotenzen sind wieder zu beachten:
$\begin{split} \qty{100}{\micro\henry} &= \qty{100e-6}{\henry} \\ \qty{1}{\mega\hertz} &= \qty{1e6}{\hertz} \end{split}$
$X_\text{L}$ muss mit der Formel  $X_\text{L} = \omega \cdot L$ zuerst  berechnet werden, danach kann die Berechnung des Scheinwiderstandes $|Z|$  mit der Formel $|Z| = \sqrt{R^2 + {X_\text{L}}^2}$ erfolgen.

<indepth>
% Widerstandsdreieck R - XL in Latex erstellen

[photo:302:a_R-L Widerstandsdreieck:Widerstandsdreieck für die Reihenschaltung von $R$ und $X_\text{L}$]
Das Widerstandsdreieck für die Reihenschaltung von $R$ und $X_\text{L}$ veranschaulicht grafisch die Berechnung mit der Formel $|Z| = \sqrt{R^2 + {X_\text{L}}^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{628}{\ohm})^2}$
Zusätzlich sieht man auch den Phasenverschiebungswinkel $\varphi$ zwischen $U$ und $I$ und das $I$ nacheilend ist.
</indepth>


<margin>
Lösungshilfe
AD 103: $\qty{100}{\pico\farad} + \qty{1500}{\pico\farad} + \qty{220}{\pico\farad} + \qty{1}{\pico\farad} = \qty{1821}{\pico\farad}$
AD 101: $\qty{13}{\pico\farad}$
AD 104: $X_\text{C} = \frac{1}{6,28 \cdot \qty{1e6}{\hertz} \cdot \qty{1e-9}{\farad}} = \qty{159}{\ohm}$
$|Z| = \sqrt{R^2 + {X_\text{C}}^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{159}{\ohm})^2} \approx \qty{188}{\ohm}$
AD 105: $\qty{636}{\ohm}$
$X_\text{L} = \omega \cdot L = 2\pi \cdot f \cdot L = 2\pi \cdot \qty{1}{\mega\hertz} \cdot \qty{100}{\micro\henry} = \qty{628}{\ohm}$
$|Z| = \sqrt{R^2 + {X_\text{L}}^2} = \sqrt{(\qty{100}{\ohm})^2 + (\qty{628}{\ohm})^2} \approx \qty{636}{\ohm}$
</margin>
