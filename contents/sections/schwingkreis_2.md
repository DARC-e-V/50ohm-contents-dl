In der Formelsammlung finden wir die folgende Formel für die Berechnung der Grenzfrequenz von RC-Gliedern, z.B. von Hoch- oder Tiefpassfiltern:

$f_\text{g} = \frac{1}{2 \pi \cdot R \cdot C}$

Mit dieser Formel können wir eine Reihe von Prüfungsfragen lösen.

<indepth>
Für mathematisch interessierte Leser: Die Formel für die Grenzfrequenz eines RC-Gliedes lässt sich auch durch die Betrachtung der komplexen Impedanzen von Widerstand und Kondensator herleiten. Wir betrachten den RC-Tiefpass als frequenzabhängigen Spannungsteiler.

[picture:175:a_rc_tiepass:RC-Tiefpass als frequenzabhängiger Spannungsteiler]

Für das Verhältnis von Ausgangs- zu Eingangsspannung gilt:

$\frac{|U_\text{A}|}{|U_\text{E}|} = \frac{|X_\text{C}|}{|R + X_\text{C}|}$

Der kapazitive Blindwiderstand des Kondensators lautet:

$X_\text{C} = \frac{1}{j\omega C}$

Damit ergibt sich:

$\frac{|U_\text{A}|}{|U_\text{E}|} = \frac{\left|\frac{1}{j\omega C}\right|}{\left|R + \frac{1}{j\omega C}\right|}$

Für die Beträge erhalten wir:

$\frac{|U_\text{A}|}{|U_\text{E}|} = \frac{\frac{1}{\omega C}}{\sqrt{R^2 + \frac{1}{\omega^2 C^2}}}$

Multipliziert man Zähler und Nenner mit $\omega C$, vereinfacht sich der Ausdruck zu:

$\frac{|U_\text{A}|}{|U_\text{E}|} = \frac{1}{\sqrt{1 + R^2\omega^2 C^2}}$

Die Grenzfrequenz ist so definiert, dass die Ausgangsspannung auf den Faktor $\frac{1}{\sqrt{2}} \approx 0{,}707$ des ursprünglichen Wertes abgefallen ist. Dies entspricht etwa $\qty{70}{\percent}$ der Ausgangsspannung bzw. einem Pegelabfall von $\qty{3}{\dB}$.

$\frac{|U_\text{A}|}{|U_\text{E}|} = \frac{1}{\sqrt{2}}$

Daraus folgt:

$\frac{1}{\sqrt{1 + R^2\omega^2 C^2}} = \frac{1}{\sqrt{2}}$

Damit muss gelten:

$R^2\omega^2 C^2 = 1$

und somit:

$\omega R C = 1$

Mit $\omega = 2\pi f$ ergibt sich:

$2\pi f_\text{g} R C = 1$

Daraus folgt für die Grenzfrequenz:

$f_\text{g} = \frac{1}{2\pi R C}$
</indepth>

[question:AD201] 
[question:AD202] 
[question:AD203] 

**Resonanzfrequenz**
Schaltet man eine Spule und einen Kondensator entweder seriell oder parallel, entsteht ein Schwingkreis. Wir erinnern uns: Bei hohen Frequenzen hat die Spule einen hohen Widerstand. Beim Kondensator verhält es sich genau umgekehrt, so dass eine niedrige Frequenz zu einem hohen Kondensatorwiderstand führt. Bei der Frequenz, bei der Spule und Kondensator den gleichen Widerstand haben, handelt es sich um die Resonanzfrequenz - unabhängig davon, ob es sich um einen Serien- oder Parallelschwingkreis handelt. 
[question:AD206] 
Je nachdem, ob die Schaltung nun als Serien- oder Parallelschwingkreis ausgeführt wird, ändert sich aber nun das Filterverhalten bei der Resonanzfrequenz. 
Bei einem **Parallelschwingkreis** lässt sich durch die Eigenresonanz im Schwingkreis nur wenig Energie zuführen - und zwar nur soweit, wie es im Schwingkreis Verluste gibt (z.B. durch den Drahtwiderstand der Spule). Lässt man die Verluste jedoch außer Acht, findet im Schwingkreis eine kontinuierliche Umladung zwischen größtmöglichem elektrischen Feld im Kondensator und dem größtmöglichen magnetischen Feld in der Spule statt. Theoretisch ist im verlustfreien Schwingkreis im Resonanzfall die Impedanz also unendlich groß. 
Abseits dieser Resonanzfrequenz bestimmt das Bauteil mit dem geringeren Widerstand den gesamten Widerstand (Impedanz) des Schwingkreises, da beide Bauteile parallel liegen. So ist bei hohen Frequenzen der Kondensator niederohmiger als die Spule. Bei niedrigen Frequenzen ist die Spule niederohmiger als der Kondensator. Bei Frequenzen über und unter der Resonanzfrequenz hat ein Parallelschwingkreis also einen geringeren Widerstand (Impedanz). 

