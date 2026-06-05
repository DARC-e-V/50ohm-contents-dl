Leistungsverstärker werden im Amateurfunkbereich zur Verstärkung des intern erzeugten HF-Signals aus vorherigen Stufen verwendet, um die gewünschte Ausgangsleistung des Senders zu erzielen. Hierbei unterscheidet man grundlegend in 2 Typen von HF-Verstärkern. Zum einen breitbandige HF-Verstärker, welche eine gleichbleibende Verstärkung über einen relativ breiten Frequenzbereich haben (z.B. Kurzwellenbereich $\qtyrange{1}{30}{\mega\hertz}$). Zum anderen selektive HF-Verstärker, welche das Maximum Ihrer Verstärkung nur in einem schmalen Frequenzbereich haben (z.B. nur in einem Amateurband des Kurzwellenbereichs).

Breitbandige HF-Verstärker erkennt man typischerweise an breitbandigen Koppeltransformatoren zwischen den einzelnen Verstärkerstufen, die **nicht** mittels einer Parallel- oder Serienkapazität als Schwingkreis ausgebildet sind.

Selektive HF-Verstärker erkennt man hingegen typischerweise an deren frequenzselektiver Auslegung, die durch Serien- oder Parallel-Schwingkreise im HF-Signalpfad gekennzeichnet sind.



[question:AF412]
[question:AF408]

Verstärker der vorgenannten Typen können auch mehrstufig durch Verkettung einzelner Stufen ausgeführt sein.

[question:AF413]

Zwischen Verstärkerstufen eines Leistungsverstärkers und deren Ein- und Ausgängen ist es erforderlich eine Impedanzanpassung vorzunehmen. Dies ist notwendig, damit die HF-Ausgangsimpedanz einer vorherigen Stufe auf die HF-Eingangsimpedanz der folgenden Stufe bestmöglich angepasst wird für maximale Verstärkung und minimale Verzerrungen und optimalen Wirkungsgrad (Vermeidung von Reflexionen und Nichtlinearitäten). 

Die Impedanzanpassung kann entweder breitbandig durch Verwendung eines Transformators mit geeignetem Übersetzungsverhältnis oder frequenzselektiv durch einen angezapften Schwingkreis erfolgen.

Bei frequenzselektiver Anpassung gibt es zwei grundlegende Möglichkeiten diese vorzunehmen:
- durch einen induktiven Spannungsteiler (Spule mit Anzapfung und Parallelkondensator)
- durch einen kapazitiven Spannungsteiler (zwei Kondensatoren in Reihenschaltung mit Spule in Parallelschaltung)

Diese Spulen und Kondenstatoren können in unterschiedlichen Konfigurationen angeordnet sein (Parallel- oder Serien-kreis) um die gewünschte Impedanztransformation zu erreichen und gegebenenfalls gleichzeitig Oberwellen zu unterdrücken (Pi-Filter).

[question:AF409]
[question:AF410]
[question:AF414]
[question:AF407]
[question:AF406]
[question:AF417]

Ein Pi-Filter kann Impedanzen an dessen Ein- und Ausgang durch das Verhältnis der beiden Kapazitäten anpassen. Die Spule des PI-Filters definiert zusammen mit den beiden Kapazitäten die Auslegungsfrequenz des Filters. Das PI-Filter unterdrückt gleichzeitig durch seinen Tiefpass-Charakter unerwünschte Oberwellen des Sendesignals.

[question:AF405]

Ein ähnliche Funktion hat eine LC-Schaltung hinter einem HF-Leistungsverstärker. Auch diese dient der Impedanzanpassung und gleichzeitiger Unterdrückung von Oberwellen.

[question:AF404]

Der Wirkungsgrad eine HF-Leistungsverstärkers wird definiert durch das Verhältnis der vom Leistungsverstärker abgegebenen HF-Ausgangsleistung und der dem Verstärker zugeführten Gleichstrom-Versorgungsleistung.

[question:AF401]

Die aktiven Elemente in einem Leistungsverstärker benötigen neben der erforderlichen Betriebsspannung auch eine gleichspannungsmäßige Einstellung des Arbeitspunktes (BIAS). Dieser Arbeitspunkt wird üblicherweise durch Spannungsteiler erzeugt die aus einer stabilisierten Hilfsspannung, durch Verwendung von Trimmpotentiometern für eine optimale Einstellung, die gewünschte BIAS-Spannung an den Elementen erzeugen.
Bei Betrachtung der BIAS-Spannung und deren Auswirkungen auf die Elemente der Schaltung ist die Schaltung nur gleichspannungsmäßig zu betrachten. Hierbei werden Kondensatoren als Elemente, die nur Wechselspannungen übertragen können, ignoriert.
Wicklungen von Transformatoren sowie Spulen werden bei der gleichspannungsmäßigen Betrachtung als Kurzschluss gesehen.

[question:AF420]
[question:AF423]
[question:AF424]

%TODO Fragennummern fixen
%TODO doe Frage 2373 bräuchte eine genauerer Erklärung wie man auf die 3.5 V kommt (370||6800 = 350).

Die Berechnung der BIAS-Spannung bei gegebener Schaltung (Frage AF421) erfolgt durch Anwendung des Ohmschen-Gesetzes unter Berücksichtigung von Parallel- und Serienschaltung von Widerständen. Wichtig bei der Betrachtung der Frage ist, dass die Gate-Anschlüsse der Transistoren Kapazitäten darstellen und somit bei gleichspannungsmäßiger Betrachtung vernachlässigbar sind.

[question:AF421]

Bei Leistungsverstärkern ist es wichtig die einzelnen Stufen HF-Mäßig von der Betriebsspannung bestmöglich zu entkoppeln um Rückwirkungen auf andere Stufen zu vermeiden (Schwingneigung, Modulationseffekte etc.). Dazu werden die Betriebsspannungs-Zuführungen der einzelnen Stufen mit in Serie geschalteten Induktivitäten sowie Abblock-Kondensatoren nach Masse gegeneinander entkoppelt. Diese Anordnung stellt einen Tiefpass dar, da im Idealfall nur die gewünschte DC-Betriebsspannung durchgelassen wird, HF-Anteile jedoch abgeblockt werden.

[question:AF411]
[question:AF419]
[question:AF418]
[question:AF422]

Die HF-Eigenschaften realer Kondensatoren sind frequenzabhängig. Große Kapazitäten wie Elektrolytkondensatoren können nur bei niedrigen Frequenzen eingesetzt werden und sind im HF-Bereich nur bedingt wirksam. Um auch höhere Frequenzen durch Kondensatoren abzublocken verwendet man häufig eine Kombination aus unterschiedlichen Kondensator-Typen und Kapazitäts-Werten, die zusammen einen größeren Frequenzbereich abblocken können.

[question:AF415]

Um die Gesamtverstärkung eines mehrstufigen Leistungsverstärkers zu ermitteln muss die Differenz zwischen Ausgangs- und Eingangsleistung durch vorzeichenrichtige Subtraktion der dBm-Werte vorgenommen werden. Beispiel: Eingangsleistung $\qty{-5}{\dBm}$, Ausgangsleistung $\qty{20}{\dBm}$ ergibt eine Gesamtverstärkung von $\qty{25}{\dB}$ ($\qty{20}{\dBm} - (\qty{-5}{\dBm}) = \qty{25}{\dB}$)

[question:AF428]