Gesucht ist der Bereich des Eingangswiderstands der Schaltung. Der linke Widerstand mit $\qty{200}{\ohm}$ liegt immer in Reihe zur restlichen Schaltung.

Nach diesem Widerstand teilt sich die Schaltung in zwei parallele Zweige auf:

* ein Zweig mit $\qty{100}{\ohm}$
* ein Zweig mit $\qty{200}{\ohm} + R$

Zunächst betrachten wir den kleinsten Wert. Dazu setzen wir:

$ R = \qty{0}{\ohm} $

Dann liegt $\qty{100}{\ohm}$ parallel zu $\qty{200}{\ohm}$:

$ R_\mathrm{par} = \frac{\qty{100}{\ohm} \cdot \qty{200}{\ohm}}{\qty{100}{\ohm} + \qty{200}{\ohm}} \approx \qty{67}{\ohm} $

Mit dem vorgeschalteten Widerstand ergibt sich:

$ R_\mathrm{min} = \qty{200}{\ohm} + \qty{67}{\ohm} = \qty{267}{\ohm} $

Nun betrachten wir den größten Wert. Dazu setzen wir:

$ R = \qty{1}{\kilo\ohm} $

Dann liegt $\qty{100}{\ohm}$ parallel zu $\qty{200}{\ohm} + \qty{1}{\kilo\ohm}$, also parallel zu $\qty{1200}{\ohm}$:

$ R_\mathrm{par} = \frac{\qty{100}{\ohm} \cdot \qty{1200}{\ohm}}{\qty{100}{\ohm} + \qty{1200}{\ohm}} \approx \qty{92}{\ohm} $

Mit dem vorgeschalteten Widerstand ergibt sich:

$ R_\mathrm{max} = \qty{200}{\ohm} + \qty{92}{\ohm} = \qty{292}{\ohm} $

Der Eingangswiderstand liegt also im Bereich von etwa $\qtyrange{267}{292}{\ohm}$.