Bei einem **Serienschwingkreis** handelt es sich um einen geöffneten Schwingkreis, bei dem die Energie zur Umladung zwischen Kondensator und Spule immer durch Ein- und Ausgang hindurchmuss. Bei der Resonanzfrequenz schwingt der Serienschwingkreis also immer "durch" den Frequenzerzeuger und eine evtl. anhängende Last. Der Widerstand (Impedanz) ist bei der Resonanzfrequenz also sehr gering. Theoretisch und ohne Berücksichtigung von Verlusten z.B. durch den Drahtwiderstand der Spule liegt dieser sogar bei $\qty{0}{\ohm}$. Das liegt unter anderem auch daran, dass sich durch die Phasenlagen zwischen Spule und Kondensator die Spannungen über die einzelnen Komponenten gegenseitig aufheben.
Da Spule und Kondensator in Reihe liegen, bestimmt in diesem Fall das Bauteil mit dem höchsten Widerstand den Gesamtwiderstand der Schaltung. Bei hoher Frequenz hat die Spule einen hohen Widerstand. Bei niedriger Frequenz hat der Kondensator einen hohen Widerstand. Bei Frequenzen über und unter der Resonanzfrequenz haben wir beim Serienschwingkreis daher jeweils einen hohen Gesamtwiderstand (Impedanz). 

[question:AD207] 
[question:AD204] 

Bei Parallel- und Serienschwingkreisen gilt im Resonanzfall folgender Zusammenhang:

$X_\text{C} = X_\text{L}$

Dies bedeutet, dass im Resonanzfall die Widerstände (Impedanzen) beider Bauteile (Spule und Kondensator) genau gleich groß sind. Ohmsche Widerstände und Verluste haben keinen Einfluss auf die Resonanzfrequenz und können daher bei der Berechnung der Resonanzfrequenz von Schwingkreisen vernachlässigt werden.

<tip>
Ohmsche Widerstände in Parallel- und Serienschwingkreisen wirken sich jedoch auf die Güte ($Q$) und damit auf die Bandbreite ($B$) des Schwingkreises aus - hierauf werden wir später noch genauer eingehen.
</tip>

Um die Resonanzfrequenz von Parallel- und Serienschwingkreisen zu berechnen, verwenden wir die sog. Thomsonsche Schwingkreisformel (die jeder Funkamateur auswendig kennen muss):

$f = \frac{1}{2 \pi \cdot \sqrt{L \cdot C}}$

[question:AD208] 
[question:AD209]
[question:AD210] 

---

Die Resonanzfrequenz von Parallelschwingkreisen wird genau wie bei Serienschwingkreisen mit der zuvor genannten Thomsonschen Schwingkreisformel berechnet. Auch hier hat ein parallel geschalteter Widerstand keinen Einfluss auf die Resonanzfrequenz, jedoch auf die Güte (Q) und Bandbreite (B).

[question:AD211] 
[question:AD212] 

---

