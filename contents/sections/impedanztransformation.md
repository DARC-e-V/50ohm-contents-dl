Nicht jede Antenne besitzt an ihrem Speisepunkt genau die Impedanz, die für den Anschluss an eine bestimmte Speiseleitung oder einen Sender benötigt wird. Weicht die Impedanz beispielsweise von den üblichen $\qty{50}{\ohm}$ ab, muss sie entsprechend angepasst werden, damit die HF-Leistung möglichst verlustarm übertragen werden kann. Dazu wird die vorhandene Impedanz in eine andere, gewünschte Impedanz *transformiert*. Dies bezeichnet man als *Impedanztransformation* beziehungsweise *Impedanzanpassung*.

Für die Impedanzanpassung bzw. Impedanztransformation gibt es verschiedene Möglichkeiten. Häufig verwendet werden beispielsweise:

* Transformatoren,
* $\frac{\lambda}{4}$-Leitungen oder
* Anpassnetzwerke aus Spulen und Kondensatoren.

Transformatoren haben wir bereits bei der endgespeisten Antenne mit 1:49 Unun kennengelernt. Im Folgenden betrachten wir deshalb zwei weitere Möglichkeiten genauer: die Impedanztransformation mit $\frac{\lambda}{4}$-Leitungen aus dem Vorherigen Abschnitt und die Anpassung mit LC-Netzwerken. Schauen wir zunächst nochmal auf die Transformationsleitungen, hier ist es übrigens egal ob wir eine symmetrische Speiseleitung oder eine unsymmetrische Koaxialleitung verwenden, die Transformation funktioniert in beiden Fällen:

Bei einer Leitung, deren elektrische Länge $\lambda/4$ beträgt, werden Wirkwiderstände, die kleiner als der Wellenwiderstand der Leitung sind, zu Widerständen die größer als der Wellenwiderstand der Leitung sind. Umgekehrt werden Wirkwiderstände, die größer als der Wellenwiderstand der Leitung sind, zu Widerständen die kleiner als der Wellenwiderstand sind. Diesen Umstand macht man sich z.B. zunutze, um  hochohmige Antennen auf ein niederohmiges System ($\qty{50}{\ohm}$) anzupassen.

[question:AG410]
[question:AG409]

Bei einer Leitungslänge von $\lambda/2$ hebt sich der Effekt jedoch wieder auf, so dass keine Impedanztransformation auftritt.

[question:AG412]
[question:AG416]

Für die folgenden Fragen erinnern wir uns daran, dass ein Halbwellendipol stromgespeist wird (niederohmig) und ein Ganzwellendipol spannungsgespeist wird (hochohmig).

[question:AG413]
[question:AG414]
[question:AG415]

Möchte man auf einen bestimmten Widerstandswert transformieren, so ergibt sich der dazu notwendige Wellenwiderstand aus dem geometrischen Mittel aus Lastwiderstand $Z_\mathrm{A}$ und gewünschtem Speisewiderstand $Z_\mathrm{E}$ am anderen Ende des Kabels:

$Z = \sqrt{Z_\mathrm{E} \cdot Z_\mathrm{A}}$

[question:AG417]
[question:AG418]

---

Oftmals werden jedoch auch Spulen und Kondensatoren zur Impedanzanpassung benutzt. Oft zu finden ist das sogenannte Pi-Filter, das neben seiner Wirkung als Tiefpass eine Impedanztransformation zur Folge hat. Entsprechend lässt sich ein solches Pi-Filter auch als Antennentuner benutzen.

<indepth>
*Der Name "Pi-Filter"* stammt von der Anordnung der Bauteile im Schaltbild, die an den griechischen Buchstaben $\pi$ erinnert, und hat nichts mit der Kreiszahl $\pi$ zu tun.
</indepth>

[question:AG406]
