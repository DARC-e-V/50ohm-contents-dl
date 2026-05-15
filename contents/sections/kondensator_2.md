In der Klasse E haben wir bereits die Kapazität eines Kondensators sowie sein qualitatives Verhalten bei Wechselspannung kennengelernt: Ein Kondensator verhält sich wie ein frequenzabhängiger Widerstand. Dabei haben wir zunächst festgehalten, dass der kapazitive Blindwiderstand umgekehrt proportional zur Frequenz ist. Verringert man die Frequenz, so wird der Blindwiderstand $X_\text{C}$ größer. Erhöht man hingegen die Frequenz, nimmt der Widerstand entsprechend ab. Der Sachverhalt eines Kondensators bei Wechselspannung lässt sich durch die Formel für den kapazitiven Blindwiderstand $X_\text{C}$ beschreiben:

$|X_\text{C}| = \frac{1}{\omega\cdot C} = \frac{1}{2\pi\cdot f \cdot C}$

In der Klasse A wollen wir dieses Verhalten nun genauer betrachten und auch erfahren, warum dieser Widerstand als "Blindwiderstand" bezeichnet wird. Zunächst müssen wir uns allerdings noch merken, dass der Blindwiderstand eines Kondensators auch negativ ist, um die folgende Frage lösen zu können: 

[question:AC102]

<indepth>
Warum ist der kapazitive Blindwiderstand negativ? Der Hintergrund liegt in der komplexen Wechselstromrechnung, die für die Amateurfunkprüfung nicht zwingend erforderlich ist.

Für Leserinnen und Leser mit Kenntnissen in komplexen Zahlen sei jedoch angemerkt, dass die korrekte Darstellung des kapazitiven Blindwiderstands eigentlich

$X_\text{C} = \frac{1}{j\omega C}$

lautet. Dabei steht $j$ für die imaginäre Einheit $\sqrt{-1}$.

Erweitert man diesen Ausdruck mit $j$, ergibt sich:

$X_\text{C} = \frac{1}{j\omega C} = \frac{1 \cdot j}{j\omega C \cdot j} =\frac{-j}{\omega C}$

Daraus wird ersichtlich, dass der kapazitive Blindwiderstand nicht nur negativ, sondern auch komplex ist. Das negative Vorzeichen beschreibt dabei die Phasenlage zwischen Strom und Spannung am Kondensator welche wir in diesem Kapitel noch genauer betrachten.
</indepth>

---

Moderne, kostengünstige Messgeräte, die Funkamateure heutzutage gerne einsetzen, sind Antennenanalyzer oder vektorielle Network Analyzer (VNA). Sie messen die Veränderung des Blindwiderstandes $X_\text{C}$ in Abhängigkeit der Frequenz und können das Messergebnis auch grafisch darstellen.
Abbildung [ref:a_kapazitiver_Blindwiderstand] zeigt die Veränderung des kapazitiven Blindwiderstandes (blaue Linie) eines $\qty{1500}{\pico\farad}$ Styroflexkondensators im Frequenzbereich von $\qtyrange{1}{4,5}{\mega\hertz}$. 

<margin>
[photo:248:a_kapazitiver_Blindwiderstand:Kapazitiver Blindwiderstand $X_\text{C}$ (Blaue Kurve) und Phasenlage (Rote Kurve) eines $\qty{1500}{\pico\farad}$ Styroflexkondensators im Frequenzbereich von $\qtyrange{1}{4,5}{\mega\hertz}$.]
</margin>


Versuche nun die folgenden Fragen durch die obige Formel zu beantworten. Achte dabei besonders auf die Einheiten bzw. die Zehnerpotenzen, damit du die richtigen Ergebnisse erhältst.

[question:AC104]
[question:AC105]
[question:AC106]
[question:AC107]

Bei der folgenden Frage ist die Kapazität gesucht. Versuche hierfür die Formel umzustellen, damit du die Kapazität $C$ berechnen kannst:

[question:AC108]

---

Führt man eine gleichzeitige Strom- und Spannungsmessung an einem Kondensator mit einem Zweikanal-Oszilloskop durch (vgl. [ref:a_strom_eilt_vor]), zeigt sich ein zunächst überraschendes Ergebnis: Zwischen Strom und Spannung besteht eine Phasenverschiebung von $\qty{90}{\degree}$, wobei der Strom der Spannung vorausläuft.

Das bedeutet, dass der Strom bereits seinen Maximalwert erreicht, während die Spannung noch ansteigt. Dieses charakteristische Verhalten ist eine grundlegende Eigenschaft von Kondensatoren und spielt eine wichtige Rolle in der Wechselstromtechnik, insbesondere bei Filtern und Schwingkreisen.
Die rote Linie in Abbildung [ref:a_kapazitiver_Blindwiderstand] stellt die Phasenlage des kapazitiven Blindwiderstandes bei nahezu konstanten $\qty{-90}{\degree}$ dar.

