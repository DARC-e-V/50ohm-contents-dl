Den Bipolartransistor hatten wir bereits in den Ausbildungsunterlagen zur Klasse E ausführlich diskutiert. Er besteht aus drei Halbleiterzonen, die abwechselnd n- und p-dotiert sind. Die Zonen bezeichnet man als Emitter, Basis und Kollektor. Beim *npn-Transistor* ist der Emitter n-, die Basis p- und der Kollektor n-dotiert. Beim pnp-Transistor ist es entsprechend ein p-Emitter, eine n-Basis und ein p-Kollektor. 

[question:AC503]
[question:AC504]

[question:AC501]

Physikalisch steuert die Basis-Emitter-Spannung $U_{BE}$ den Kollektorstrom $I_C$ und zwar exponentiell. Beim npn-Transistor gilt zum Beispiel:

$I_C = I_S \cdot \exp\left(\frac{U_{BE}}{U_T}\right)$

$I_S$ ist der Sättigungsstrom, der stark von der Bauart des Transistors abhängt. Er ist dem Datenblatt zu entnehmen. $U_T$ ist die sogenannte Temperaturspannung, die bei Raumtemperatur etwa $\qty{26}{\milli\volt}$ beträgt.

Ein Unterschied zum später betrachteten Feldeffekt-Transistor ist, dass beim Bipolartransistor immer auch ein Strom im Eingang (der Basis) fließt, der Basisstrom $I_B$. Auch er ist exponentiell von $U_{BE}$ abhängig, wobei $I_S$ um einen Faktor $B$ kleiner ist als beim Kollektorstrom.

$I_B = \frac{I_S}{B} \cdot \exp \left(\frac{U_{BE}}{U_T}\right)$

Der Faktor $B$ ist also der Quotient aus Kollektor- und Basisstrom:

$B = \frac{I_C}{I_B}$

Es ist deshalb praktisch, sich den Bipolartransistor als *stromgesteuert* vorzustellen. Dies ist die gewünschte Antwort auf die obige Frage, auch wenn es physikalisch nicht ganz korrekt ist.

[question:AC505]

Ein Transistor wird hier als "leitend" bezeichnet, wenn ein signifikanter Kollektorstrom fließt. Dazu muss die Basis-Emitter-Diode stets in Flussrichtung geschaltet sein, also $U_{BE}$ positiv bei npn- und negativ bei pnp-Transistoren. Die Kollektor-Basis-Diode dagegen muss sperren, denn es sollen keine Ladungsträger aus dem Kollektor in die Basis injiziert werden.

[question:AC502]

Feldeffekt-Transistoren haben ein ganz anderes Steuerprinzip als Bipolartransistoren. Während bei Bipolartransistoren sowohl Elektronen also auch Defektelektronen ("Löcher") betrachtet werden müssen (daher "bipolar"), ist beim Feldeffekt-Transistor nur eine Ladungsträgersorte beteiligt ("unipolar"). Dies können entweder Elektronen (*n-Kanal-Feldeffekt-Transistor*) oder Löcher (*p-Kanal-Feldeffekt-Transistor*) sein.

Allen Feldeffekt-Transistoren (oder *FETs*) gemein ist, dass im normalen Betrieb kein Strom im Eingang, der Gate-Elektrode, fließt. Die Steuerung der Ladung im Kanal (dem Bereich zwischen *Source* und *Drain*) ist ausschließlich von der Gate-Source-Spannung abhängig.

[question:AC512]

Die Elektroden des FET werden wie folgt bezeichnet:

* *Source*: dies ist die "Quelle" (engl. source) für die Ladungsträger im Kanal. Nicht verwirren lassen: die sogenannte technische Stromrichtung ist entgegen der Ladungsträger-Flussrichtung definiert!
* *Drain*: dies ist der Abfluss (engl. drain) für die Ladungsträger im Kanal.
* *Gate*: Das Gate (englisch für Gatter) steuert den Fluss der Ladungsträger im Kanal.

