## Ausgangslage: ASK und PSK

* Bei ASK und PSK können mehr Symbole verwendet werden, um mehr Bits pro Symbol zu übertragen
* Bei sehr vielen Symbolen liegen die möglichen Signalzustände jedoch immer dichter beieinander
* Der Empfänger muss dadurch kleinere Unterschiede erkennen können
* Das Verfahren wird anfälliger für Störungen

<note>
Es scheint zunächst nahezuliegen, einfach immer mehr Amplituden oder Phasenlagen zu verwenden. Dadurch können zwar mehr Bits pro Symbol übertragen werden, gleichzeitig wird es für den Empfänger aber schwieriger, die einzelnen Symbole sicher voneinander zu unterscheiden.
</note>

---

## Quadraturamplitudenmodulation (QAM)

* Trick: Es wird nicht nur *ein* Parameter verändert
* QAM kombiniert unterschiedliche
  * Amplituden und
  * Phasenlagen
* Ein Symbol entspricht einer bestimmten Kombination aus Amplitude und Phase

<fragment>
Bei gleicher Symbolrate können dadurch mehr Bits pro Sekunde übertragen werden.
</fragment>

<note>
Anstatt beispielsweise bei ASK sehr viele unterschiedliche Amplituden unterscheiden zu müssen, nutzt QAM zwei Freiheitsgrade gleichzeitig: Amplitude und Phase.

Dadurch kann bereits mit einer vergleichsweise kleinen Anzahl unterschiedlicher Werte eine größere Zahl verschiedener Symbole erzeugt werden.
</note>

--- style="font-size: 0.7em;"
## Beispiel: 8-QAM

[picture:702:a_8qam:Signalverlauf eines 8QAM-Signals, je Symbol mit Amplitude ($\num{0,5}$ bzw. $\num{1}$), Phasenlage und 3-stelliger Bitfolge]

* $\num{8}$ verschiedene Symbole
* Jedes Symbol besitzt eine bestimmte Amplitude und Phasenlage
* $\num{8}$ Symbole → $\num{3}$ Bits pro Symbol

<note>
Die Abbildung zeigt ein 8-QAM-Signal im Zeitbereich.

Jedem Symbol ist durch das Mapping eine dreistellige Bitfolge zugeordnet. Da acht unterschiedliche Symbole existieren, können mit jedem Symbol drei Bits übertragen werden.
</note>

---
## Beispiel: 16-QAM

<left>
[picture:1061:a_16qam:I-Q-Diagramm für ein 16-QAM-Mapping]
</left>
<right>
* $\num{16}$ verschiedene Signalpunkte
* Jeder Punkt entspricht einem Wertepaar $(I,Q)$
* Daraus ergeben sich unterschiedliche Amplituden und Phasenlagen
* $\num{16}$ Symbole → $\num{4}$ Bits pro Symbol
</right>

<note>
Im Konstellationsdiagramm lässt sich besonders gut erkennen, wie QAM viele unterschiedliche Symbole erzeugt.

Bei 16-QAM gibt es 16 mögliche Signalpunkte. Jedem Punkt wird eine vierstellige Bitkombination zugeordnet.

Die Lage eines Punktes wird durch die beiden Werte I und Q beschrieben. Daraus ergeben sich wiederum die Amplitude und die Phasenlage des resultierenden Signals.
</note>

---
[question:AE403]

---
## Wie wird ein QAM-Signal erzeugt?

Nachdem wir das Konstellationsdiagramm kennengelernt haben, stellt sich die Frage:

<fragment>
**Wie erzeugt ein Sender einen gewünschten Signalpunkt?**
</fragment>

<fragment>
Dazu kann ein *I/Q-Modulator* verwendet werden.
</fragment>

---
## I/Q-Modulator

<left>
[picture:196:a_iq_modulator:Blockschaltbild eines I/Q-Modulators]
</left>
<right>
* Zwei Träger mit gleicher Frequenz
* Phasenverschiebung von $\qty{90}{\degree}$
* Ein Träger wird mit dem *I-Signal* gewichtet
* Der andere Träger wird mit dem *Q-Signal* gewichtet
* Anschließend werden beide Signale addiert
</right>

<note>
Ein I/Q-Modulator arbeitet mit zwei sinusförmigen Trägern gleicher Frequenz. Die beiden Träger sind um 90 Grad gegeneinander phasenverschoben.

Der erste wird mit dem I-Wert und der zweite mit dem Q-Wert gewichtet. Anschließend werden beide Signalanteile addiert.

Je nach Kombination von I und Q entsteht dadurch ein Signal mit einer bestimmten Amplitude und Phasenlage.
</note>

---
## I und Q bestimmen Amplitude und Phase

* Jeder Signalpunkt im Konstellationsdiagramm entspricht einem Wertepaar $(I,Q)$
* Durch Änderung von I und Q ändern sich
  * die Amplitude und
  * die Phasenlage
  des resultierenden Signals

<fragment>
Damit kann der I/Q-Modulator jeden gewünschten Punkt des Mappings erzeugen.
</fragment>

