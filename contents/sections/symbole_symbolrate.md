Bei digitalen Übertragungen werden Informationen in Form von Symbolen übertragen. Ein Symbol ist dabei ein unterscheidbarer Signalzustand, der für eine bestimmte Zeit übertragen wird. Diese Signalzustände können sich beispielsweise durch unterschiedliche Amplituden, Frequenzen oder Phasen beziehungsweise durch Kombinationen dieser Eigenschaften unterscheiden. Wie solche Symbole erzeugt werden, betrachten wir in den folgenden Abschnitten. Je nachdem, wie viele unterschiedliche Symbole ein Übertragungsverfahren verwenden kann, kann ein einzelnes Symbol ein oder mehrere Bits an Information enthalten.

Stehen nur zwei unterschiedliche Symbole zur Verfügung, kann mit jedem Symbol genau ein Bit übertragen werden. Bei vier möglichen Symbolen können bereits zwei Bit mit einem Symbol übertragen werden, da sich mit zwei Bit vier verschiedene Kombinationen darstellen lassen. Entsprechend können acht unterschiedliche Symbole drei Bit und $\num{16}$ unterschiedliche Symbole vier Bit gleichzeitig übertragen.

Allgemein ergibt sich die Anzahl $N$ der mit einem Symbol übertragbaren Bits aus der Anzahl $M=2^N$ der möglichen Symbole:

$N = \log_2(M)$

Die *Symbolrate* gibt an, wie viele Symbole pro Sekunde übertragen werden. Ihre Einheit ist *Baud*. Eine Symbolrate von $\qty{1000}{\baud}$ bedeutet also, dass pro Sekunde $\num{1000}$ Symbole übertragen werden.

Die Symbolrate ist nicht zwangsläufig mit der Datenrate identisch. Werden mit jedem Symbol mehrere Bits übertragen, ist die Datenrate entsprechend größer. Für die Datenrate $R_\mathrm{D}$ (mit der Einheit $\unit{\bit\per\second}$) und die Symbolrate $R_\mathrm{S}$ gilt:

$R_\mathrm{D} = R_\mathrm{S} \cdot N$

Werden beispielsweise bei einer Symbolrate von $\qty{1200}{\baud}$ mit jedem Symbol zwei Bit übertragen, ergibt sich eine Datenrate von:

$R_\mathrm{D} = \qty{1200}{\baud} \cdot 2 = \qty{2400}{\bit\per\second}$

Die Anzahl der möglichen Symbole und die Symbolrate sind damit wichtige Größen für digitale Übertragungsverfahren. Wie sich die einzelnen Symbole durch unterschiedliche Eigenschaften eines Signals darstellen lassen, betrachten wir in den folgenden Abschnitten.

[question:AA104]

---

Ein einfaches Beispiel dafür, wie unterschiedliche Symbole durch verschiedene Signalzustände dargestellt werden können, ist die bereits aus Klasse E bekannte *Frequenzumtastung* (*Frequency-Shift Keying*, FSK).

Bei FSK wird die Frequenz des ausgesendeten Signals zwischen verschiedenen Werten umgeschaltet. Die Abbildung [ref:a_fsk] zeigt eine binäre FSK mit zwei möglichen Symbolfrequenzen in der Zeitdarstellung. Beispielsweise kann die höhere Frequenz für das Symbol $1$ und die niedrigere Frequenz für das Symbol $0$ stehen. Da zwei verschiedene Symbole zur Verfügung stehen, kann mit jedem Symbol ein Bit übertragen werden.

<margin>
[picture:703:a_fsk:FSK (Frequency-Shift Keying)]
</margin>

Ein Beispiel ist *RTTY*. Hier wird zwischen zwei Symbolfrequenzen umgetastet, beispielsweise zwischen $\qty{14072,43}{\kilo\hertz}$ und $\qty{14072,60}{\kilo\hertz}$. Mit jedem Symbol kann damit ein Bit, also $0$ oder $1$, übertragen werden.

[question:AE405]

FSK ist jedoch nicht auf zwei Symbolfrequenzen beschränkt. Werden beispielsweise vier unterschiedliche Frequenzen verwendet, stehen vier verschiedene Symbole zur Verfügung. Jedem Symbol kann dann eine der vier möglichen Bitkombinationen $00$, $01$, $10$ oder $11$ zugeordnet werden. Dadurch können mit jedem Symbol zwei Bit übertragen werden.

Ein Beispiel dafür ist das Übertragungsverfahren *FT4*. Hier kann zwischen vier Symbolfrequenzen umgetastet werden, beispielsweise $\qty{14081,20}{\kilo\hertz}$, $\qty{14081,40}{\kilo\hertz}$, $\qty{14081,61}{\kilo\hertz}$ und $\qty{14081,83}{\kilo\hertz}$.

[question:AE406]