Die hier zur Verwirrung eingestreuten Begriffe Emitter, Basis, Kollektor beziehen sich auf den Bipolartransistor.

[question:AC513]

[question:AC514]

Wie wir bereits festgestellt hatten, ist der FET ein *spannungsgesteuertes* Bauelement, in dem kein Gate-Strom fließt. Die gewünschte Antwort ist die, dass die Gate-Source-Spannung den *Kanalwiderstand* steuert. Allerdings kann das Verhalten des Kanals nur für sehr kleine Drain-Source-Spannungen als Widerstand beschrieben werden, in sofern ist die Antwort etwas unglücklich formuliert. Besser wäre: die Gate-Source-Spannung steuert den Kanalstrom.

[question:AC506]

Die senkrechte Linie symbolisiert den Kanal, die oben (Drain) und unten (Source) kontaktiert wird. Links ist das Gate zu sehen -- der Pfeil erinnert zusammen mit dem senkrechten Strich an eine Diode. Es handelt sich also um einen FET, genau genommen einen Sperrschicht-FET.

Bei den folgenden Fragen geht es darum, bestimmte FET-Typen ihrem Schaltsymbol zuzuordnen. Dazu ein paar Grundregeln:

* Der Strom im Kanal kann entweder von Elektronen oder von Löchern getragen werden. Wir sprechen im ersten Fall von einem *n-Kanal-FET*, im zweiten Fall von einem *p-Kanal-FET*.
* Wir können FETs auch danach unterscheiden, ob für eine Gate-Source-Spannung $U_{GS}=0$ ein Strom im Kanal fließt oder nicht. Sie heißen dann entweder *selbstleitend* oder *selbstsperrend*. 
* Schließlich können wir FETs danach unterscheiden, ob die Gate-Elektrode eine Diode ist, oder eine Kondensator-Struktur. Ist Gate eine Diode, sprechen wir von  einem Sperrschicht-FET. Beispiele sind der JFET (junction field effect transistor) und der MESFET (metal semiconductor field effect transistor). Beim MESFET ist die Gate-Diode eine Schottky-Diode. Bei einem *Isolierschicht-FET* ist die Gate-Elektrode durch einen Isolator (ein Dielektrikum) vom Kanal getrennt. Die anliegende Spannung steuert die Dichte von Ladungsträgern im Kanal. Ist der Isolator ein Oxid, zum Beispiel Siliziumdioxid, sprechen wir auch von einem MOSFET (metal oxide semiconductor FET). Wegen ihrer Verwendung in Digitalschaltkreisen sind MOSFETs mit sehr weitem Abstand die häufigsten Transistortypen.

Der Pfeil zeigt an, ob es sich um einen n- oder p-Kanal-FET handelt. Wie bei der Diode zeigt der Pfeil auf die Kathode, also den n-dotierten Bereich. Zeigt also der Pfeil auf den Kanal, handelt es sich um einen n-Kanal-FET. Beim Sperrschicht-FET trägt das Gate den Kanal, beim Isolierschicht-FET ist der Pfeil zwischen Kanal und der sogenannten Bulk-Schicht zu sehen, die unter dem Kanal liegt und meist intern mit der Source-Elektrode verbunden ist.

Im Isolierschicht-FET bilden Gate und Kanal auch grafisch einen Kondensator.

Beim selbstleitenden FET geht die Linie zwischen Source und Drain durch, während sie beim selbstsperrenden FET unterbrochen ist.

[question:AC507]
[question:AC508]
[question:AC509]
[question:AC510]
[question:AC511]

Im Folgenden betrachten wir noch ein paar einfache Transistor-Schaltungen.

[question:AC515]

Der gewünschte Arbeitspunkt wird dadurch eingestellt, dass über $R_1$ ein Basisstrom eingeprägt wird. Der Basisstrom ist um die gegebene Stromverstärkung von 298 kleiner als der Kollektorstrom. Über dem Widerstand fällt die Differenz von Betriebsspannung und Basispotential ab. Das Basispotential ist mit $\qty{0,6}{\volt}$ gegeben. Also rechnen wir:

$R_1 = 298 \cdot \frac{\qty{12}{\volt} - \qty{0,6}{\volt}}{\qty{0,005}{\ampere}} \approx \qty{680}{\kilo\ohm}$

Die Schaltung hat allerdings in der Praxis einen gewaltigen Nachteil: die Stromverstärkung eines Bipolartransistors ist nicht besonders gut kontrolliert. Nehmen wir als Beispiel den populären BC547B. Seine Stromverstärkung kann nach Spezifikation zwischen 200 und 450 liegen. Der Kollektorstrom kann also mit dieser Schaltung durchaus um mehr als einen Faktor 2 vom Entwurf abweichen.

[question:AC516]

In Frage AC516 wird der Arbeitspunkt des Bipolartransistors über einen Spannungsteiler eingestellt. Der sogenannte Querstrom ist der Strom, der hier durch $R_2$ fließt. Er sollte mindestens zehnmal so hoch wie der Basisstrom sein, damit der Basisstrom keinen großen Einfluss auf den Arbeitspunkt hat. 

Allerdings ist auch diese Schaltung nicht sehr empfehlenswert. Zum einen hängt der Kollektorstrom exponentiell von der Basis-Emitter-Spannung ab. Die Widerstände haben eine Toleranz, durch die das Basispotential durchaus etwas vom Soll abweichen kann -- mit einer großen Auswirkung auf den Kollektorstrom. Außerdem ist die Schwellspannung der Basis-Emitter-Diode mit etwa $\qty{-2}{\milli\volt\per\kelvin}$ recht stark temperaturabhängig. Daher wird diese Schaltung einen starken Temperaturgang des Kollektorstroms haben. Das kann manchmal erwünscht sein, aber man muss es im Blick haben.

[question:AC518]

Der Spannungsteiler $R_1$ und $R_2$ stellt das Basispotential ein, das, weil der Emitter auf Masse liegt, etwa $\qty{0,6}{\volt}$ betragen muss. Bei einem Kollektorstrom von $\qty{2}{\milli\ampere}$ und einer Stromverstärkung von $\num{200}$ ist der Basisstrom $\qty{2}{\milli\ampere} / 200 = \qty{10}{\micro\ampere}$. Der Strom durch $R_2$ soll der zehnfache Basisstrom sein, durch $R_1$ fließt  $11 \cdot \qty{10}{\micro\ampere} = \qty{110}{\micro\ampere}$. Der Widerstand $R_1$ ist dann:

$R_1 = \frac{\qty{10}{\volt} - \qty{0,6}{\volt}}{\qty{110}{\micro\ampere}} = \qty{85,5}{\kilo\ohm}$

[question:AC517]

Die obige Schaltung zeigt eine typische Arbeitspunkteinstellung für den Bipolartransistor. Das Basispotential wird über den Spannungsteiler $R_1$ und $R_2$ festgelegt. Da über dem Emitterwiderstand $R_E$ $\qty{1}{\volt}$ abfallen soll, muss das Basispotential auf $\qty{1,6}{\volt}$ betragen. Bei einem Kollektorstrom von $\qty{2}{\milli\ampere}$ und einer Stromversorgung von 200 beträgt der Basisstrom $\qty{10}{\micro\ampere}$. Da der Strom durch $R_2$ der zehnfache Basisstrom fließen soll, fließt durch $R_1$ der elffache Basisstrom, also $\qty{110}{\micro\ampere}$. Über $R_1$ fällt die Differenz der Betriebsspannung ($\qty{10}{\volt}$) und dem Basispotential ab, also $\qty{8,4}{\volt}$. Nun können wir $R_1$ bestimmen:

$R_1 = \frac{\qty{8,4}{\volt}}{\qty{110}{\micro\ampere}} = \qty{76,4}{\kilo\ohm}$

