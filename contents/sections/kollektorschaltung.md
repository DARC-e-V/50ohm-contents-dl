In den nächsten beiden Kapiteln beschäftigen wir uns mit zwei wichtigen Grundschaltungen eines bipolaren Transistors. Zunächst betrachten wir in diesem Kapitel die *Kollektorschaltung*, im darauffolgenden Kapitel die *Emitterschaltung*. Beide Schaltungen sind in Abbildung [ref:a_emitter_collector] dargestellt. Sie besitzen unterschiedliche Eigenschaften und werden daher für verschiedene Anwendungen eingesetzt.

<margin>
[picture:1118:a_emitter_collector:Emitter- und Kollektorschaltung mit Bezeichnugnen Basis (B), Kollektor (C) und Emitter (E)]
</margin>

Die Bezeichnung der Grundschaltungen eines bipolaren Transistors richtet sich nach dem Anschluss, der weder als Eingang noch als Ausgang der Schaltung dient und damit den gemeinsamen Bezugspunkt für den Eingangs- und den Ausgangskreis bildet. Bei der Kollektorschaltung ist dies der Kollektor. 

---

[question:AD401]

<tip>
Verstärkerschaltungen von Bipolartransistoren werden nach dem Anschluss benannt, an dem weder Eingang noch Ausgang direkt angeschlossen sind (vgl. Abbildung [ref:a_emitter_collector]). 
</tip>

Da der Kollektor üblicherweise mit der Versorgungsspannung verbunden ist und für Wechselspannungen näherungsweise auf einem festen Potenzial liegt, folgt die Spannung am Emitter der Spannung an der Basis. Die Kollektorschaltung wird daher auch oft als *Emitterfolger* bezeichnet.

Steigt die Eingangsspannung beispielsweise während einer positiven Halbwelle an, erhöht sich der Emitterstrom. Dadurch nimmt der Spannungsabfall am Emitterwiderstand zu und auch die Ausgangsspannung steigt. Ein- und Ausgangssignal sind daher phasengleich; die Phasenverschiebung beträgt $\qty{0}{\degree}$. Aus diesem Grund wird die Kollektorschaltung auch als *Emitterfolger* bezeichnet.

[question:AD405]

---

Die Abbildung [ref:a_collector_circuit] zeigt eine einfache Kollektorschaltung mit Spannungsversorgung, Emitterwiderstand und Koppelkondensatoren. 

<margin>
[picture:140:a_collector_circuit:Kollektorschaltung mit Spannungsversorgung, Emitterwiderstand und Koppelkondensatoren]
</margin>

Für den Betrieb als linearer Strom-Verstärker benötigt der Transistor in der Kollektorschaltung einen definierten Arbeitspunkt (BIAS), der normalerweise durch einen Spannungsteiler an der Basis festgelegt wird.

Der Emitterwiderstand wandelt den Strom, der durch die Kollektor-Emitter-Strecke fließt, in einen Spannungsabfall um, der am Emitter abgegriffen wird. Der Emitterstrom des Transistors fließt (gemeinsam mit dem normalerweise vernachlässigbaren Basis-Strom-Anteil) über den Emitter durch den Emitterwiderstand gegen Masse. Der Strom durch den Emitterwiderstand verursacht durch den entstehenden Spannungsabfall an diesem eine Erhöhung des Emitterpotenzials (Emitterspannung) und wirkt somit als Gegenkopplung für die Basis-Spannung. Hierdurch wird der Arbeitspunkt des Transistors zusätzlich stabilisiert, weil thermisch bedingte Änderungen des Kollektorstroms hierdurch ausgeregelt werden.

Die Ein- und Auskopplung der Signale an Basis und Emitter erfolgt über sog. Koppelkondensatoren. Diese haben die Aufgabe, Gleichspannungsanteile von der Verstärkerstufe, die zu einer Veränderung des Arbeitspunktes führen würden, fernzuhalten.

Der Abblockkondensator in der Betriebsspannung (+) dient der Abführung von unerwünschten HF- und NF-Signalen, damit Rückkopplungseffekte auf die Stufe und die Versorgungsspannung vermieden werden. Zudem wird der Kollektor durch den Abblockkondensator signalmäßig (für Wechselspannung) auf Ein- und Ausgang gelegt.

Die Spannungsverstärkung der Kollektorschaltung bewegt sich bei entsprechender Auslegung im Bereich von $\num{0,9}$ bis $\num{0,98}$ und ist immer etwas kleiner als $1$. 

Man könnte sich nun fragen, welchen Nutzen ein Verstärker mit einer Spannungsverstärkung kleiner als $1$ hat. Die Kollektorschaltung besitzt jedoch einen entscheidenden Vorteil, den wir im Folgenden betrachten. 

[question:AD402]

Die Kollektorschaltung besitzt eine deutliche Stromverstärkung. Ihre Eingangsimpedanz ist relativ hoch, weil nur ein kleiner Strom in die Basis fließen kann. Die Ausgangsimpedanz ist hingegen relativ niedrig. Wird die Ausgangsspannung durch eine angeschlossene Last verändert, ändert sich dadurch die Basis-Emitter-Spannung und der Transistor regelt seinen Emitterstrom so nach, dass er dieser Änderung entgegenwirkt. Durch diese Gegenkopplung kann die Kollektorschaltung eine niederohmige Last treiben, ohne dass sich ihre Ausgangsspannung stark verändert.

[question:AD403]

Aus diesem Grund wird die Kollektorschaltung häufig als *Pufferstufe zwischen Oszillator und weiteren Schaltungsteilen*, die den Oszillator ansonsten niederohmig belasten würden, verwendet, um eine Entkopplung und bessere Frequenzstabilisierung des Oszillators zu erreichen.

[question:AD404]