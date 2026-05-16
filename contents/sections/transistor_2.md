Den Bipolartransistor hatten wir bereits in den Ausbildungsunterlagen zur Klasse E diskutiert. In der Klasse A werden wir das Thema weiter vertiefen und auch noch einen weiteren Transistor betrachten.

Der Bipolartransistor besteht aus drei Halbleiterzonen, die abwechselnd n- und p-dotiert sind. Die Zonen bezeichnet man als Emitter, Basis und Kollektor. Beim *npn-Transistor* ist der Emitter n-, die Basis p- und der Kollektor n-dotiert. Beim pnp-Transistor ist es entsprechend ein p-Emitter, eine n-Basis und ein p-Kollektor. 

Die Abbildung [ref:a_bipolartransistor_aus] zeigt einen npn-Transistor im ausgeschalteten Zustand.
Sobald die Basis-Emitter-Spannung $U_\mathrm{BE}$ durch Einschalten des Schalters angelegt wird (typisch $\approx \qtyrange{0,6}{0,7}{\volt}$ bei Silizium), wird die Basis-Emitter-Diode leitend. Dadurch fließt ein kleiner Basisstrom $I_\mathrm{B}$ (vgl. Abbildung [ref:a_bipolartransistor_ein]).

Dieser kleine Basisstrom bewirkt, dass aus dem Emitter viele Elektronen in die dünne Basis eingebracht werden. Da die Basis sehr schmal ist, gelangen die meisten dieser Ladungsträger weiter zum Kollektor. Dort werden sie durch die anliegende Kollektor-Emitter-Spannung $U_\mathrm{CE}$ "abgesaugt", der Kollektorstrom $I_\mathrm{C}$ fließt. Er ist um den Faktor $B$ größer als der Basisstrom, wobei $B$ die sogenannte Stromverstärkung des Transistors ist. Typische Werte für $B$ liegen im Bereich von $\num{20}$ bis $\num{500}$.

<margin>
[picture:1071:a_bipolartransistor_aus:NPN Bipolartransistor im augeschaltenen Zustand]
[picture:1072:a_bipolartransistor_ein:NPN Bipolartransistor im eingesschalteten Zustand]
</margin>

[question:AC503]

Es empfiehl sich z.B. den NPN-Transistor zu merken. Bei PNP ist dann alles umgekehrt.

[question:AC504]

Physikalisch steuert die Basis-Emitter-Spannung $U_\text{BE}$ den Kollektorstrom $I_\text{C}$ und zwar exponentiell. Beim npn-Transistor gilt zum Beispiel:

$I_\text{C} = I_\text{S} \cdot e^{\frac{U_\text{BE}}{U_\text{T}}}$

$I_\text{S}$ ist der Sättigungsstrom, der stark von der Bauart des Transistors abhängt. Er ist dem Datenblatt zu entnehmen. $U_\text{T}$ ist die sogenannte Temperaturspannung, die bei Raumtemperatur etwa $\qty{26}{\milli\volt}$ beträgt.

Ein Unterschied zum später betrachteten Feldeffekt-Transistor ist, dass beim Bipolartransistor immer auch ein Strom im Eingang (der Basis) fließt, der Basisstrom $I_\text{B}$. Auch er ist exponentiell von $U_\text{BE}$ abhängig, wobei $I_\text{S}$ um einen Faktor $B$ kleiner ist als beim Kollektorstrom.

$I_\text{B} = \frac{I_\text{S}}{B} \cdot e^{\frac{U_\text{BE}}{U_\text{T}}}$

Der Faktor $B$ ist also der Quotient aus Kollektor- und Basisstrom:

$B = \frac{I_\text{C}}{I_\text{B}}$

Auch wenn der Bipolartransistor physikalisch über $U_\mathrm{BE}$ gesteuert wird, bezeichnet man ihn als *stromgesteuert*, weil er nur dann leitet, wenn ein Basisstrom fließt.

[question:AC501]

Ein Transistor wird als "leitend" in "Durchlassrichtung" bezeichnet, wenn ein signifikanter Kollektorstrom fließt. Dazu muss die Basis-Emitter-Diode stets in Flussrichtung geschaltet sein, also $U_\text{BE}$ positiv bei npn- und negativ bei pnp-Transistoren. Die Kollektor-Basis-Diode dagegen muss sperren, denn es sollen keine Ladungsträger aus dem Kollektor in die Basis injiziert werden.

