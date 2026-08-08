<margin>
[picture:804:mischer_linear_vs_nichtlinear:Linearer Widerstand und nichtlineare Diode]
</margin>


Bauelemente und Baugruppen können sich *linear* oder *nichtlinear* verhalten. Bei einem linearen Bauelement folgt die Ausgangsgröße der Eingangsgröße nach einem festen Zusammenhang. Ein idealer Widerstand besitzt beispielsweise eine lineare Kennlinie. Die Kennlinie einer Diode ist dagegen nichtlinear (vgl. [ref:mischer_linear_vs_nichtlinear]).

Für einen Mischprozess reicht ein rein lineares Verhalten nicht aus. Werden mehrere Signale durch eine lineare Schaltung übertragen, können sie zwar verstärkt, abgeschwächt oder miteinander addiert werden, sie beeinflussen sich dabei jedoch nicht gegenseitig. Es entstehen dadurch keine neuen Frequenzanteile.

Damit eine Mischung stattfinden kann, müssen die Eingangssignale miteinander verknüpft werden. Dies kann beispielsweise durch die nichtlineare Kennlinie einer Diode oder eines Transistors geschehen. Eine weitere häufig verwendete Möglichkeit besteht darin, das Eingangssignal mit Hilfe des Oszillatorsignals schnell ein- und auszuschalten beziehungsweise umzupolen. Auch ein solcher Schaltvorgang ist kein linearer Vorgang und bewirkt, dass beide Signale miteinander verknüpft werden.

Genau diese Eigenschaft wird in einem Mischer gezielt ausgenutzt. Deshalb arbeiten Mischstufen mit nichtlinearen Bauelementen oder mit Schaltungen, in denen Transistoren oder Dioden durch das Oszillatorsignal geschaltet werden.
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
