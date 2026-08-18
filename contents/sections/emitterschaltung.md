Im vorherigen Kapitel haben wir die Kollektorschaltung eines bipolaren Transistors kennengelernt. In diesem Kapitel betrachten wir die *Emitterschaltung*.

<margin>
[picture:1118:a_emitter_collector:Emitter- und Kollektorschaltung mit Bezeichnugnen Basis (B), Kollektor (C) und Emitter (E)]

Fassen wir kurz die Eigenschaften der Kollektor und Emitterschaltung in folgender Tabelle zuammen: 

| l: Eigenschaft | X: Emitterschaltung | X: Kollektorschaltung |
| Phasenverschiebung | $\qty{180}{\degree}$ | $\qty{0}{\degree}$ |
| Spannungsverstärkung | $\num{100}\dots\num{300}$ | $\num{0,9}\dots\num{0,98}$ |
| Eingangsimpedanz | hoch | hoch |
| Ausgangsimpedanz | hoch | niedrig |
</margin>

Wie wir im vorherigen Kapitel gelernt haben richtet sich die Bezeichnung der Grundschaltungen eines bipolaren Transistors nach dem Anschluss, der weder als Eingang noch als Ausgang der Schaltung dient und damit den gemeinsamen Bezugspunkt für den Eingangs- und den Ausgangskreis bildet. Bei der Emitterschaltung ist dies der Emitter. 

---

[question:AD409]

<tip>
Verstärkerschaltungen von Bipolartransistoren werden nach dem Anschluss benannt, an dem weder Eingang noch Ausgang direkt angeschlossen sind (vgl. Abbildung [ref:a_emitter_collector]). 
</tip>

---

Die Abbildung [ref:a_emitterschaltung] zeigt eine einfache Emitterschaltung mit Spannungsversorgung, Kollektorwiderstand und Koppelkondensatoren.

Für den Betrieb als linearer Spannungs-Verstärker benötigt der Transistor in der Emitterschaltung einen definierten Arbeitspunkt (engl. bias, Vorspannung), der normalerweise durch einen Spannungsteiler an der Basis festgelegt wird.

<margin>
[picture:136:a_emitterschaltung:Emitterschaltung]
</margin>

[question:AD411]

Der Kollerktorwiderstand wandelt den Strom, der durch die Kollektor-Emitter-Strecke, fließt in einen Spannungsabfall um, der am Kollektor abgegriffen wird. Der Kollektorstrom des Transistors fließt (gemeinsam mit dem normalerweise vernachlässigbaren Basis-Strom-Anteil) über den Emitter durch den Emitterwiderstand gegen Masse. Der Strom durch den Emitterwiderstand verursacht durch den entstehenden Spannungsabfall an diesem eine Erhöhung des Emitterpotenzials (Emitterspannung) und wirkt somit als Gegenkopplung für die Basis-Spannung. Hierdurch wird der Arbeitspunkt des Transistors zusätzlich stabilisiert, weil thermisch bedingte Änderungen des Kollektorstroms hierdurch ausgeregelt werden.

Die Ein- und Auskopplung der Signale an Basis und Kollektor erfolgt über sog. Koppelkondensatoren. Diese haben die Aufgabe, Gleichspannungsanteile von der Verstärkerstufe, die zu einer Veränderung des Arbeitspunktes führen würden, fernzuhalten.

[question:AD412]

Der Abblockkondensator in der Betriebsspannung (+) dient der Abführung von unerwünschten HF- und NF-Signalen, damit Rückkopplungseffekte auf die Stufe und die Versorgungsspannung vermieden werden.

Die Phasenverschiebung zwischen Ein- und Ausgangssignal beträgt bei der Emitterschaltung $\qty{180}{\degree}$, da bei einer positiven Halbwelle in der Eingangsspannung an der Basis der Kollektorstrom steigt und damit der Spannungsabfall am Kollektorwiderstand zunimmt. Hierdurch sinkt die Spannung am Ausgangskondensator. Es kommt zu einer negativen Halbwelle am Ausgang der Verstärkerstufe.

[question:AD407]
[question:AD408]

Die Spannungsverstärkung der Emitterschaltung bewegt sich bei entsprechender Auslegung im Bereich von $100\dots 300$ und ist damit sehr hoch im Vergleich zur Kollektorschaltung.

[question:AD410]

Der Kondensator am Emitter überbrückt den Emitterwiderstand für Wechselspannungen, wodurch die Gegenkopplung verringert und die Wechselspannungsverstärkung erhöht wird, während der Gleichstrom-Arbeitspunkt unverändert bleibt.

[question:AD413]

Wird jedoch der Emitterkondensator entfernt, so sinkt der Verstärkungsfaktor der Schaltung erheblich (z.B. von $\num{100}$ auf $\num{10}$). Er wird letztlich nur noch durch das Verhältnis von Kollektorwiderstand zu Emitterwiderstand definiert.

[question:AD414]
[question:AD415]

Wird eine Emitterschaltung wie in der folgenden Frage ohne Arbeitspunktvoreinstellung durch einen Spannungsteiler betrieben, so erfolgt die Ansteuerung des Transistors allein durch das zugeführte Eingangssignal. Erst wenn dieses den Wert von ca. $\qty{0,6}{\volt}$ überschreitet, wird die Basis-Emitter-Strecke des Transistors leitend. Hierdurch fließt nur in den Spannungsspitzen ein Kollektorstrom, der einen Spannungsabfall am Ausgang hervorruft. Als Ausgangssignal erscheint die Versorgungsspannung, welche zu den Zeiten, zu denen der Transistor in den leitfähigen Bereich kommt, abfällt. So erklärt sich das entsprechende Ausgangssignal.

[question:AD406]