[question:AC101]

<margin>
[photo:268:a_strom_eilt_vor:Phasenverschiebung am Kondensator zwischen Spannung und Strom]
</margin>

<tip>
Merkhilfe: Beim Kondensat*ooo*r eilt der Strom v*ooo*r!
</tip>

---

Die Phasenverschiebung zwischen Spannung und Strom beträgt also $\qty{90}{\degree}$, wobei der Strom (rot) der Spannung (blau) voreilt, wie in Abbildung [ref:a_blindleistung_kondensator] gezeigt. Betrachtet man die momentane Leistung mit $P = U \cdot I$, so ergibt sich eine Leistungskurve (grün), die symmetrisch um die Nulllinie schwankt, ebenfalls dargestellt in Abbildung [ref:a_blindleistung_kondensator].

<margin>
[picture:943:a_blindleistung_kondensator:Das Produkt von $U \cdot I$ ergibt die grüne Leistungskurve]
</margin>

Der Mittelwert dieser Leistung ist Null, das heißt, es wird keine Wirkleistung umgesetzt. Stattdessen wird Energie periodisch im elektrischen Feld des Kondensators gespeichert und wieder an die Quelle zurückgegeben. Man spricht daher bei einem ideal verlustfreien Kondensator von Blindleistung und einem Blindwiderstand.

Nur ein ohmscher Widerstand nimmt Wirkleistung auf, da bei ihm Spannung und Strom in Phase sind, also keine Phasenverschiebung vorliegt. Das bedeutet, dass Spannung und Strom gleichzeitig positiv oder negativ sind, sodass die momentane Leistung $P = U \cdot I$ stets positiv ist.

Ein idealer Blindwiderstand hingegen nimmt keine Wirkleistung auf und wird daher im Idealfall auch nicht warm. Stattdessen wird Energie periodisch gespeichert und wieder an die Quelle zurückgegeben.

[question:AC111]

[question:AC103]

---

Erwärmt sich ein Kondensator in Hochfrequenzanwendungen dennoch, so ist dies ein Hinweis auf Verluste im Bauteil. Ein idealer Kondensator würde keine Energie in Wärme umsetzen, reale Kondensatoren besitzen jedoch parasitäre Eigenschaften, die zu Verlusten führen.

Diese Verluste lassen sich im Ersatzschaltbild erkennen: Der Widerstand $R_\text{ESR}$ (Equivalent Series Resistance) beschreibt die ohmschen Verluste im Kondensator, während $R_\text{Isolator}$ die Verluste im Dielektrikum modelliert. Zusätzlich beeinflusst die parasitäre Induktivität $L_\text{ESL}$ das Verhalten bei hohen Frequenzen.

Zur technischen Bewertung dieser Verluste verwendet man die Güte $Q$ (Quality Factor) sowie den Verlustfaktor $\tan\delta$. Beide Größen beschreiben, wie stark ein realer Kondensator vom idealen Verhalten abweicht.

Zwischen beiden Größen besteht ein direkter Zusammenhang:

$Q = \frac{1}{\tan\delta}$

Merke: Hohe Verluste führen zu einer niedrigen Güte $Q$ und damit zu einem großen Verlustfaktor $\tan\delta$. Je höher die Frequenz, desto stärker wirken sich diese Verluste aus, da der Blindwiderstand $X_\text{C}$ mit steigender Frequenz abnimmt, während die parasitären Widerstände konstant bleiben.

<margin>
[picture:1065:a_ersatzschaltbild_kondensator:Ersatzschaltbild eines realen Kondensators mit parasitären Verlusten.]
</margin>

---

[question:AC109]

[question:AC110]

<indepth>
Durch die komplexe Wechselstromrechnung kann man den Blindwiderstand $X_\text{C}$ mit den parasitären Verlusten $R$ in Form eines Zeigerdiagramms darstellen: 
[picture:1066:a_tan_delta:$\tan\delta$ im komplexen Zeigerdiagramm]

Der Tangens beschreibt ja das Verhältnis von Gegenkathete zu Ankathete, also in diesem Fall die Verluste $R$ im Verhältnis zum verlustfreien kapazitiven Blindwiderstand $X_\text{C}$. 

$\tan\delta = \frac{R}{|X_\text{C}|}$

Je größer die Verluste, desto größer ist der Winkel $\delta$ und damit auch der Verlustfaktor $\tan\delta$. Ein idealer Kondensator würde einen Winkel von $\delta = 0$ Grad aufweisen, da er keine Verluste hat.

Durch diese komplexe bzw. geometrische Addition ergibt sich die Größe $Z$. Sie wird als *Impedanz* bezeichnet und beschreibt den komplexen Gesamtwiderstand eines Bauteils. Der Betrag der Impedanz $|Z|$ entspricht dem sogenannten *Scheinwiderstand*.
</indepth>
