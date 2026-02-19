Das dritte passive Bauelement in der Funktechnik – nach Widerstand und Kondensator – ist die *Spule*. Verschiedene Spulenarten und Ihre Schaltsymbole sind in den Abbildungen [ref:e_spulen] und [ref:e_schaltsymbole_spulen] dargestellt. Wie wir bereits im Kapitel zum magnetischen Feld gelernt haben, wird in einer Spule ein Magnetfeld erzeugt, sobald ein elektrischer Strom durch die Spule fließt. Die einfachste Bauform einer Spule ist die sogenannte gerade *Zylinderspule*, wie sie in Abbildung [ref:e_spule_Aufbau] gezeigt wird.

<margin>
[photo:207:e_spulen:Verschiedene Bauformen von Spulen]
[picture:942:e_schaltsymbole_spulen:Schaltsymbole für unterschiedliche Spulenarten]
[picture:948:e_spule_Aufbau:Aufbau einer Spule]
</margin>

---

Eine Zylinderspule hat eine sogenannte Induktivität $L$, welche sich nach folgender Formel berechnet:

$L = \frac{\mu_0 \cdot \mu_r \cdot N^2 \cdot A_S}{l}$

Betrachtet man den Aufbau einer Spule, dann findet man also folgende Größen:
1. $\mu_0$ ist die magnetische Feldkonstante, eine Naturkonstante mit dem Wert $\qty{1,2566e-6}{\henry\per\meter}$. Den Wert kann man immer in der Formelsammlung nachschlagen.
2. $\mu_r$ ist eine Materialkonstante, denn der Spulenkern kann aus einem speziellen Material bestehen, das magnetische Felder verstärken kann.
3. Anzahl $N$ der Spulenwindungen aus Kupferlackdraht oder versilbertem Kupferdraht 
4. $A_S$ gibt die Querschnittsfläche des Spulenkerns an $A$
5. Spulenlänge $l$

[question:EA102]

<indepth>
Der Formelbuchstabe $L$ wurde zu Ehren des Professors Emil Lenz (1804–1864) aus St. Petersburg gewählt, der die nach ihm benannte Lenzsche Regel formulierte.
</indepth>

<unit>
Eine Spule besitzt die Induktivität $L$ mit der Einheit $\qty{1}{\volt\second\per\ampere}$, die üblicherweise in *Henry* ($\unit{\henry}$) angegeben wird. Die Einheit ist nach dem amerikanischen Physiker *Joseph Henry* (1797–1878) benannt. Eine Induktivität von $\qty{1}{\henry}$ liegt vor, wenn eine Stromänderung von $\qty{1}{\ampere}$ innerhalb einer Sekunde eine Selbstinduktionsspannung von $\qty{1}{\volt}$ hervorruft. In der Praxis liegen die Werte von Induktivitäten meist deutlich darunter und werden typischerweise in $\unit{\milli\henry}$, $\unit{\micro\henry}$ oder $\unit{\nano\henry}$ angegeben.
</unit>

---

Mithilfe der Formel und den folgenden qualitativen Zusammenhängen kann man bereits eine Reihe von Prüfungsfragen lösen:

1. Die Induktivität steigt quadratisch mit der Windungszahl. Wenn die Windungszahl verdoppelt wird, dann steigt die Induktivität auf das Vierfache
2. Wenn die Spule zusammengedrückt wird, dann steigt die Induktivität L
3. Wenn die Querschnittsfläche vergrößert wird, dann steigt die Induktivität L
4. Wenn das Magnetfeld in der Spule durch ein geeignetes, magnetisch leitfähiges Material (z.B. Eisen) verstärkt wird, dann steigt die Induktivität L

[question:EC305]

Wenn man die Spule staucht, dann wird $l$ verkleinert. Dadurch steigt die Induktivität $L$.

[question:EC306]

Wenn man die Spulenlänge $l$ verdoppelt, dann muss sich die Induktivität $L$ halbieren.

[question:EC307]

Wenn die Anzahl der Windungen $N$ verdoppelt wird, dann vervierfacht sich die Induktivität $L$.

Wenn die Windungszahl verringert wird, dann sinkt die Induktivität, aber selbst bei einer halben oder Viertelwindung  und sogar bei einem geraden Stück Draht ist noch eine geringe parasitäre Induktivität vorhanden.

[question:EC304]

Als *ferromagnetisch* bezeichnen wir eine bestimmte Klasse an Materialien, die auf atomarer Ebene kleine Elementarmagnete enthalten, die sich unter dem Einfluss eines äußeren magnetischen Felds ausrichten und so die *magnetische Flussdichte* sehr erhöhen (mit der wir uns an dieser Stelle aber noch nicht beschäftigen). Unter den reinen chemischen Elementen sind nur Eisen, Kobalt und Nickel ferromagnetisch.

