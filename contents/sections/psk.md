Die Phasenumtastung (Phase Shift Keying, PSK) ist ein digitales Modulationsverfahren, das zur Übertragung von Daten in der Telekommunikation und im Amateurfunk genutzt wird. PSK basiert auf der Veränderung der Phase eines Trägersignals, um verschiedene Datenzustände zu repräsentieren. Im Vergleich zu Amplituden- oder Frequenzmodulation ist PSK weniger anfällig für Amplitudenrauschen und kann bei gleicher Bandbreite eine höhere Datenrate erreichen.

<margin>
[picture:705:psk:Phasenumtastung (Phase-shift Keying)]
</margin>

<margin>
[picture:1101:psk:PSK im Konstellationsdiagramm]
</margin>

---

In der einfachsten Form, dem **BPSK (Binary Phase Shift Keying)**, gibt es zwei Phasenwinkel, z. B. $\qty{0}{\degree}$ und $\qty{180}{\degree}$. Jeder Phasenwinkel repräsentiert einen Bitwert ($\num{0}$ oder $\num{1}$). Bei einem Wechsel der Bitwerte verändert sich die Phase des Trägers um $\qty{180}{\degree}$.

<indepth>
Genaugenommen kann BPSK mit den Winkeln $\qty{0}{\degree}$ und $\qty{180}{\degree}$ auch als ein ASK-Verfahren betrachtet werden, bei dem die Amplitude des Trägersignals zwischen einem negativen und einem positiven Wert umgeschaltet wird. Durch die Symetrie des Sinus-Signals ensteht dann der Phasensprung. Dies ist ein Spezialfall. Es wären übrigens auch andere Phasenwinkel wie z. B. $\qty{90}{\degree}$ und $\qty{270}{\degree}$ möglich, die ebenfalls einen Phasensprung von $\qty{180}{\degree}$ erzeugen würden.
</indepth>

Für höhere Datenraten gibt es Varianten wie **QPSK (Quadrature Phase Shift Keying)** und **8-PSK**, bei denen vier bzw. acht Phasenlagen verwendet werden, um mehrere Bits pro Symbol zu übertragen:
- **QPSK**: Verwendet vier Phasen ($\qty{0}{\degree}$, $\qty{90}{\degree}$, $\qty{180}{\degree}$ und $\qty{270}{\degree}$), um jeweils zwei Bits pro Symbol zu kodieren.
- **8-PSK**: Verwendet acht Phasen, um drei Bits pro Symbol zu kodieren.

Signale in der Zeitdarstellung

In der Zeitdarstellung eines PSK-Signals zeigt sich die Phasenumtastung als abrupter Wechsel im Phasenwinkel des Trägersignals, während die Amplitude konstant bleibt. Dies ist ein deutlicher Unterschied zur Amplituden- oder Frequenzmodulation, da die Höhe und Frequenz des Signals gleichbleiben, nur die Phase ändert sich bei jedem Symbolwechsel.

Beispiel: BPSK in der Zeitdarstellung
- Bei BPSK ist das Signal in zwei Phasen gespalten: z. B. positive Amplitude für eine Phase ($\qty{0}{\degree}$) und negative Amplitude für die entgegengesetzte Phase ($\qty{180}{\degree}$).
- In einem Zeit-Diagramm sieht man daher bei jedem Bitwechsel einen Sprung des Signals, z. B. von positiv nach negativ oder umgekehrt.

Beispiel: QPSK in der Zeitdarstellung
- Hier sieht man vier verschiedene Phasenwinkel. Die Übergänge können ebenfalls abrupt sein, aber die Amplitude ändert sich nicht.
- Da hier mehrere Phasenwinkel verwendet werden, sind die Phasensprünge kleiner, und die Kurve hat einen etwas „geglätteten“ Verlauf im Vergleich zu BPSK.

Wie die Signale zu erkennen sind

