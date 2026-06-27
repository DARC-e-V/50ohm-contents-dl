In der Klasse E haben wir uns auch schon mit der Spule beschäftigt. Bei Gleichstrom hat die Spule im eingeschwungenen Zustand einen sehr kleinen Widerstand. Die Spule wirkt dann wie ein Stück Draht. Beim Wechselstrom jedoch, zeigt die Spule, ähnlich wie ein Kondensator, einen Wechselstromwiderstand $X_{\textrm{L}}$, das heißt, obwohl der Spulendraht nur einen sehr kleinen ohmschen Widerstand (Leiterwiderstand) besitzt, fließt ein Strom, der aber mit steigender Frequenz der Wechselspannung kleiner wird:

$|X_{L}| = \omega \cdot L = 2\cdot\pi\cdot f \cdot L$

Aus der Formel lässt sich erkennen, dass der Wechselstromwiderstand mit zunehmender Frequenz ansteigt und mit abnehmender Frequenz sinkt. Im gegensatz zum Kondensator ist der Wechelstromwiderstand einer Spule positiv. 

<indepth>
Warum ist der induktive Blindwiderstand positiv? Der Hintergrund liegt wieder in der komplexen Wechselstromrechnung, die für die Amateurfunkprüfung nicht zwingend erforderlich ist.

Für Leserinnen und Leser mit Kenntnissen in komplexen Zahlen sei jedoch angemerkt, dass die korrekte Darstellung des induktiven Blindwiderstands eigentlich

$X_L = j\omega L$

lautet. Dabei steht $j$ wieder für die imaginäre Einheit $\sqrt{-1}$.

Daraus wird ersichtlich, dass der induktive Blindwiderstand nicht nur positiv, sondern auch komplex ist. Das positive Vorzeichen beschreibt dabei die Phasenlage zwischen Strom und Spannung an der Spule welche wir in diesem Kapitel noch genauer betrachten.
</indepth>

[question:AC202]

[question:AC203]

---

Mit einem vektoriellen Network Analyzer (VNA) lässt sich die Veränderung des induktiven Blindwiderstandes $X_L$ in Abhängigkeit von der Frequenz darstellen (vgl. Abbildung [ref:a_XL_Verlauf]). 

<margin>
[photo:265:a_XL_Verlauf:Veränderung des induktiven Blindwiderstandes $X_L$ einer Spule von $\qty{500}{\kilo\hertz}$ bis $\qty{10}{\mega\hertz}$]
</margin>

Versuche nun die folgende Frage durch die obige Formel zu beantworten. Achte dabei besonders auf die Einheiten bzw. die Zehnerpotenzen, damit du die richtigen Ergebnisse erhältst.

[question:AC204]

---

Ähnlich wie beim Kondensator tritt auch bei der Spule eine Phasenverschiebung zwischen Spannung und Strom auf. Diese beträgt $\qty{+90}{\degree}$, wobei der Strom der Spannung nacheilt, wie in Abbildung [ref:a_Blindleistung_Spule] dargestellt. Die rote Linie in Abbildung [ref:a_XL_Verlauf] zeigt die Phasenlage des induktiven Blindwiderstandes $X_L$ bei ca. $\qty{+90}{\degree}$.

<tip>
Merkhilfe: Bei der Induktivit*äää*t kommt der Strom zu sp*äää*t!
</tip>

[question:AC201]

Daraus ergibt sich eine Leistungskurve, die symmetrisch um die Nulllinie schwankt. Der Mittelwert dieser Leistung ist null, das heißt, es wird – genau wie beim Kondensator – keine Wirkleistung aufgenommen. Stattdessen wird Energie periodisch im Magnetfeld der Spule gespeichert und wieder an die Quelle zurückgegeben.

Man spricht daher bei einer ideal verlustfreien Spule von Blindleistung und einem Blindwiderstand.

<margin>
[picture:944:a_Blindleistung_Spule:Das Produkt von $U \cdot I$ ergibt die grüne Leistungskurve]
</margin>

Sollte eine Spule bei Hochfrequenzanwendungen warm werden, dann besitzt sie Verluste, die diese Erwärmung bewirken. Die Verluste entstehen durch den ohmschen Widerstand des Drahtes und zusätzlich wirkt auch noch der Skin-Effekt, der den Drahtquerschnitt scheinbar verkleinert. Auch hier wird, wie beim Kondensator die Güte $Q$ bzw. der Verlustfaktor $\tan\delta$ zur Beschreibung der Verluste herangezogen.

[question:AC209]

---

Nun haben wir den kapazitiven Blindwiderstand $X_C$ des Kondensators und den induktiven Blindwiderstand $X_L$ der Spule kennengelernt. Beide Größen sind frequenzabhängig und bilden zusammen mit dem ohmschen Widerstand $R$ die sogenannte *Impedanz* $Z$ eines Bauteils.

Die Blindwiderstände $X_L$ und $X_C$ wirken dabei entgegengesetzt und können sich gegenseitig teilweise oder vollständig aufheben. Für die Verrechnung der Blindwiderstände mit dem ohmschen Widerstand ist jedoch keine einfache algebraische Addition möglich, sondern eine geometrische Addition notwendig. Diese erfolgt mithilfe des Satzes des Pythagoras (vgl. Abbildung [ref:a_impedanzdreieck]).

