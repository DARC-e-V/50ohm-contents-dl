Im Kapitel zu den grundlegenden Schaltungen haben wir bereits verschiedene Transistorverstärker kennengelernt. Im Sender betrachten wir nun insbesondere *Leistungsverstärker*. Sie verstärken das in den vorherigen Stufen erzeugte HF-Signal auf die gewünschte Ausgangsleistung des Senders.

Bei HF-Leistungsverstärkern kann man grundsätzlich zwischen zwei Ausführungen unterscheiden:

1. *Breitbandige HF-Verstärker* weisen über einen relativ großen Frequenzbereich eine möglichst gleichmäßige Verstärkung auf, beispielsweise über weite Teile des Kurzwellenbereichs von $\qtyrange{1}{30}{\mega\hertz}$, vgl. Abbildung [ref:a_breitbandverstärker].
2. *Selektive HF-Verstärker* sind dagegen auf einen vergleichsweise schmalen Frequenzbereich abgestimmt, beispielsweise auf ein einzelnes Amateurfunkband, vgl. Abbildung [ref:a_selektiver_verstaerker].

Breitbandige HF-Verstärker erkennt man häufig an breitbandigen Koppeltransformatoren zwischen den einzelnen Verstärkerstufen. Diese bilden zusammen mit Kondensatoren keine auf eine bestimmte Frequenz abgestimmten Schwingkreise. Auch das bereits bekannte Prinzip des Gegentaktverstärkers findet man in vielen HF-Leistungsverstärkern wieder.

<margin>
[picture:491:a_breitbandverstärker:Breitbandiger HF-Leistungsverstärker mit Gegentakt-Schaltung]
</margin>

[question:AF412]

Selektive HF-Verstärker erkennt man hingegen typischerweise an deren frequenzselektiver Auslegung, die durch Serien- oder Parallelschwingkreise im HF-Signalpfad gekennzeichnet sind.

<margin>
[picture:778:a_selektiver_verstaerker:Selektiver HF-Leistungsverstärker mit frequenzselektiver Auslegung]
</margin>

[question:AF408]

---

Verstärker der vorgenannten Typen können auch mehrstufig durch Verkettung einzelner Stufen ausgeführt sein.

[question:AF413]

Zwischen Verstärkerstufen eines Leistungsverstärkers und deren Ein- und Ausgängen ist es erforderlich eine Impedanzanpassung vorzunehmen. Dies ist notwendig, damit die HF-Ausgangsimpedanz einer vorherigen Stufe auf die HF-Eingangsimpedanz der folgenden Stufe bestmöglich angepasst wird für maximale Verstärkung und minimale Verzerrungen und optimalen Wirkungsgrad (Vermeidung von Reflexionen und Nichtlinearitäten). 

Die Impedanzanpassung kann entweder breitbandig durch Verwendung eines Transformators mit geeignetem Übersetzungsverhältnis oder frequenzselektiv durch einen angezapften Schwingkreis erfolgen.

Bei frequenzselektiver Anpassung gibt es zwei grundlegende Möglichkeiten diese vorzunehmen:
- durch einen induktiven Spannungsteiler (Spule mit Anzapfung und Parallelkondensator)
- durch einen kapazitiven Spannungsteiler (zwei Kondensatoren in Reihenschaltung mit Spule in Parallelschaltung)

Diese Spulen und Kondenstatoren können in unterschiedlichen Konfigurationen angeordnet sein (Parallel- oder Serienkreis) um die gewünschte Impedanztransformation zu erreichen und gegebenenfalls gleichzeitig Oberwellen zu unterdrücken (Pi-Filter).

[question:AF409]
[question:AF410]
[question:AF414]
[question:AF407]
[question:AF406]

---

Die Abbildung [ref:a_fet_verstaerker] zeigt einen Kurzwellen-Verstärker mit LDMOS Feldeffekttransistoren. LDMOS steht für *Laterally Diffused Metal-Oxide-Semiconductor* und bezeichnet einen speziellen Feldeffekttransistor für HF-Leistungsverstärker. Die eigentliche Verstärkerschaltung (oberer Teil) ist sehr simpel aufgebaut. Es ist wieder ein Gegentaktverstärker mit zwei FETs, die in Push-Pull-Konfiguration arbeiten. Die beiden Transistoren werden über einen gemeinsamen Eingangstransformator angesteuert. Der Ausgang des Verstärkers wird über einen weiteren Transformator abgegriffen. Der untere Teil der Schaltung, ist auch weniger komplex, als man denkt: Im Großen und Ganzen wird hier nur die über einen Spannungsteiler die BIAS-Spannung für die Transistoren erzeugt.

Man darf sich nicht von der bekannten Eigenschaft eines Feldeffekttransistors täuschen lassen: Bei Gleichspannung ist das Gate praktisch stromlos und besitzt daher eine sehr hohe Eingangsimpedanz. Bei hohen Frequenzen spielen jedoch die parasitären Kapazitäten des Transistors eine wichtige Rolle, insbesondere die Kapazitäten zwischen Gate und Source sowie zwischen Gate und Drain. Ihr kapazitiver Blindwiderstand wird mit steigender Frequenz kleiner, sodass am Gate ein HF-Strom fließen kann. Bei HF-Leistungstransistoren kann die Eingangsimpedanz deshalb deutlich niedriger sein als man es von der Gleichstrombetrachtung eines FETs erwarten würde. Der Eingangstransformator $T_1$ dient daher zur Anpassung der $\qty{50}{\ohm}$ an die niederohmige Eingangsimpedanz der Transistoren.

<margin>
[picture:786:a_fet_verstaerker:Kurzwellen-Verstärker mit Feldeffekttransistoren]
</margin>

[question:AF417]

---