[question:AC505]

Im Folgenden betrachten wir noch ein paar einfache Transistor-Schaltungen auf Basis des Bipolartransistors.

---

[question:AC515]

Der gewünschte Arbeitspunkt wird dadurch eingestellt, dass über $R_1$ ein Basisstrom eingeprägt wird. Der Basisstrom ist um die gegebene Stromverstärkung von $\num{298}$ kleiner als der Kollektorstrom. Über dem Widerstand fällt die Differenz von Betriebsspannung und Basispotential ab. Das Basispotential ist mit $\qty{0,6}{\volt}$ gegeben. Also rechnen wir:

$R_1 = 298 \cdot \frac{\qty{12}{\volt} - \qty{0,6}{\volt}}{\qty{0,005}{\ampere}} \approx \qty{680}{\kilo\ohm}$

<indepth>
Die Schaltung hat allerdings in der Praxis einen gewaltigen Nachteil: die Stromverstärkung eines Bipolartransistors ist nicht besonders gut kontrolliert. Nehmen wir als Beispiel den populären BC547B. Seine Stromverstärkung kann nach Spezifikation zwischen $\num{200}$ und $\num{450}$ liegen. Der Kollektorstrom kann also mit dieser Schaltung durchaus um mehr als einen Faktor $2$ vom Entwurf abweichen.
</indepth>

Um eine bessere Stabilität des Arbeitspunkts zu erreichen, wird der Arbeitspunkt des Bipolartransistors in der Regel über einen Spannungsteiler eingestellt. Der sogenannte Querstrom ist der Strom, der hier durch $R_2$ fließt. Er sollte mindestens zehnmal so hoch wie der Basisstrom sein, damit der Basisstrom keinen großen Einfluss auf den Arbeitspunkt hat. 

---

[question:AC516]

<indepth>
Auch diese Schaltung ist aus Praxissicht nicht sehr empfehlenswert. Zum einen hängt der Kollektorstrom exponentiell von der Basis-Emitter-Spannung ab. Die Widerstände haben eine Toleranz, durch die das Basispotential durchaus etwas vom Soll abweichen kann - mit einer großen Auswirkung auf den Kollektorstrom. Außerdem ist die Schwellspannung der Basis-Emitter-Diode mit etwa $\qty{-2}{\milli\volt\per\kelvin}$ recht stark temperaturabhängig. Daher wird diese Schaltung einen starken Temperaturgang des Kollektorstroms haben. Das kann manchmal erwünscht sein, aber man muss es im Blick haben. Wir lernen noch eine Schaltung kennen, die eine Gegenkopplung enthält, die den Arbeitspunkt stabilisiert.
</indepth>

Auch zu dieser Schaltung gibt es eine Rechenaufgabe:

[question:AC518]

Der Spannungsteiler $R_1$ und $R_2$ stellt das Basispotential ein, das, weil der Emitter auf Masse liegt, etwa $\qty{0,6}{\volt}$ betragen muss. Bei einem Kollektorstrom von $\qty{2}{\milli\ampere}$ und einer Stromverstärkung von $\num{200}$ ist der Basisstrom $\qty{2}{\milli\ampere} / 200 = \qty{10}{\micro\ampere}$. Der Strom durch $R_2$ soll der zehnfache Basisstrom sein, durch $R_1$ fließt $11 \cdot \qty{10}{\micro\ampere} = \qty{110}{\micro\ampere}$. Der Widerstand $R_1$ ist dann:

$R_1 = \frac{\qty{10}{\volt} - \qty{0,6}{\volt}}{\qty{110}{\micro\ampere}} = \qty{85,5}{\kilo\ohm}$

Die nächste Schaltung zeigt eine typische Arbeitspunkteinstellung für den Bipolartransistor, wie sie auch in der Praxis verwendet wird.

---

[question:AC517]

<indepth>
Dies ist eine gute Schaltung, welche auch in der Praxis häufig verwendet wird, weil der Kollektorstrom vor allem durch den Emitterwiderstand $R_\text{E}$ festgelegt wird, der eine Serien-Gegenkopplung darstellt:

