Eine Phasenregelschleife (PLL) kann beispielsweise einen variablen und potenziell instabilen VCO mit einem stabilen Referenzoszillator (G) synchronisieren. Dazu vergleicht sie die Phasen beider Signale und regelt den VCO so nach, dass eine stabile Ausgangsfrequenz entsteht. Im Amateurfunk werden PLLs vor allem zur stabilen und präzisen Frequenzaufbereitung in Sendern und Empfängern eingesetzt, etwa zur Kanalwahl, zur Erzeugung von Mischfrequenzen und zur Synchronisation von Oszillatoren.

Eine PLL besteht im Wesentlichen aus folgenden Komponenten:

* *Phasenvergleicher*: Vergleicht die Phasen der Signale vom VCO und vom Referenzoszillator.
* *Tiefpassfilter*: Wandelt die vom Phasenvergleicher erzeugten Impulse in eine Gleichspannung um.
* *VCO*: Erzeugt das Ausgangssignal, dessen Frequenz durch die vom Tiefpassfilter ausgegebene Gleichspannung gesteuert wird.

[question:AD701]

Optional kann die PLL durch einen *Frequenzteiler* ergänzt werden, um die Frequenz des VCOs auf Vielfache der Referenzfrequenz zu synchronisieren.

<margin>
[picture:45:a_oszillator_pll:Darstellung einer Phasenregelschleife (PLL)]  
</margin>

---

Der Phasenvergleicher misst die Phasendifferenz zwischen den Signalen des VCO ($f_\mathrm{out}$) und des Referenzoszillators ($f_\mathrm{ref}$). Bei einer Phasenabweichung gibt er Impulse aus, die dem Fehler entsprechen. Diese Impulse werden durch den Tiefpassfilter geglättet und in eine proportionale Gleichspannung umgewandelt. Die erzeugte Gleichspannung dient als Steuersignal für den VCO, das dessen Frequenz nachreguliert, sodass sich die Phasendifferenz schrittweise auf null reduziert. Ist dieser Zustand erreicht, sagt man, die PLL ist „eingerastet“ (locked) also in einem *stabilen Zustand*. Im stabilen Zustand der PLL sind die Frequenzen und Phasenlagen der beiden Signale identisch. Es gilt:

$f_\mathrm{ref}=\frac{f_\mathrm{out}}{n}$

Die Ausgangsfrequenz ist stabil und entspricht im Wesentlichen der Referenzfrequenz oder deren Vielfachen (je nach gewähltem Teilverhältnis des Frequenzteilers).

Das Funktionsprinzip wird an einem einfachen Beispiel an Abbildung [ref:a_oszillator_pll] deutlich: Der Referenzoszillator liefert am Punkt A eine Frequenz von $f_\mathrm{ref}=\qty{10}{\mega\hertz}$. Die Ausgangsfrequenz des VCO wird am Punkt C durch den Frequenzteiler mit dem Teilerverhältnis $n=100$ geteilt. Ist die PLL eingerastet, also im *stabilen Zustand*, sind die Frequenzen an den Punkten A und B gleich. Daraus ergibt sich für die Ausgangsfrequenz:

$f_\mathrm{out}=n\cdot f_\mathrm{ref}=100\cdot\qty{10}{\mega\hertz}=\qty{1}{\giga\hertz}$

Der VCO erzeugt somit eine Frequenz von $\qty{1}{\giga\hertz}$, die durch den Frequenzteiler auf $\qty{10}{\mega\hertz}$ heruntergeteilt und mit der Referenzfrequenz verglichen wird.

<indepth>
Eine PLL kann analog, digital oder als Mischform aus beiden Techniken aufgebaut werden. In Funkgeräten werden häufig digitale Phasenvergleicher und Frequenzteiler mit einem analogen Schleifenfilter und VCO kombiniert.
</indepth>

[question:AD702]

Die Genauigkeit und Stabilität der PLL-Ausgangsfrequenz hängt in erster Linie von der Qualität des Referenzoszillators ab, welcher üblicherweise ein Quarzoszillator ist.

[question:AD705]

Um eine PLL auf unterschiedliche Frequenzen einzustellen, kann dies durch den Frequenzteiler erfolgen. Dadurch wird es möglich, die Ausgangsfrequenz als ein ganzzahliges Vielfaches der Referenzfrequenz zu erzeugen. Das kleinste wählbare Frequenzintervall entspricht dabei der Frequenz des Referenzoszillators, da die Teilung nur in ganzzahligen Schritten erfolgen kann. Bei einem FM-Funkgerät mit einem Kanalraster von $\qty{12,5}{\kilo\hertz}$ kann daher eine Vergleichsfrequenz von $\qty{12,5}{\kilo\hertz}$ verwendet werden. Wird das Teilerverhältnis $n$ um eins erhöht oder verringert, ändert sich die Ausgangsfrequenz entsprechend um $\qty{12,5}{\kilo\hertz}$. Auf diese Weise kann die PLL auf die einzelnen Funkkanäle eingestellt werden.

[question:AD703]

Um bei gegebener Referenzfrequenz eine bestimmte Ausgangsfrequenz zu erreichen, wird der Teilfaktor so gewählt, dass an den Eingängen des Phasenvergleichers dieselbe Frequenz anliegt. Dadurch lässt sich das benötigte Teilverhältnis für die gewünschte Ausgangsfrequenz berechnen.

[question:AD704]