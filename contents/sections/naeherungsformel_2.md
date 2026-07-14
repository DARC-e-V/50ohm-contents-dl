In der Klasse E haben wir bereits eine Näherungsformel kennengelernt, mit der sich der Sicherheitsabstand zu einer Antenne berechnen lässt:

$d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_{\textrm{EIRP}}}}{E}$

Diese Formel kann für viele Antennenformen angewendet werden, wenn die Bedingung

$d > \frac{\lambda}{2\pi}$

erfüllt ist, wir uns also außerhalb des reaktiven Nahfelds befinden. Im Folgenden betrachten wir, woher diese Einschränkung und der in der Formel auftretende Wert von $\qty{30}{\ohm}$ stammen.

In allgemeiner Form lautet die Näherungsformel:

$d = \frac{\sqrt{\frac{Z_0}{4\pi}\cdot P_{\textrm{EIRP}}}}{E}$

Dabei bezeichnet $Z_0$ den Feldwellenwiderstand des freien Raums. Wie wir im vorherigen Kapitel gesehen haben, nähert sich dieser mit zunehmendem Abstand von der Antenne dem Fernfeldwert

$Z_0 = \qty{120\pi}{\ohm} \approx \qty{377}{\ohm}$

an (vgl. Abbildung [ref:a_feldwellenwiderstand]). Setzen wir diesen Wert in den Ausdruck $\frac{Z_0}{4\pi}$ ein, erhalten wir:

$\frac{Z_0}{4\pi} = \frac{\qty{120\pi}{\ohm}}{4\pi} = \qty{30}{\ohm}$

Damit ergibt sich die aus der Klasse E bekannte Näherungsformel. Gleichzeitig wird deutlich, weshalb sie nicht im reaktiven Nahfeld verwendet werden darf: Dort ist der Feldwellenwiderstand nicht konstant, sondern hängt stark vom Abstand, von der Antennenform und von der betrachteten Richtung ab. Für Berechnungen im reaktiven Nahfeld, also für Abstände $d \le \frac{\lambda}{2\pi}$, sind daher in der Regel ausführlichere Rechnungen, numerische Simulationen, oder Messungen erforderlich. 

<margin>
[picture:1116:a_feldwellenwiderstand:Verlauf des Feldwellenwiderstands über die Bereiche Nahfeld und Fernfeld (Logarithmisch).]
</margin>

Wird die Fernfeld-Näherungsformel bei einer Dipolantenne bereits im strahlenden Nahfeld angewendet, ergibt sich in der Regel ein größerer Sicherheitsabstand als tatsächlich erforderlich. Der Feldwellenwiderstand liegt dort unterhalb von $\qty{377}{\ohm}$, während die Näherungsformel mit dem höheren Fernfeldwert rechnet. Das Ergebnis ist daher konservativ und liegt auf der sicheren Seite. Diese Vorgehensweise wird von der Bundesnetzagentur akzeptiert.

Für magnetische Antennen und elektrisch sehr kurze Antennen gilt dies jedoch nicht. Abbildung [ref:a_feldwellenwiderstand] zeigt beispielsweise, dass der Feldwellenwiderstand einer magnetischen Loop-Antenne im strahlenden Nahfeld deutlich über $\qty{377}{\ohm}$ liegen kann. Die Fernfeld-Näherungsformel würde in diesem Fall einen zu kleinen Sicherheitsabstand ergeben. Deshalb müssen für solche Antennen andere Verfahren eingesetzt werden, beispielsweise spezielle Programme zur Nahfeldberechnung (Simulationen) oder Messungen.

[question:AK103]

Für die Berechnung der Personenschutzabstände kann im Fernfeld die bekannte Näherungsformel verwendet werden. Dadurch lassen sich aufwendige Messungen oder Simulationen häufig vermeiden. Besonders im Portabelbetrieb ermöglicht sie eine schnelle überschlägige Abschätzung des erforderlichen Sicherheitsabstands. 