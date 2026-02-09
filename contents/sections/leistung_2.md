In der Klasse N haben wir den Leistungsbegriff bereits als Produkt aus Strom und Spannung ($P = U \cdot I$) kennengelernt. In der Klasse E vertiefen wir dieses Thema weiter, indem wir uns unter anderem mit dem Umstellen von Formeln befassen.

---

Dazu betrachten wir die Schaltung in Abbildung [ref:e_leistung_r]. Sie zeigt, wie an einem Widerstand elektrische Leistung in Wärme umgesetzt wird. Angenommen, die Größen $P$ und $R$ sind bekannt, so lässt sich mithilfe der Leistungsformel ($P = U \cdot I$) und des ohmschen Gesetzes ($U = R \cdot I$) die Spannung $U$ bestimmen.

<margin>
[picture:1013:e_leistung_r:Leistung wird am Wiederstand $R$ in Wärme umgesetzt]
</margin>
  
---

<tip>
Die hergeleiteten Formeln sind auch übersichtlich in der [Formelsammlung](https://50ohm.de/hm) zu finden. 
</tip>
  
Zunächst stellen wir dazu die Gleichung des ohmschen Gesetzes nach dem Strom um:

$ U = R \cdot I \quad\quad\quad |~: R $

$ I = \frac{U}{R}$.

Setzen wir diesen Ausdruck für $I$ in unsere Leistungsformel ein, so ergibt sich:

$P=U \cdot \frac{U}{R}$

$P=\frac{U^2}{R}$. 

Diese Gleichung lösen wir nach $U^2$ auf, indem wir beide Seiten mit R multiplizieren:

$P=\frac{U^2}{R} \quad\quad\quad |~\cdot R$

$U^2 = P \cdot R$.

Nun möchten wir die Spannung $U$ bestimmen. Dazu wenden wir die Umkehroperation des Quadrierens an, nämlich das Ziehen der Quadratwurzel. Dadurch erhalten wir:

$ U^2 = P \cdot R \quad\quad\quad |~\sqrt{~~}$

$U = \sqrt{P \cdot R}$.

In einigen Prüfungsfragen ist es wichtig, die richtigen Zusammenhänge zu erkennen. Mithilfe der Formelsammlung lässt sich die korrekte Lösung jederzeit herleiten.

[question:EB504]
  
Auch für den Strom $I$ lässt sich durch Einsetzen des ohmschen Gesetzes in die Leistungsformel der Zusammenhang zwischen Strom $I$, Widerstand $R$ und Leistung $P$ herleiten.

Wir starten mit den beiden Gleichungen $P = U \cdot I$ und $U = R \cdot I$. Setzt man die zweite Gleichung in die erste für $U$ ein, ergibt sich:

$P = R \cdot I \cdot I$

$P = I^2 \cdot R$.

Wir lösen nach $I^2$ auf, indem wir beide Seiten durch R teilen: 

$P = I^2 \cdot R \quad\quad\quad |~:~R$

$I^2 = \frac{P}{R} $.

Im letzen Schritt ziehen wir dann die Wurzel:

$I^2 = \frac{P}{R}  \quad\quad\quad |~\sqrt{~~}$

$I = \sqrt{\frac{P}{R}}$


[question:EB505]

Kennt man die Leistung $P$ und den Strom $I$ oder die Spannung $U$, kann man daraus stets auch den Widerstand $R$ berechnen.

Wir kennen bereits:

$P=\frac{U^2}{R}$

Wir lösen nach R auf, indem wir beide Seiten der Gleichung mit R multiplizieren und dann durch P teilen:

$R = \frac{U^2}{P}$

Andererseits ist $P = I^2 \cdot R$. Wir teilen beide Seiten durch $I^2$ und erhalten den gesuchten Ausdruck:

$R = \frac{P}{I^2}$

[question:EB506]

Alle zuvor vorgestellten Zusammenhänge der Gleichspannungstechnik zwischen Leistung, Strom und Spannung gelten auch für Wechselstrom. Allerdings müssen dabei die Effektivwerte von Strom und Spannung verwendet werden. In einem vorherigen Kapitel haben wir bereits kennen gelernt wie man aus dem Spitzenwert den Effektivwert berechnet: 

$U_{eff} = \frac{\hat{U}}{\sqrt{2}}$ bzw. $\hat{U} = U_{eff} \cdot \sqrt{2}$

[question:EB503]

Das bedeutet, dass wir mit allen zuvor hergeleiteten Formeln nun auch die folgenden Aufgaben aus der Welt der Hochfrequenz – also der Wechselspannung – berechnen können.

%%%%%

[question:EB507]

Der Effektivwert beträgt hier $U_\text{eff} = \qty{100}{\volt}$. Der Abschlusswiderstand beträgt $\qty{50}{\ohm}$ (reiner Wirkwiderstand). Gesucht ist die Leistung an der Last.

$P = \frac{U^2}{R} =\frac{(\qty{100}{\volt})^2}{\qty{50}{\ohm}} = \qty{200}{\watt}$

%%%%%

[question:EB508]

Auch wenn der Strom bekannt ist, kann man mit der bekannten Formel $P = I^2 \cdot R$ berechnen. Wir setzen ein:
  
$P = (\qty{2}{\ampere})^2 \cdot \qty{50}{\ohm} = \qty{200}{\watt}$

%%%%%

[question:EB509]

Zur Berechnung der Leistung, die in einem $\qty{100}{\ohm}$-Widerstand umgesetzt wird, an dem eine Spannung von $\qty{10}{\volt}$ abfällt, benutzen wir wieder:

$P = \frac{U^2}{R} = \frac{(\qty{10}{\volt})^2}{\qty{100}{\ohm}} = \qty{1}{\watt} $

%%%%%

[question:EB510]

Die Beantwortung dieser Frage bedarf eines gewissen Nachdenkens. Es ist sowohl eine maximale Spannungsfestigkeit ($\qty{700}{\volt}$) als auch eine Maximalleistung ($\qty{1}{\watt}$) angegeben. Es fragt sich nur, welche Grenze zuerst erreicht wird, wenn wir die Spannung erhöhen.

Berechnen wir zunächst die Spannung, die am Widerstand (\qty{10}{\kilo\ohm}$) anliegen muss, damit gerade die zulässige Leistung erreicht wird. Dazu rechnen wir (Herleitung weiter oben):

$U = \sqrt{P \cdot R} = \sqrt{\qty{1}{\watt} \cdot \qty{10000}{\ohm}} = \qty{100}{\volt}$

Das ist dann auch schon die gesuchte maximale Gleichspannung!

%%%%%

[question:EB511]

Hier ist der Rechenweg derselbe wie in der Aufgabe davor, nur die Zahlenwerte sind anders:

$U = \sqrt{P \cdot R} = \sqrt{\qty{6}{\watt} \cdot \qty{10^5}{\ohm}} \approx \qty{774,6}{\volt} \approx \qty{775}{\volt}$

%%%%%

[question:EB512]

Wenn der Widerstandswert und die maximale Belastbarkeit gegeben sind und nach dem Maximalstrom gefragt wird, verwenden wir die Beziehung:

$I = \sqrt{\frac{P}{R}} =  \sqrt{\frac{\qty{23}{\watt}}{\qty{120}{\ohm}}} \approx \qty{0,4378}{\ampere} \approx \qty{438}{\milli\ampere}$

[question:EB513]

In dieser Frage wird ein Oszilloskop verwendet, um die Spitzen-Spitzen Spannung an der Last zu messen. Diese Spannung beträgt $U_{SS} = \qty{25}{\volt}$. Das bedeutet die Spitzenspannung beträgt $\hat{U} = \qty{12,5}{\volt}$ Wir berechnen zunächst den Effektivwert der Spannung:

$U_{eff} = \frac{\hat{U}}{\sqrt{2}} = \frac{\qty{12,5}{\volt}}{\sqrt{2}} \approx \qty{8,84}{\volt}$

Dann ist der Effektivstrom (Ohmsches Gesetz):

$I_{eff} = \frac{U_{eff}}{R} = \frac{\qty{8,84}{\volt}}{\qty{1000}{\ohm}} = \qty{8,8}{\milli\ampere}$

Damit ließe sich auch die effektive Leistung berechnen, doch so weit geht die Frage hier nicht.

---

[question:EB514]

Die Antwort zu dieser Frage schließlich lässt sich sehr gut im Kopf rechnen. Hier werden 11 gleiche Widerstände, wie in Abbildung [ref:e_dummyload_11] gezeigt, parallel geschaltet. Das heißt, der Strom durch jeden einzelnen Widerstand ist $1/11$ des Gesamtstroms. Also ist die Leistung an jedem Widerstand auch nur $1/11$ der Gesamtleistung.

Also ist die zulässige Gesamtleistung $11 \cdot \qty{5}{\watt} =\qty{55}{\watt}$.

<margin>
[picture:1014:e_dummyload_11:Dummyload aus 11 gleich großen Widerständen]
</margin>