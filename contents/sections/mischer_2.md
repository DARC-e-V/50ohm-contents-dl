<margin>
[picture:804:mischer_linear_vs_nichtlinear:Linearer Widerstand und nichtlineare Diode]
</margin>

Steuerkennlinien von Baugruppen oder Bauelementen können linearen, nichtlinearen oder abschnittsweise gemischten Charakter haben. Zum Beispiel hat ein Widerstand eine lineare Kennline, die Kennlinie einer Diode ist hingegen nichtlinear [ref:mischer_linear_vs_nichtlinear].

Im linearen Bereich von Steuerkennlinien finden keine Verzerrungen der Eingangssignale statt da zu jeder Änderung eines Eingangssignals eine prozentual gleichgroße Änderung des Ausgangssignals erfolgt. Mathematisch entspricht dies einem linearen Verhalten (Addition). Ein Beispiel für eine durchgehend lineare Steuerkennlinie ist ein Widerstand. An linearen Steuerkennlinien oder im linearen Bereich von Steuerkennlinien findet *kein* Mischprozess statt.

Im nichtlinearen Bereich von Steuerkennlinien finden Verzerrungen der Eingangssignale statt, da eine Änderung eines Eingangssignals keine prozentual gleichgroße Änderung eines Ausgangssignals bewirkt. Mathematisch entspricht dies einem nichtlinearen Verhalten bei dem eine Multiplikation der Eingangsgrößen stattfindet und daher zusätzliche Mischprodukte (abhängig von der Form der Kennlinie) entstehen. Daher findet im nichtlinearen Bereich von Steuerkennlinien immer ein Mischprozess statt. Mischprodukte erzeugen immer zusätzliche Frequenzen im Ausgangssignal welche überwiegend als Summen und Differenzen der Eingangsfrequenzen im Ausgangssignal vorliegen.

In der Praxis bilden sich jedoch auch viele unerwünschte Mischprodukte höherer Ordnung, die durch technische Maßnahmen wie Filterung gezielt unterdrückt werden müssen.

[question:AF212]

Ziel eines Mischers ist, dass an dessen Ausgang idealerweise nur die gewünschten Mischprodukte erscheinen und unerwünschte Mischprodukte sowie die Eingangssignale maximal unterdrückt werden.

Am besten erreicht man dieses Ziel mit Hilfe eines sog. Balancemischers. Dieser ist mit 4 Dioden oder Transistoren in Ringschaltung aufgebaut [ref:mischer_ringmischer]. Durch seinen damit symmetrischen Aufbau werden die Eingangssignale im Ausgang maximal unterdrückt. Andere Mischerbauformen wie z.B. Doppeldiodenmischer, Dualtransistormischer sowie additive Diodenmischer leiten durch ihren unsymmetrischen Aufbau immer auch eines der Eingangssignale auf den Ausgang durch.

<indepth>
Funktionsweise eines Ringmischers:

Der Lokal-Oszillator ($U_2$ im Schaubild) schaltet immer zwei gegenüberliegende Dioden während einer Halbwelle leitend, während die beiden anderen Dioden gesperrt sind. In der nächsten Halbwelle des Lokal-Oszillators kehren sich die Verhältnisse genau um. Hierfür muss die Amplitude des Lokal-Oszillators ($U_2$) ausreichend hoch sein, damit die Dioden während der positiven und negativen Halbwellen ausreichend durchgesteuert werden können.

Hierdurch arbeitet der Diodenring als Polwender für das am Eingang anliegende Signal ($U_1$).
Zum erreichen eines guten Mischergebnisses bezüglich unerwünschter Mischprodukte und Unterdrückung des Eingangssignals muss dessen Amplitude deutlich kleiner sein als die Amplitude des Lokal-Oszillators.
Optimale Werte werden durch sog. High-Level-Ringmischer erreicht, deren LO-Eingangspegel im Bereich von bis zu $\qty{10}{\milli\watt}$ liegen können.

<webonly>
[include:applet_ringmodulator]
</webonly>
<latexonly>
[picture:805:mischer_ringmischer:Balancemischer, Ringmischer oder auch Ringmodulator]
</latexonly>
</indepth>

<tip>
Wichtig ist, dass man den Ringmischer von der Schaltung eines Dioden-Gleichrichters, welcher sehr ähnlich aussieht, dadurch unterscheiden kann, dass die Dioden beim Ringmischer hintereinander als Ring geschaltet sind (Kathode jeweils mit folgender Anode der folgenden Diode verbunden). Beim Gleichrichter hingegen sind immer 2 Kathoden und 2 Anoden verbunden.
</tip>
  
Der Balancemischer, der auch als Ringmischer oder Ringmodulator bezeichnet wird, ist am besten geeignet um unerwünschte Ausgangssignale zu unterdrücken.

[question:AF213]
[question:AF214]
