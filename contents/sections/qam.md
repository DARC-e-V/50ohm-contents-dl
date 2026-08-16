Bisher haben wir ASK und PSK kennengelernt. Es scheint für beide Verfahren zunächst nahezuliegen, die Anzahl der Symbole möglichst groß zu wählen, damit pro Symbol möglichst viele Informationen übertragen werden können. Doch dann muss ein Empfänger z. B. zwischen vielen unterschiedlichen Amplituden unterscheiden können. Somit wird das Verfahren anfälliger für Störungen.

Um dieses Problem zu mildern, kann man auf einen Trick zurückgreifen: Anstelle der Änderung nur eines Parameters (z. B. der Amplitude) werden pro Symbol zwei Parameter verändert, nämlich die Amplitude und die Phase. Ein Symbol entspricht dann einer Kombination einer bestimmten Amplitude mit einer bestimmten Phasenlage. So ergibt sich trotz kleiner Anzahl unterschiedlicher Amplituden und Phasenlagen dennoch eine größere Anzahl an Symbolen. Bei gleicher Symbolrate können somit mehr Bits pro Sekunde übertragen werden. Dieses Verfahren wird *Quadraturamplitudenmodulation* (QAM) genannt.

Die Abbildung [ref:a_8qam] zeigt ein 8-QAM-Signal im zeitlichen Verlauf. Jedes Symbol besitzt eine bestimmte Amplitude, eine bestimmte Phasenlage und eine 3-stellige Bitfolge, die durch das Mapping festgelegt ist. Mit jedem Symbol können somit drei Bits übertragen werden. Die Abbildung [ref:a_16qam] zeigt ein 16-QAM-Mapping im Konstellationsdiagramm. Jedes Symbol entspricht einer Kombination aus einer bestimmten Amplitude und einer bestimmten Phasenlage. Mit jedem Symbol können somit vier Bits übertragen werden.

<margin>
[picture:702:a_8qam:Signalverlauf eines 8QAM-Signals, je Symbol mit Amplitude ($\num{0,5}$ bzw. $\num{1}$), Phasenlage und 3-stelliger Bitfolge]
[picture:1061:a_16qam:I-Q-Diagramm für ein 16-QAM-Mapping]
</margin>

[question:AE403]

---

Nachdem wir die I/Q-Darstellung, das Konstellationsdiagramm und die Quadraturamplitudenmodulation kennengelernt haben, stellt sich die Frage, wie ein solches Signal technisch erzeugt werden kann. Dazu kann ein sogenannter *I/Q-Modulator* verwendet werden.

Ein I/Q-Modulator arbeitet mit zwei Trägern gleicher Frequenz, die um $\qty{90}{\degree}$ gegeneinander phasenverschoben sind. Der erste Träger wird mit dem I-Signal und der um $\qty{90}{\degree}$ phasenverschobene Träger mit dem Q-Signal gewichtet. Abbildung [ref:a_iq_modulator] zeigt das Blockschaltbild eines I/Q-Modulators.

Anschließend werden die beiden modulierten Träger addiert. Je nachdem, welche Werte I und Q besitzen, entsteht dadurch ein Signal mit einer bestimmten Amplitude und Phasenlage. Werden die Werte von I und Q verändert, kann sich somit sowohl die Amplitude als auch die Phase des resultierenden Signals ändern.

<margin>
[picture:196:a_iq_modulator:Blockschaltbild eines I/Q-Modulators]
</margin>

<webonly>
<indepth>
Das Ganze lässt sich leicht mathematisch beschreiben. Für die Summe eines Cosinus-Trägers mit einem anderen, um $\qty{90}{\degree}$ phasenverschobenen Cosinus-Träger gilt folgender Zusammenhang:

$ I(t)\cdot \cos\left(\omega t\right) + Q(t)\cdot \cos\left(\omega t + \qty{90}{\degree}\right)=A \cdot \cos\left(\omega t+\phi\right) $

Es entsteht also ein neues Cosinussignal mit einer Amplitude von

$A=\sqrt{I(t)^2 + Q(t)^2}$ 

und einer Phasenverschiebung von 

$ \phi = \operatorname{atan2}\left(Q(t),I(t)\right)$

[include:applet_iq]
</indepth>
</webonly>

[question:AF632]
[question:AE404]

In einem digitalen System können die Werte für I und Q sehr einfach in Software erzeugt werden. Dazu ordnet beispielsweise ein Mikrocontroller, Signalprozessor oder SDR jedem zu übertragenden Symbol zwei Zahlenwerte für I und Q zu. Ein Signalpunkt im Konstellationsdiagramm entspricht somit unmittelbar einem Wertepaar $(I,Q)$.

Bei einer 16-QAM könnten beispielsweise für I und Q jeweils vier unterschiedliche Werte verwendet werden. Durch ihre Kombination entstehen die $\num{16}$ verschiedenen Signalpunkte. Die Software muss für jedes Symbol lediglich die zum gewünschten Signalpunkt gehörenden I- und Q-Werte ausgeben.

Die zunächst digitalen Zahlenwerte für I und Q können anschließend mit zwei DA-Wandlern in analoge Spannungen umgewandelt und dem I/Q-Modulator zugeführt werden. So lässt sich praktisch jeder gewünschte Punkt im Konstellationsdiagramm durch Software erzeugen. Moderne *Software Defined Radios* (SDR) nutzen genau dieses Prinzip: Ein großer Teil der Modulation wird nicht mehr durch fest verdrahtete analoge Schaltungen festgelegt, sondern durch die Berechnung der I- und Q-Signale in Software.

---

Ein I/Q-Modulator ist dabei keineswegs auf digitale Modulationsverfahren wie QPSK oder QAM beschränkt. Anstelle einzelner fester I- und Q-Werte kann die Software auch kontinuierlich veränderliche Signalverläufe für I und Q berechnen. Damit lassen sich auch analoge Modulationsverfahren erzeugen.

Bei einer Amplitudenmodulation wird beispielsweise die Länge des resultierenden Signalzeigers verändert. Bei einer Phasenmodulation wird sein Winkel verändert. Auch bei einer Frequenzmodulation wird die Phase des Signalzeigers kontinuierlich verändert, wobei die Geschwindigkeit dieser Phasenänderung die momentane Frequenz bestimmt. Mit zwei passend erzeugten I- und Q-Signalen lässt sich außerdem ein Einseitenbandsignal (SSB) erzeugen.

Mit demselben I/Q-Modulator können daher unter anderem AM, FM, PM, SSB, PSK und QAM erzeugt werden. Lediglich die I- und Q-Signale müssen jeweils anders berechnet werden. 

Der I/Q-Modulator ist damit gewissermaßen das "Schweizer Taschenmesser der Modulatoren". Dies ist zugleich ein wesentlicher Grund für die große Flexibilität moderner SDR-Technik: Das verwendete Modulationsverfahren wird zu einem großen Teil durch Software bestimmt, während die Hochfrequenzhardware weitgehend unverändert bleiben kann.