In einem Oszilloskop- oder Phasen-Diagramm sind die Phasenübergänge sichtbar:
- **Im Zeitbereich**: Ein abruptes Umkippen der Signalphase (positiv zu negativ oder zwischen verschiedenen Phasenlagen).
- **Im Phasendiagramm** (oft als Constellation Diagram angezeigt): Jeder Phasenwinkel ist als Punkt auf einem Kreis dargestellt, der für die verschiedenen Zustände (Bits) steht. Bei einem sauberen Signal bleiben die Punkte stabil auf festen Positionen.

PSK ist besonders nützlich in der digitalen Kommunikation, da es hohe Datenraten bei vergleichsweise robuster Übertragung erlaubt. Die Veränderung der Phase bei gleichbleibender Amplitude hilft, das Signal auch bei Rauschen und Interferenzen besser zu erkennen und damit eine stabilere Übertragung zu ermöglichen.

[question:AE401]

---

Dieses Prinzip von Symbolen lässt sich auch auf die Phasenumtastung übertragen. Eine einfache Phasenumtastung (Binary Phase-Shift Keying, BPSK) verwendet nur zwei verschiedene Phasenlagen und kann daher nur ein Bit gleichzeitig senden. Die Quadraturphasenumtastung (Quadrature Phase-Shift Keying, QPSK) hingegen nutzt schon vier verschiedene Phasenlagen ($\qty{0}{\degree}$, $\qty{90}{\degree}$, $\qty{180}{\degree}$ und $\qty{270}{\degree}$). QPSK überträgt somit zwei Bits in jedem Schritt.

[question:AE402]

---

Schauen wir uns im ersten Schritt QPSK in Abbildung [ref:a_qpsk] an: Bei QPSK werden jeweils zwei Bits zu einem Symbol zusammengefasst. Da wir zwei Bits pro Symbol haben, ergeben sich vier mögliche Kombinationen ($\num{00}$, $\num{01}$, $\num{10}$, $\num{11}$). Jede dieser Kombinationen wird einem spezifischen Signalpunkt zugeordnet, der durch eine bestimmte Phase repräsentiert wird.

<margin>
[picture:1059:a_qpsk:I-Q-Diagramm für ein QPSK-Mapping]
</margin>

---

Bei QPSK hat jedes Symbol eine eigene Phase. Die Phasen werden typischerweise in $\qty{90}{\degree}$-Schritten definiert und auf die vier möglichen Bitkombinationen gemapped, zum Beispiel:

- $\num{11}$ entspricht $\qty{45}{\degree}$
- $\num{01}$ entspricht $\qty{135}{\degree}$
- $\num{00}$ entspricht $\qty{225}{\degree}$
- $\num{10}$ entspricht $\qty{315}{\degree}$

Die Amplitude der Signale bleibt dabei konstant, und die Information wird ausschließlich durch die Phasenlage übertragen. Deshalb liegen die vier Punkte im Konstellationsdiagramm für QPSK auf einem Kreis. 

<indepth>
Genau genommen gibt es aber auch noch andere Möglichkeiten, die Phasen den Bitkombinationen zuzuordnen, solange sie eindeutig sind. Das hier gezeigte Mapping ist nur ein Beispiel. In dem hier gezeigten Beispiel wurden die Zuordnungen so gewählt, dass sich zwischen benachbarten Symbolen nur wenige Bits ändern. Das hat den Vorteil, dass unter Rauscheinfluss nur wenige Bitfehler entstehen. Dafür wird der Gray-Code verwendet, der in den meisten digitalen Übertragungsverfahren Anwendung findet.
</indepth>

---

Jeder dieser Punkte repräsentiert ein Symbol. Der Empfänger kann anhand der Phasenlage bestimmen, welche Bitkombination gesendet wurde. Das Konstellationsdiagramm bei QPSK zeigt vier Signalpunkte im rechten Winkel zueinander, die den vier verwendeten Phasen entsprechen. Die große Trennung zwischen den einzelnen Phasen ermöglicht eine zuverlässige Decodierung auch unter rauschbehafteten Bedingungen.