Um die Resonanzfrequenz von Schwingkreisen zu verändern, kann entweder die Induktivität der Spule oder die Kapazität des Kondensators im Schwingkreis verändert werden.
Wie aus der Thomsonschen Schwingkreisformel ersichtlich befinden sich die Größen $L$ und $C$ jeweils unter dem Bruchstrich. Hierdurch bewirkt eine Vergrößerung von $L$ oder $C$ eine Verringerung der Schwingkreisfrequenz, da der Nenner der Formel größer wird. Die Quadratwurzel hat auf diesen Zusammenhang keinen Einfluss, da die Wurzel aus einer größeren Zahl ebenfalls eine größere Zahl ist. Der Zusammenhang hierbei ist jedoch nicht linear.
Bei einer Verkleinerung von $L$ und $C$ gilt umgekehrt, dass die Resonanzfrequenz des Schwingkreises sich vergrößert.
Die Induktivität einer Spule kann durch Vergrößern der Windungszahl, durch Zusammenschieben oder Einführen eines Ferritkerns vergrößert werden.
Umgekehrt kann die Induktivität einer Spule verringert werden durch Verringerung der Windungszahl, durch Auseinanderziehen oder durch Entfernen eines Ferritkerns oder durch Einführen eines Kupferkerns.
Die Kapazität von Kondensatoren kann durch Austausch oder die Verwendung von Trimm- oder Drehkondensatoren beeinflusst werden.

[question:AD213] 
[question:AD214] 
[question:AD215] 
[question:AD216] 
[question:AD217] 

Oft ist es in Schaltungen erforderlich, die Resonanzfrequenz eines Schwingkreises durch eine Steuerspannung zu beeinflussen (z.B. bei einem VCO - Voltage Controlled Oscillator). Hierfür kann man z.B. eine Kapazitätsdiode verwenden, die in Sperrrichtung betrieben wird. Je höher die Gegenspannung der Diode wird, desto geringer wird deren Kapazität, welche durch die Größe der Grenzschicht (P-N-Übergang) bestimmt wird. Die Grenzschicht vergrößert sich bei Vergrößerung der angelegten Sperrspannung, wodurch sich die Kapazität verringert und damit die Frequenz des Schwingkreises gemäß Thomsonscher Schwingkreisformel steigt.
Umgekehrt verkleinert sich die Grenzschicht der Kapazitätsdiode bei Verringerung der angelegten Sperrspannung, wodurch sich die Kapazität erhöht und damit die Frequenz des Schwingkreises kleiner wird.
Die Sperrspannung kann z.B. durch ein Potentiometer oder einen Steuerkreis erzeugt werden.

%TODO: Evtl. Grafik zu Sperrschicht und Verhalten in Kapazitätsdiode.

[question:AD218] 

Eine Kombination aus Parallel- und Serienschwingkreisen kann bei geeigneter Anordnung als Bandpassfilter verwendet werden. Im Resonanzfall verhalten sich die parallelen Schwingkreise wie hochohmige Widerstände und der Serienschwingkreis wie ein niederohmiger Widerstand.

[question:AD205]

Die Bandbreiten von Filtern und Bandpässen werden in $\unit{\dB}$ bezogen auf einen Referenzwert des Filters angegeben. Hierbei kann die Bandbreite bei einer vorgegebenen Dämpfung oder in Bezug auf die minimale Dämpfung der Durchlasskurve des Filters gemessen werden.
Üblicherweise wird die *Bandbreite* eines Filters als der sog. *$\qty{-3}{\dB}$-Wert* angegeben, bei dem nur noch die halbe Leistung eines Signals das Filter passieren kann; dies entspricht dem *$0,7$-fachen der Signalspannung*.
Die Bandbreite wird als die *Differenz zwischen dem oberen und unteren $\qty{-3}{\dB}$-Wert* gemessen.
So wird z.B. die $\qty{-3}{\dB}$-Dämpfung bezogen auf die minimale Dämpfung der Filterkurve verwendet, um die Eignung eines Filters für bestimmte Betriebsarten (SSB, CW, RTTY) anzugeben.
Ein schmalbandiges Filter (mit einer $\qty{-3}{\dB}$-Bandbreite von $\qty{500}{\hertz}$) wird beispielsweise für Telegrafie (CW) verwendet.
Ein breitbandiges Filter mit (mit einer $\qty{-3}{\dB}$-Bandbreite von $\qty{2,7}{\kilo\hertz}$) wird beispielsweise für Sprachmodulation (SSB) verwendet.
Für Filter mit hoher Güte werden hierfür in der Regel Quarzfilter eingesetzt.

[question:AD219]
[question:AD221] 
[question:AD222]
[question:AD220]