Steigt der Kollektorstrom $I_\text{C}$, so steigt auch der Emitterstrom $I_\text{E}$. Dadurch fällt am Emitterwiderstand $R_\text{E}$ eine größere Spannung ab. Der Emitter wird also positiver. Da die Basisspannung durch den Spannungsteiler aus $R_1$ und $R_2$ nahezu konstant bleibt, wird die Basis-Emitter-Spannung $ U_\text{BE} = U_\text{B} - U_\text{E}$ kleiner.

Eine kleinere Basis-Emitter-Spannung bedeutet, dass der Transistor weniger leitend wird. Der ursprünglich angestiegene Strom wird dadurch wieder reduziert.

Die Schaltung wirkt also Änderungen des Stroms automatisch entgegen. Deshalb spricht man von einer Gegenkopplung. Steigt der Strom, wird der Transistor etwas „zugedreht“. Sinkt der Strom, wird der Transistor wieder stärker leitend. Dadurch stabilisiert sich der Arbeitspunkt der Schaltung.
</indepth>

Das Basispotential wird über den Spannungsteiler $R_1$ und $R_2$ festgelegt. Da über dem Emitterwiderstand $R_\text{E}$ $\qty{1}{\volt}$ abfallen soll, muss das Basispotential $\qty{1,6}{\volt}$ betragen. Bei einem Kollektorstrom von $\qty{2}{\milli\ampere}$ und einer Stromverstärkung von $\num{200}$ beträgt der Basisstrom $\qty{10}{\micro\ampere}$. Da der Strom durch $R_2$ der zehnfache Basisstrom fließen soll, fließt durch $R_1$ der elffache Basisstrom, also $\qty{110}{\micro\ampere}$. Über $R_1$ fällt die Differenz der Betriebsspannung ($\qty{10}{\volt}$) und dem Basispotential ab, also $\qty{8,4}{\volt}$. Nun können wir $R_1$ bestimmen:

$R_1 = \frac{\qty{8,4}{\volt}}{\qty{110}{\micro\ampere}} = \qty{76,4}{\kilo\ohm}$

[question:AC519]

Wenn $R_1$ durch den Fehler nicht von Strom durchflossen, so fällt an $R_2$ keine Spannung ab - die Basis liegt auf Massepotential. Dann ist $U_\text{BE} \geq \qty{0,6}{\volt}$ nicht erfüllt, und der Transistor ist stromlos. Da am Kollektorwiderstand $R_\text{C}$ keine Spannung abfällt, steigt das Kollektorpotential auf die Betriebsspannung an.

[question:AC520]

Bei dem hier gegebenen Fehlerbild ist $R_2$ stromlos. Die Basis ist über $R_1$ mit der Betriebsspannung verbunden. Über diesen Pfad wird ein Basisstrom injiziert. Bei der üblichen Dimensionierung (Querstrom ist der zehnfache reguläre Basisstrom) ist der Basisstrom 11-fach höher als der reguläre Basisstrom - der Kollektorstrom wird sehr stark ansteigen, der Spannungsabfall an $R_\text{C}$ steigt stark an, die Kollektor-Emitter-Spannung sinkt auf den Sättigungswert von etwa $\qty{0,1}{\volt}$ ab. Der Kollektorstrom wird nur durch $R_\text{C}$ begrenzt.

---

In der nächsten Aufgabe geht es um ein Relais, das über den in Serie dargestellten npn-Transistor geschaltet wird (vgl. Abbildung [ref:a_relais_schaltung]). Nehmen wir an, dass der Transistor zunächst durchgeschaltet ist, es fließt ein Strom durch die Relaisspule, das Relais hat angezogen.

<margin>
[picture:426:a_relais_schaltung:Relais-Schaltung mit npn-Transistor und Freilaufdiode]
</margin>

Nun schaltet der Transistor ab, der Stromfluss bricht zusammen. Die starke Änderung des Stroms induziert allerdings kurzzeitig in der Spule des Relais eine hohe negative Spannung, die zur Zerstörung des Transistors führen kann.

Um dies zu verhindern, schalten wir eine Freilaufdiode *parallel*. Sie ist so geschaltet, dass sie im Regelbetrieb (Transistor durchgeschaltet) keinen Strom führt - sie muss also in Sperrrichtung eingebaut werden. Die negative Spannung, die beim Zusammenbruch des Stroms kurzzeitig auftritt, schaltet die Diode in Flussrichtung, die entstehende Spannung wird (bei Siliziumdioden) auf $\qty{-0,7}{\volt} \ldots \qty{-0,8}{\volt}$ begrenzt.