Wie oben schon angedeutet benötigen die aktiven Elemente in einem Leistungsverstärker neben der erforderlichen Betriebsspannung auch eine gleichspannungsmäßige Einstellung des Arbeitspunktes (BIAS). Dieser Arbeitspunkt wird üblicherweise durch Spannungsteiler erzeugt die aus einer stabilisierten Hilfsspannung, durch Verwendung von Trimmpotentiometern für eine optimale Einstellung, die gewünschte BIAS-Spannung an den Elementen erzeugen.

<tip>
Bei Betrachtung der BIAS-Spannung und deren Auswirkungen auf die Elemente der Schaltung ist die Schaltung nur gleichspannungsmäßig zu betrachten. Hierbei werden Kondensatoren als Elemente, die nur Wechselspannungen übertragen können, ignoriert. Wicklungen von Transformatoren sowie Spulen werden bei der gleichspannungsmäßigen Betrachtung als Kurzschluss gesehen. Grundsätzlich reicht es bei diesen Aufgaben aus, das Grundwissen aus den Klassen N und E zum Ohmschen Gesetz und Spannungsteilern anzuwenden!
</tip>

[question:AF420]

---

Die Berechnung der BIAS-Spannung bei gegebener Schaltung in der nächsten Frage erfolgt durch Anwendung des Ohmschen-Gesetzes unter Berücksichtigung von Parallel- und Serienschaltung von Widerständen. Wichtig bei der Betrachtung der Frage ist, dass die Gate-Anschlüsse der Transistoren Kapazitäten darstellen und somit bei gleichspannungsmäßiger Betrachtung vernachlässigbar sind.

[question:AF421]

<indepth>
Der Widerstand $R_5=\qty{51}{\ohm}$ beeinflusst die Gleichspannung am Gate praktisch nicht, da in das Gate des LDMOS-Transistors nahezu kein Gleichstrom fließt. Für das HF-Signal ist $R_5$ jedoch wichtig: Er bedämpft zusammen mit der Gate-Kapazität mögliche hochfrequente Schwingungen und verbessert damit die Stabilität des Verstärkers.

Der Widerstand $R_4=\qty{6,8}{\kilo\ohm}$ sorgt dafür, dass das Gate auch bei einer Unterbrechung der Arbeitspunkteinstellung ein definiertes Potential gegen Masse besitzt. Er entlädt außerdem die Gate-Kapazität und verhindert damit, dass der Transistor durch ein frei schwebendes Gate unbeabsichtigt leitend wird, z. B. wenn das Potentiometer $R_3$ defekt ist. Da $R_4$ parallel zum unteren Zweig des Spannungsteilers liegt, muss er bei der genauen Berechnung der Gate-Spannung berücksichtigt werden.
</indepth>

---

Die Schaltung in Abbildung [ref:a_fet_verstaerker_vhf] zeigt einen VHF-Leistungsverstärker mit Feldeffekttransistoren. Auch hier arbeiten die beiden Transistoren als Gegentaktendstufe, was der einfache Teil der Schaltung ist. Die kurzen Koaxialleitungen dienen als Teil des Anpassnetzwerks dazu, die niedrige Impedanz der LDMOS-Transistoren auf eine für die übrige Schaltung geeignete Impedanz zu transformieren. Der Rest ist der Schaltung ist erneut die Erzeugung der BIAS-Spannung für die Transistoren inklusive einer Temperaturkompensation. Die Potentiometer $R_1$ und $R_2$ bilden jeweils einen Spannungsteiler, der die BIAS-Spannung für den jeweiligen Transistor einstellt.

[question:AF424]
[question:AF423]

<margin>
[picture:783:a_fet_verstaerker_vhf:VHF-Verstärker mit Feldeffekttransistoren]
</margin>


---

Ein Pi-Filter (vgl. Abbildung [ref:a_pi_filter]) kann Impedanzen an dessen Ein- und Ausgang durch das Verhältnis der beiden Kapazitäten anpassen. Die Spule des PI-Filters definiert zusammen mit den beiden Kapazitäten die Auslegungsfrequenz des Filters. Das PI-Filter unterdrückt gleichzeitig durch seinen Tiefpass-Charakter unerwünschte Oberwellen des Sendesignals.

<margin>
[picture:1100:a_pi_filter:PI-Filter]
</margin>

[question:AF405]

Ein ähnliche Funktion hat eine LC-Schaltung hinter einem HF-Leistungsverstärker. Auch diese dient der Impedanzanpassung und gleichzeitiger Unterdrückung von Oberwellen.

[question:AF404]

Bei Leistungsverstärkern ist es wichtig die einzelnen Stufen HF-Mäßig von der Betriebsspannung bestmöglich zu entkoppeln um Rückwirkungen auf andere Stufen zu vermeiden (Schwingneigung, Modulationseffekte etc.). Dazu werden die Betriebsspannungszuführungen der einzelnen Stufen mit in Serie geschalteten Induktivitäten sowie Abblockkondensatoren nach Masse gegeneinander entkoppelt. Diese Anordnung stellt einen Tiefpass dar, da im Idealfall nur die gewünschte DC-Betriebsspannung durchgelassen wird, HF-Anteile jedoch abgeblockt werden.

[question:AF411]
[question:AF419]
[question:AF418]
[question:AF422]

Die HF-Eigenschaften realer Kondensatoren sind frequenzabhängig. Große Kapazitäten wie Elektrolytkondensatoren können nur bei niedrigen Frequenzen eingesetzt werden und sind im HF-Bereich nur bedingt wirksam. Um auch höhere Frequenzen durch Kondensatoren abzublocken verwendet man häufig eine Kombination aus unterschiedlichen Kondensatortypen und Kapazitätswerten, die zusammen einen größeren Frequenzbereich abblocken können.

[question:AF415]