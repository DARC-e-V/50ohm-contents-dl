Im Amateurfunk haben wir es häufig sowohl mit sehr großen als auch mit sehr kleinen Zahlen zu tun. Die Einheit der Frequenz – das Hertz ($\unit{\hertz}$) – sowie die typischen Vorsätze für große Zahlen wie *Kilo* ($\unit{\kilo}$), *Mega* ($\unit{\mega}$) und *Giga* ($\unit{\giga}$) sind uns bereits begegnet.

Auch für kleine Zahlen gibt es solche Einheitenvorsätze. Bekannt ist zum Beispiel *Milli*, abgekürzt mit $\unit{\milli}$. Ein Millimeter entspricht einem Tausendstel Meter, also $\qty{0,001}{\meter}$. Die am meisten verwendeten Vorsätze für große und kleine Zahlen stehen in Tabelle [ref:e_einheitenvorzeichen].

<margin>
| c: Vorsatz | c: Abkürzung | l: Wert |
| Pico | $\unit{\pico}$ | $10^{-12} = 0,000000000001$ |
| Nano | $\unit{\nano}$ | $10^{-9} = 0,000000001$ |
| Mikro | $\unit{\micro}$ | $10^{-6} = 0,000001$ |
| Milli | $\unit{\milli}$ | $10^{-3} = 0,001$ |
| |  | $10^{0} = 1$ |
| Kilo | $\unit{\kilo}$ | $10^{3} = 1000$ |
| Mega | $\unit{\mega}$ | $10^{6} = 1000000$ |
| Giga | $\unit{\giga}$ | $10^{9} = 1000000000$ |
[table:e_einheitenvorzeichen:Einheitenvorsätze für Zehnerpotenzen]
</margin>

Neben den Einheiten Hertz und Meter, die wir bereits kennengelernt haben, gibt es noch viele weitere physikalische Einheiten, auf die wir im weiteren Verlauf des Kurses eingehen werden. Dazu gehören zum Beispiel die elektrische Spannung, gemessen in Volt ($\unit{\volt}$), der elektrische Strom in Ampere ($\unit{\ampere}$), die Leistung in Watt ($\unit{\watt}$), der elektrische Widerstand in Ohm ($\unit{\ohm}$) und weitere.

Um die folgenden Sachverhalte verstehen zu können, ist es noch nicht notwendig, diese Einheiten im Detail zu kennen. Wichtig ist zunächst nur, die Bedeutung und Anwendung der Einheitenvorsätze zu verstehen.

Leider kann man diese gezeigten Einheitenvorsätze nicht direkt in jeden Taschenrechner eingeben. Man verwendet dafür sogenannte Zehnerpotenzen.

---

Schauen wir uns das zunächst am Beispiel des Vorsatzes Kilo an, der für $1000$ steht: Statt $1000$ kann man auch $10 \cdot 10 \cdot 10$ schreiben. Dafür gibt es die Abkürzung $10^3$ (gesprochen "10 hoch 3" oder "3. Potenz von 10"). Die Angaben $\qty{1500}{\hertz}$, $\qty{1,5}{\kilo\hertz}$ und $\qty{1,5e3}{\hertz}$ stehen für den selben Wert.

<tip>
Man kann es sich auch anders merken: Man multipliziert die Zahl so oft mit 10, wie die Hochzahl (der Exponent) angibt. Bei Zahlen ohne Komma hängt man einfach so viele Nullen an, wie im Exponent steht.
</tip>

Für eine Million muss man nicht drei, sondern sechs Exemplare der Zahl 10 miteinander multiplizieren. Also entspricht der Vorsatz Mega dem Wert $10^6$. Die Schreibweise $\qty{28e6}{\hertz}$ bedeutet demnach dasselbe wie $\qty{28}{\mega\hertz}$.

Für kleine Zahlen funktioniert es ähnlich. Ein Tausendstel ist $\frac{1}{10} \cdot \frac{1}{10} \cdot \frac{1}{10}$. Das schreibt man als $10^{-3}$ ("zehn hoch minus drei"). Der Wert $\qty{3,5e-3}}{\volt}$ ist also nichts anderes als $\qty{3,5}{\milli\volt}$ und $\qty{22e-6}{\volt}$ steht für $\qty{22}{\micro\volt}$. Die wichtigsten Zehnerpotenzen stehen wieder in Tabelle [ref:e_einheitenvorzeichen].

---

Technisch-wissenschaftliche Taschenrechner verfügen in der Regel über eine Taste für Potenzen, meist bezeichnet mit $x^y$. Manche Modelle bieten zusätzlich eine vereinfachte Eingabemöglichkeit für Zehnerpotenzen: eine Taste mit der Beschriftung *Exp*, *E* oder $\cdot 10^x$. Diese steht für "mal zehn hoch …" und erleichtert die Eingabe sehr großer oder sehr kleiner Zahlen.

Beispiel: Um den Wert $\num{3,5e6}$ einzugeben, drückt man: 3.5 → Exp → 6

<tip>
Schau am besten in die Bedienungsanleitung deines Taschenrechners, um die genaue Tastenkombination zu finden.
</tip>

Die Anzeige besonders großer oder kleiner Werte hängt vom Gerät ab. Manche schreiben sie als gewöhnliche Zehnerpotenzen, andere mit *Exp* oder *E* für *mal 10 hoch*. Oft schaltet die Taste *S/D* zwischen verschiedenen Darstellungen um. In der Zehnerpotenz-Schreibweise verschieben Tasten wie *ENG*, *<ENG* oder *ENG>* das Komma oder hängen am Schluss Nullen an und passen dabei die Hochzahl so an, dass sich der Wert nicht ändert. Schau am besten hier in die Bedienungsanleitung deines Taschenrechners.

---

Abbildung [ref:e_taschenrechner] zeigt drei Darstellungen der selben Zahl in einer Taschenrechner-App. Die drei Buttons für den Umgang mit Zehnerpotenzen wurden rot markiert.

<margin>
[photo:172:e_taschenrechner:Verschiedene Darstellungen der Zahl 0,007 in einer Taschenrechner-App]
</margin>

Im Folgenden findest du mehrere Prüfungsfragen, die du mithilfe deines Taschenrechners lösen kannst. Gib dazu die jeweilige Zahl entsprechend der Aufgabenstellung ein – achte dabei gegebenenfalls auf die Einheitenpräfixe und verwende den Exponentialmodus. Mit der ENG-Taste kannst du die Umrechnung automatisch durchführen lassen.

Mit etwas Übung lassen sich die Aufgaben natürlich auch im Kopf lösen. Die Einheiten können in diesen Beispielen vernachlässigt werden, da es hier in erster Linie auf die korrekte Darstellung in Exponentialschreibweise bzw. auf den passenden Einheitenpräfix ankommt. In zukünftigen Berechnungen wird es zunehmend wichtig sein, ein Ergebnis mit einem bestimmten Einheitenpräfix auszuwählen oder entsprechend umzurechnen.

%EA110
[question:EA110]
%EA109
[question:EA109]
%EA108
[question:EA108]
%EA116
[question:EA116]
%EA114
[question:EA114]
[question:EA111]
[question:EA112]
[question:EA115]
[question:EA113]