[question:AC524]

---

Feldeffekt-Transistoren haben ein ganz anderes Steuerprinzip als Bipolartransistoren. Während bei Bipolartransistoren sowohl Elektronen also auch Defektelektronen ("Löcher") betrachtet werden müssen (daher "bipolar"), ist beim Feldeffekt-Transistor nur eine Ladungsträgersorte beteiligt ("unipolar"). Dies können entweder Elektronen (*n-Kanal-Feldeffekt-Transistor*) oder Löcher (*p-Kanal-Feldeffekt-Transistor*) sein.

Die Elektroden des FET, welche in Abbildung [ref:a_fet_schnitt_aus] dargestellt sind, werden wie folgt bezeichnet:

* *Source*: dies ist die "Quelle" (engl. source) für die Ladungsträger im Kanal. Nicht verwirren lassen: die sogenannte technische Stromrichtung ist entgegen der Ladungsträger-Flussrichtung definiert!
* *Drain*: dies ist der Abfluss (engl. drain) für die Ladungsträger im Kanal.
* *Gate*: Das Gate (englisch für Gatter) steuert den Fluss der Ladungsträger im Kanal.

[question:AC512]

Allen Feldeffekt-Transistoren (oder *FETs*) gemein ist, dass im normalen Betrieb kein Strom im Eingang, der Gate-Elektrode, fließt. Die Steuerung der Ladung im Kanal (dem Bereich zwischen *Source* und *Drain*) ist ausschließlich von der Gate-Source-Spannung abhängig.

<margin>
[picture:1073:a_fet_schnitt_aus:FET im Querschnitt, nicht leitend]
[picture:1074:a_fet_schnitt_ein:FET im Querschnitt, leitend]
</margin>

Die Abbildungen [ref:a_fet_schnitt_aus] und [ref:a_fet_schnitt_ein] zeigen den Querschnitt eines n-Kanal-MOSFETs im gesperrten und im leitenden Zustand. Im oberen Bild ist keine ausreichende Gate-Source-Spannung $U_{GS}$ angelegt. Zwischen den n-dotierten Bereichen von Source und Drain befindet sich das p-dotierte Substrat, sodass kein leitfähiger Kanal vorhanden ist. Der Transistor sperrt, und zwischen Source und Drain kann kein Strom fließen.

Wird am Gate eine positive Spannung gegenüber Source angelegt (vgl. Abbildung [ref:a_fet_schnitt_ein]), entsteht durch die isolierende SiO$_2$-Schicht hindurch ein elektrisches Feld. Dieses Feld zieht Elektronen an die Oberfläche des p-dotierten Substrats direkt unterhalb des Gates. Dadurch bildet sich dort ein leitfähiger n-Kanal, der Source und Drain miteinander verbindet. Der MOSFET wird leitend, und es kann ein Strom zwischen Drain und Source fließen.

Wichtig ist dabei, dass das Gate durch die Oxidschicht elektrisch isoliert ist. Im Idealfall fließt daher kein Gate-Strom; der MOSFET wird nicht durch einen Steuerstrom, sondern durch das elektrische Feld am Gate gesteuert. Deshalb wird er auch als *spannungsgesteuertes* Bauelement bezeichnet.

[question:AC502]

[question:AC513]

[question:AC514]

Wie wir bereits festgestellt hatten, ist der FET ein *spannungsgesteuertes* Bauelement, in dem kein Gate-Strom fließt. Die gewünschte Antwort ist die, dass die Gate-Source-Spannung den *Kanalwiderstand* steuert. Allerdings kann das Verhalten des Kanals nur für sehr kleine Drain-Source-Spannungen als Widerstand beschrieben werden, in sofern ist die Antwort etwas unglücklich formuliert. Besser wäre: die Gate-Source-Spannung steuert den Kanalstrom.

---

Die senkrechte Linie symbolisiert den Kanal, die oben (Drain) und unten (Source) kontaktiert wird. Links ist das Gate zu sehen - der Pfeil erinnert zusammen mit dem senkrechten Strich an eine Diode. Es handelt sich also um einen FET, genau genommen einen Sperrschicht-FET. Die Abbildung [ref:a_fet_overview] zeigt eine Übersicht über die verschiedenen FET-Typen mit ihren Schaltsymbolen.