Die Güte eines Schwingkreises (Q-Faktor) wird durch das Verhältnis der Blindwiderstände von Kapazität und Induktivität im Resonanzfall zum ohmschen Verlustwiderstand bestimmt. Wenn ein Schwingkreis keinerlei ohmschen Verlustwiderstände enthalten würde, so wäre dessen Q-Faktor unendlich. Reale Bauteile sind jedoch immer verlustbehaftet. Induktivitäten haben immer einen ohmschen Verlustwiderstand, Kapazitäten haben dielektrische Verluste, die sich ebenfalls als ohmscher Widerstand auswirken.
Je größer die ohmschen Widerstände in einem Schwingkreis sind, desto geringer wird dessen Q-Faktor.

Für die Berechnung des Q-Faktors verwenden wir die entsprechenden Formeln aus der Formelsammlung je nachdem ob es sich um einen Parallel- oder Serienschwingkreis handelt:

Für den Serienschwingkreis gilt im Resonanzfall ($X_\text{L} = X_\text{C}$):
$Q = \frac{f_0}{B} = \frac{X_\text{L}}{R_\text{S}}$

Für den Parallelschwingkreis gilt im Resonanzfall ($X_\text{L} = X_\text{C}$):
$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$

[question:AD225]

---

Entsprechend dem obigen Rechenbeispiel können wir jetzt auch den Gütefaktor des Parallelschwingkreises errechnen. Die Resonanzfrequenz wird wie im vorigen Beispiel berechnet. Es ist jedoch zu beachten, dass für die Berechnung von $Q$ die Formel für den Parallelschwingkreis zu verwenden ist:

$Q = \frac{f_0}{B} = \frac{R_\text{P}}{X_\text{L}}$

[question:AD226]

Die Bandbreite von Parallel- und Serienschwingkreisen lässt sich nun ebenfalls einfach aus der Resonanzfrequenz des Schwingkreises und dessen Gütefaktor wie folgt berechnen (Formel hierzu in der Formelsammlung):

$Q = \frac{f_0}{B}$

Durch Umstellen der Formel ergibt sich die Bandbreite $B$:

$B = \frac{f_0}{Q}$

Die vorgenannte Formel gilt sowohl für den Serien- als auch den Parallelschwingkreis!

[question:AD224]

---

Entsprechend kann nun auch mit dem zuvor beschriebenen Wissen die folgende Frage schrittweise berechnet werden.
[question:AD223]

Zur Übertragung von Signalen zwischen Schaltungsstufen sowie in Filtern in Sendern und Empfängern werden häufig gekoppelte Schwingkreise verwendet. Hierbei werden zwei Schwingkreise induktiv oder kapazitiv aneinander gekoppelt. Diese Kopplung kann je nach Anwendung *lose*, *unterkritisch*, *kritisch* oder *überkritisch* erfolgen. Der Grad der Kopplung bestimmt die gegenseitige Beeinflussung und damit die Bandbreite und Durchlasskurve der gesamten Anordnung.
Bei loser und unterkritischer Kopplung gibt es kaum eine gegenseitige Beeinflussung; Dafür ist die Durchlassdämpfung der Anordnung relativ hoch und die Bandbreite relativ gering.
Bei kritischer Kopplung beeinflussen sich beide Schwingkreise gerade so, dass eine im Durchlassbereich flache Durchlasskurve mit geringer Dämpfung entsteht und diese im gewünschten Durchlassbereich völlig eben ist (Plateau). Die Bandbreite der Anordnung ist hierbei größer als bei loser und unterkritischer Kopplung. Hieran ist eine kritische Kopplung auch gut zu erkennen.
Bei überkritischer Kopplung ist die gegenseitige Beeinflussung der beiden Schwingkreise sehr stark, was zu einer starken Änderung beider Resonanzfrequenzen und damit zu einer großen Bandbreite führt. Hierdurch wird die Durchlasskurve im Durchlassbereich stark verzerrt und es bilden sich links und rechts der Mittenfrequenz zwei Resonanzpunkte. Die Durchlasskurve bekommt eine "Delle". Hieran ist die überkritische Kopplung gut zu erkennen.

[question:AD227] 
[question:AD228] 
[question:AD229] 