[question:EB204]

Wenn man ein ferromagnetisches Material wie Eisen in die Spule einführt, dann wird das Magnetfeld verstärkt und die Induktivität steigt. 

Wenn wir in eine Zylinderspule einen Kern aus einem gut leitenden (nicht-ferromagnetischen) Metall wie Aluminium oder Kupfer einführen, dann sinkt die Induktivität der Spule hingegen. Das liegt daran, dass das hochfrequente Magnetfeld der Spule in den Kernen Ströme, sogenannte Wirbelströme, erzeugt ("induziert"). Diese sekundären Ströme erzeugen wiederum Magnetfelder, die dem Magnetfeld der Spule entgegenwirken. Deshalb sinkt die Induktivität. Das magnetische Feld im Inneren des Kerns wird dabei reduziert. 

Die in der folgenden Frage als richtig betrachtete Antwort ist die, dass das Magnetfeld nicht in den Kern eindringen kann und deshalb der Querschnitt des Feldes verringert. Das ist aber nicht ganz das, was physikalisch passiert. Einfach die "richtige" Antwort merken. 

[question:EB205]

---

Schauen wir uns, wie beim Kondensator auch, zuerst das Gleichstromverhalten der Spule an: Die Spule wird über einen Vorwiderstand an eine Gleichspannungsquelle angeschlossen, wie in Abbildung [ref:e_spule_einschalten] dargestellt. Im Moment des Einschaltens wird der Stromanstieg zunächst verzögert, sodass der Strom nicht sprunghaft, sondern nur allmählich bis zu seinem Maximalwert ansteigt.

Ursache hierfür ist die Lenzsche Regel: Beim Anstieg des Stroms erzeugt die Spule eine Selbstinduktionsspannung, die der Stromänderung – und damit der Ursache – entgegenwirkt. Dadurch wird der Stromanstieg begrenzt. Da zu Beginn noch kein Strom fließt, fällt zunächst nahezu die gesamte angelegte Spannung an der Spule ab. Mit zunehmendem Strom nimmt diese Induktionsspannung ab, während der Strom weiter ansteigt.

Ist der stationäre Zustand erreicht, verhält sich die Spule bei Gleichstrom näherungsweise wie ein Stück Draht. Die an ihr abfallende Spannung ist dann praktisch null. Der zeitliche Verlauf der Spannung an der Spule ist in Abbildung [ref:e_spule_einschalten_spannung] dargestellt.

<margin>
[picture:1016:e_spule_einschalten:Stromkreis zur Untersuchung einer Spule]
</margin>
<margin>
[picture:186:e_spule_einschalten_spannung:Spannungsverlauf beim Einschalten]
</margin>

[question:EC301]

---

Im Ausschaltmoment will die Selbstinduktionsspannung den Stromfluss aufrechterhalten. Die Spule wirkt dann als Generator, dessen Induktionsspannung entgegengesetzt zur vorherigen Polarität entsteht. Damit verhält sich die Spule exat gegenteilig zum Kondensator. Diese Vorgänge kann man gut mithilfe eines Oszilloskops wie in Abbildung [ref:e_Spulenstrom] beobachten.

<margin>
[photo:257:e_Spulenstrom:Ein-und Ausschaltverhalten der Spulenspannung und des Spulenstroms]
</margin>

Man kann deshalb Spulen auch zur Verzögerung benutzen. In der folgenden Frage,  steigt der Stromfluss durch Lampe 2 langsamer an, als durch Lampe 1, da eine Spule vorgeschaltet ist, deren Selbstinduktionsspannung den Einschaltstrom nur langsam ansteigen lässt.

[question:EC302]

Ähnlich wie beim Kondensator verhält sich eine Spule unterschiedlich, wenn sie an Gleichspannung oder an Wechselspannung angeschlossen wird. In der Funktechnik ist vor allem das Verhalten an Wechselspannung wichtig. Deshalb schauen wir uns nun das Wechselstromverhalten an. 

Die Spule zeigt, ähnlich wie ein Kondensator, einen Wechselstromwiderstand $X_{\textrm{L}}$, das heißt, obwohl der Spulendraht nur einen sehr kleinen ohmschen Widerstand (Leiterwiderstand) besitzt, fließt ein Strom, der aber mit steigender Frequenz der Wechselspannung kleiner wird:

$X_{L} = \omega \cdot L = 2\cdot\pi\cdot f \cdot L$

Aus der Formel lässt sich erkennen, dass der Wechselstromwiderstand mit zunehmender Frequenz ansteigt und mit abnehmender Frequenz sinkt.

[question:EC303]