<margin>
[picture:1075:a_fet_overview:FET-Übersicht mit Symbolen]
</margin>

[question:AC506]

Bei den folgenden Fragen geht es darum, bestimmte FET-Typen ihrem Schaltsymbol zuzuordnen. Dazu ein paar Grundregeln:

* Der Strom im Kanal kann entweder von Elektronen oder von Löchern getragen werden. Wir sprechen im ersten Fall von einem *n-Kanal-FET*, im zweiten Fall von einem *p-Kanal-FET*.
* Wir können FETs auch danach unterscheiden, ob für eine Gate-Source-Spannung $U_{GS}=0$ ein Strom im Kanal fließt oder nicht. Sie heißen dann entweder *selbstleitend* oder *selbstsperrend*. 
* Schließlich können wir FETs danach unterscheiden, ob die Gate-Elektrode eine Diode ist, oder eine Kondensator-Struktur. Ist Gate eine Diode, sprechen wir von einem Sperrschicht-FET. Beispiele sind der JFET (junction field effect transistor) und der MESFET (metal semiconductor field effect transistor). Beim MESFET ist die Gate-Diode eine Schottky-Diode. Bei einem *Isolierschicht-FET* ist die Gate-Elektrode durch einen Isolator (ein Dielektrikum) vom Kanal getrennt. Die anliegende Spannung steuert die Dichte von Ladungsträgern im Kanal. Ist der Isolator ein Oxid, zum Beispiel Siliziumdioxid, sprechen wir auch von einem MOSFET (metal oxide semiconductor FET). Wegen ihrer Verwendung in Digitalschaltkreisen sind MOSFETs mit sehr weitem Abstand die häufigsten Transistortypen.

Der Pfeil zeigt an, ob es sich um einen n- oder p-Kanal-FET handelt. Wie bei der Diode zeigt der Pfeil auf die Kathode, also den n-dotierten Bereich. Zeigt also der Pfeil auf den Kanal, handelt es sich um einen n-Kanal-FET. Beim Sperrschicht-FET trägt das Gate den Kanal, beim Isolierschicht-FET ist der Pfeil zwischen Kanal und der sogenannten Bulk-Schicht zu sehen, die unter dem Kanal liegt und meist intern mit der Source-Elektrode verbunden ist.

Im Isolierschicht-FET bilden Gate und Kanal auch grafisch einen Kondensator.

Beim selbstleitenden FET geht die Linie zwischen Source und Drain durch, während sie beim selbstsperrenden FET unterbrochen ist.

[question:AC507]
[question:AC508]
[question:AC509]
[question:AC510]
[question:AC511]

Im folgenden wollen wir auch ein paar MOSFET-Schaltungen betrachten, die auf den vorherigen Fragen aufbauen.

[question:AC521]

In den Gate-Anschluss eines MOSFETs fließt kein Gleichstrom. Daher handelt es sich im einen *unbelasteten* Spannungsteiler und es gilt:

$U_\text{GS} = \frac{R_2}{R_1 + R_2} \cdot U_\text{B} = \frac{\qty{1}{\kilo\ohm}}{\qty{11}{\kilo\ohm}} \cdot \qty{44}{\volt} = \qty{4}{\volt}$

[question:AC522]

Auch hier handelt es sich um einen unbelasteten Spannungsteiler. Da die Spannungen gegeben sind, setzen wir am einfachsten an:

$\frac{R_2}{R_1} = \frac{\qty{2,8}{\volt}}{\qty{44}{\volt} - \qty{2,8}{\volt}} \rightarrow R_2 = 0,068 \cdot \qty{10}{\kilo\ohm} = \qty{680}{\ohm}$

[question:AC523]

Der Leistungs-MOSFET ist hier vollständig durchgeschaltet, der Kanal lässt sich als ein ohmscher Widerstand von (lt. Aufgabenstellung) $R_\mathrm{DSon} = \qty{4}{\milli\ohm}$ darstellen. Es fließt ein Strom von $\qty{25}{\ampere}$. Die Verlustleistung berechnen wir einfach nach der bekannten Leistungs-Formel:

$P_\text{V} = I^2 \cdot R_{\mathrm{DSon}} = \qty{2,5}{\watt}$