<note>
Das ist die direkte Verbindung zwischen dem Konstellationsdiagramm und der realen Schaltung:

Die Koordinaten eines Signalpunktes sind genau die Werte I und Q, mit denen der I/Q-Modulator angesteuert wird.

Das Konstellationsdiagramm ist damit nicht nur eine Darstellung des Signals. Es beschreibt unmittelbar, welche I- und Q-Werte erzeugt werden müssen.
</note>

--- style="font-size: smaller;"

## I/Q-Modulation ausprobieren

[include:applet_iq_169]

<note>
Mit dem Applet kann die Wirkung der beiden Werte I und Q unmittelbar ausprobiert werden.

Werden I und Q verändert, verschiebt sich der Signalpunkt im Konstellationsdiagramm. Gleichzeitig kann beobachtet werden, wie sich dadurch Amplitude und Phase des resultierenden Signals verändern.

Damit lässt sich auch nachvollziehen, wie ein I/Q-Modulator die unterschiedlichen Punkte eines QAM-Mappings erzeugen kann.
</note>

---

[question:AF632]

---

[question:AE404]

---

## I und Q aus Software

* Ein Mikrocontroller, Signalprozessor oder SDR berechnet die Werte für I und Q
* Für jedes Symbol wird das entsprechende Wertepaar $(I,Q)$ bestimmt

<fragment>
Beispiel 16-QAM:

* $\num{4}$ mögliche I-Werte
* $\num{4}$ mögliche Q-Werte
* $\num{4}\cdot\num{4}=\num{16}$ mögliche Signalpunkte
</fragment>

<note>
Die I- und Q-Werte müssen nicht durch eine komplizierte analoge Schaltung erzeugt werden.

In einem digitalen System kann die Software für jedes zu übertragende Symbol einfach die beiden dazugehörigen Zahlenwerte bestimmen.

Bei einer 16-QAM können beispielsweise jeweils vier unterschiedliche Werte für I und Q verwendet werden. Aus den Kombinationen ergeben sich insgesamt 16 Signalpunkte.
</note>

---

## Vom Zahlenwert zum I/Q-Signal

* I und Q liegen zunächst als *digitale Zahlenwerte* vor
* DA-Wandler erzeugen daraus analoge I- und Q-Signale
* Diese Signale steuern den I/Q-Modulator

<fragment>
Das gewünschte Mapping kann damit zu einem großen Teil in *Software* festgelegt werden.
</fragment>

<note>
Die Software erzeugt zunächst digitale Zahlenwerte für I und Q.

DA-Wandler setzen diese anschließend in analoge Spannungen um, die dem I/Q-Modulator zugeführt werden können.

Vereinfacht betrachtet muss die Software also nur berechnen, welcher Punkt des Konstellationsdiagramms gerade erzeugt werden soll.
</note>

---

## Software Defined Radio

* Bei einem *Software Defined Radio (SDR)* wird ein großer Teil der Signalverarbeitung in Software ausgeführt
* Die Software berechnet die benötigten I- und Q-Signale
* Die Hochfrequenzhardware kann für viele unterschiedliche Modulationsverfahren gleich bleiben

<fragment>
Das Modulationsverfahren wird damit zu einem großen Teil durch *Software* bestimmt.
</fragment>

---

## Nicht nur digitale Modulation

Ein I/Q-Modulator kann auch kontinuierlich veränderliche I- und Q-Signale verarbeiten.

<fragment>
Damit lassen sich beispielsweise erzeugen:

* AM
* FM
* PM
* SSB
* PSK
* QAM
</fragment>

<note>
Das I/Q-Prinzip ist keineswegs auf QAM oder andere digitale Modulationsverfahren beschränkt.

Die Software kann anstelle einzelner fester Symbolwerte auch kontinuierlich veränderliche Verläufe für I und Q erzeugen.

Bei AM wird beispielsweise hauptsächlich der Betrag des Signalzeigers verändert. Bei PM wird sein Winkel verändert.

Auch FM kann über die Phase erzeugt werden: Die Phase wird kontinuierlich verändert, wobei die Geschwindigkeit der Phasenänderung der momentanen Frequenz entspricht.

Mit geeigneten I- und Q-Signalen lässt sich außerdem ein Einseitenbandsignal erzeugen.
</note>

---

## Nicht nur digitale Modulation

* Derselbe I/Q-Modulator kann viele unterschiedliche Modulationsverfahren erzeugen
* Lediglich die Verläufe von *I* und *Q* müssen anders berechnet werden
* Die HF-Hardware kann weitgehend unverändert bleiben

<fragment>
Der I/Q-Modulator ist damit gewissermaßen das  
**„Schweizer Taschenmesser der Modulatoren“**.
</fragment>

<note>
Genau diese Eigenschaft macht moderne SDR-Technik so flexibel.

Anstatt für AM, FM, SSB, PSK oder QAM jeweils eine eigene Modulatorschaltung zu benötigen, kann dieselbe grundlegende I/Q-Hardware verwendet werden.

Das gewünschte Verfahren entsteht dadurch, dass die Software andere I- und Q-Signale berechnet.
</note>