Dies ist eine gute Schaltung, weil der Kollektorstrom vor allem durch den Emitterwiderstand $R_E$ festgelegt wird, der eine Serien-Gegenkopplung darstellt.

[question:AC519]

Wenn $R_1$ durch den Fehler nicht von Strom durchflossen, so fällt an $R_2$ keine Spannung ab -- die Basis liegt auf Massepotential. Dann ist $U_{BE} \geq \qty{0,6}{\volt}$ nicht erfüllt, und der Transistor ist stromlos. Da am Kollektorwiderstand $R_C$ keine Spannung abfällt, steigt das Kollektorpotential auf die Betriebsspannung an.

[question:AC520]

Bei dem hier gegebenen Fehlerbild ist $R_2$ stromlos. Die Basis ist über $R_1$ mit der Betriebsspannung verbunden. Über diesen Pfad wird ein Basisstrom injiziert. Bei der üblichen Dimensionierung (Querstrom ist der zehnfache reguläre Basisstrom) ist der Basisstrom 11-fach höher als der reguläre Basisstrom -- der Kollektorstrom wird sehr stark ansteigen, der Spannungsabfall an $R_C$ steigt stark an, die Kollektor-Emitter-Spannung sinkt auf den Sättigungswert von etwa $\qty{0,1}{\volt}$ ab. Der Kollektorstrom wird nur durch $R_C$ begrenzt.

[question:AC521]

In den Gate-Anschluss eines MOSFETs fließt kein Gleichstrom. Daher handelt es sich im einen *unbelasteten* Spannungsteiler und es gilt:

$U_{GS} = \frac{R_2}{R_1 + R_2} \cdot U_B = \frac{\qty{1}{\kilo\ohm}}{\qty{11}{\kilo\ohm}} \cdot \qty{44}{\volt} = \qty{4}{\volt}$

[question:AC522]

Auch hier handelt es sich um einen unbelasteten Spannungsteiler. Da die Spannungen gegeben sind, setzen wir am einfachsten an:

$\frac{R2}{R_1} = \frac{\qty{2,8}{\volt}}{\qty{44}{\volt} - \qty{2,8}{\volt}} \rightarrow R_2 = 0,068 \cdot \qty{10}{\kilo\ohm} = \qty{680}{\ohm}$

[question:AC523]

Der Leistungs-MOSFET ist hier vollständig durchgeschaltet, der Kanal lässt sich als ein ohmscher Widerstand von (lt. Aufgabenstellung) $R_{ch} = \qty{4}{\milli\ohm}$ darstellen. Es fließt ein Strom von $\qty{25}{\ampere}$. Die Verlustleistung berechnen wir nach der Formel

$P_V = I^2 \cdot R_{ch} = \qty{2,5}{\watt}$

[question:AC524]

In dieser Aufgabe geht es um ein Relais, das über den in Serie dargestellten npn-Transistor geschaltet wird. Nehmen wir an, dass der Transistor zunächst durchgeschaltet ist, es fließt ein Strom durch die Relaisspule, das Relais hat angezogen.

Nun schaltet der Transistor ab, der Stromfluss bricht zusammen. Die starke Änderung des Stroms induziert allerdings kurzzeitig in der Spule des Relais eine hohe negative Spannung, die zur Zerstörung des Transistors führen kann.

Um dies zu verhindern, schalten wir eine Freilaufdiode *parallel*. Sie ist so geschaltet, dass sie im Regelbetrieb (Transistor durchgeschaltet) keinen Strom führt -- sie muss also in Sperrrichtung eingebaut werden. Die negative Spannung, die beim Zusammenbruch des Stroms kurzzeitig auftritt, schaltet die Diode in Flussrichtung, die enstehende Spannung wird (bei Siliziumdioden) auf $\qty{-0,7}{\volt} \ldots \qty{-0,8}{\volt}$ begrenzt.