Das Ergebnis ist die Impedanz $Z$, die den komplexen Gesamtwiderstand eines Bauteils beschreibt. Der Betrag der Impedanz $|Z|$ entspricht dem sogenannten Scheinwiderstand:

$Z = \sqrt{R^2 + (X_L - X_C)^2}$ 

oder vereinfacht (vgl. Formelsammlung – Stichwort: Scheinwiderstand):

$Z = \sqrt{R^2 + X^2}$ 

In der Hochfrequenztechnik spielt die Impedanz eine zentrale Rolle, da sie das Verhalten von Bauteilen in Schaltungen bestimmt und insbesondere für die Anpassung von Leitungen, Antennen und Verstärkern entscheidend ist. Sie wird in Ohm ($\unit{\ohm}$) angegeben und beschreibt den Gesamtwiderstand eines Bauteils bei Wechselstrombetrieb. Bei einer Reihenschaltung von Blindwiderstand und Wirkwiderstand ergibt sich ein Scheinwiderstand $Z$, der nur im Betrieb an Wechselspannung auftritt und nicht mit einem Ohm-Meter gemessen werden kann. 

<margin>
[picture:1067:a_impedanzdreieck:Impedanz $Z$ als geometrische Addition von $R$ und $X$]
</margin>

<indepth>
Die Impedanz $Z$ ist eine komplexe Größe, die sowohl den ohmschen Widerstand $R$ als auch die Blindwiderstände $X_L$ und $X_C$ berücksichtigt ($Z = R + j\cdot X$).
</indepth>

[question:AA101]

<tip>
Wirkwiderstand $\qty{100}{\ohm}$ und Blindwiderstand $\qty{100}{\ohm}$ in Reihenschaltung ergeben einen Scheinwiderstand (Impedanz) von $\qty{141}{\ohm}$.
Das Ergebnis entsteht durch geometrische Addition der beiden Widerstände über ein rechtwinkliges Dreieck nach dem den Satz des Pythagoras $a^2 + b^2 = c^2$.
Für die Widerstände bedeutet dies: $R^2 + X_L^2 = Z^2$
$Z = \sqrt{(\qty{100}{\ohm})^2 + (\qty{100}{\ohm})^2} = \qty{141}{\ohm}$
</tip>


---

Die Induktivität einer Spule haben wir auch bereits in der Klasse E kennengelernt. Grundsätzlich steigt die Induktivität wenn die Windungszahl erhöht wird, die Spulenlänge verkürzt wird, die Querschnittsfläche der Spule vergrößert wird und ein magnetisch leitfähigeres Material als Spulenkern verwendet wird. Zur Erhöhung der Induktivität, ohne die Windungszahl drastisch zu steigern, wird die Wicklung auf einen Ferritringkern gewickelt. Drosselspulen mit hoher Induktivität werden zur Verringerung hochfrequenter Ströme eingesetzt.

<indepth>
[photo:270:a_Pulvereisenringkern:Beispiel für einen Pulvereisenringkern]
[photo:271:a_Ferritringkern:Beispiel für einen Ferritkern]
</indepth>

[question:AC211]

Bei Ringkernspulen wird zur Erleichterung der Induktivitätsberechnung ein sogenannter $A_\text{L}$-Wert des Kernmaterials angegeben.
Die Berechnung der Induktivität lautet dann:
$L = N^2 \cdot A_\text{L}$ (siehe Formelsammlung - Stichwort: Induktivität einer Ringkernspule). Versuche nun damit die folgenden Fragen zu beantworten. 

<attention>
Die Benennung des $A_\text{L}$-Wertes ist in Nanohenry pro Windungen im Quadrat angegeben.
</attention>


[question:AC205]
[question:AC206]
[question:AC207]
[question:AC208]

<indepth>
Wenn sich innerhalb der Spule ein magnetisch leitfähiges Material befindet (z.B. Eisen, Ferrit) dann wird das Magnetfeld verstärkt. Die dann wirksame magnetische Flussdichte $B$ lässt sich mit der Formel (siehe Formelsammlung - Stichwort: Magnetische Flussdichte)
$B = \mu_0 \cdot \mu_r \cdot H$
berechnen. Dabei entspricht $\mu_0$ der magnetischen Feldkonstante $\qty{1,2566e-6}{\volt\second\per\ampere\meter}$ und $\mu_r$ steht für die relative Permeabilität des Kernmaterials in der Spule. Für Luft wird der Faktor $1$ eingesetzt (siehe Formelsammlung - Stichwort: Magnetische Feldkonstante; relative Permeabilität).
</indepth>

Zur Abschirmung eines Magnetfeldes benötigt man ein magnetisch gut leitfähiges Material, zum Beispiel Weißblech. Die Abbildung [ref:a_abschirmbecher] zeigt ein Beispiel für Spulen mit Abschirmbecher. Die metallischen Abschirmbecher enthalten Spulen mit einem verstellbaren Ferritkern, der über die Öffnung von oben mit einem Schraubendreher hinein- oder herausgedreht wird. Dadurch ändert sich die Induktivität der Spule.

[question:AC210]

<margin>
[photo:333:a_abschirmbecher:Beispiel für Spulen mit Abschirmbecher zur Abschirmung von magnetischen Feldern]
</margin>
