Im vorherigen Abschnitt haben wir gesehen, dass die Information in einem Symbol beispielsweise durch unterschiedliche Amplituden oder Frequenzen dargestellt werden kann. Eine weitere Möglichkeit besteht darin, die Phasenlage eines Signals zu verändern. Um Signalzustände mit unterschiedlicher Amplitude und Phase übersichtlich darzustellen, wird häufig die sogenannte *I/Q-Darstellung* verwendet.

Betrachten wir zunächst einen Signalzustand zum Zeitpunkt $t=0$. Für das Symbol werden eine Amplitude $A$ und eine Phasenlage $\varphi$ festgelegt. In einer Zeigerdarstellung bestimmt die Amplitude die Länge des Zeigers und die Phasenlage seinen Winkel gegenüber der waagerechten Achse.

Der Zeiger lässt sich in einen waagerechten und einen senkrechten Anteil zerlegen. Der waagerechte Anteil wird als $I$ für *In-Phase Component* bezeichnet, der senkrechte Anteil als $Q$ für *Quadrature Component*. Für den dargestellten Signalzustand gilt:

$I=A\cdot\cos(\varphi)$

$Q=A\cdot\cos(\varphi-\qty{90}{\degree})=A\cdot\sin(\varphi)$

Lassen wir die Zeit weiterlaufen, dreht sich der zur Schwingung gehörende Zeiger. Seine Projektionen auf die beiden Achsen verlaufen sinusförmig und sind um $\qty{90}{\degree}$ gegeneinander phasenverschoben. Das Applet zeigt diesen Zusammenhang zwischen der Schwingung und ihrer I/Q-Darstellung.

[include:applet_iq_zeiger]

[question:AF633]

Anschaulich kann man sich vorstellen, dass zu Beginn jedes Symbolintervalls der zu übertragende Symbolwert einen Punkt in der I/Q-Ebene und damit die Amplitude und die anfängliche Phasenlage der Schwingung für dieses Symbol festlegt. Beim nächsten Symbol wird entsprechend auf den Signalzustand des nächsten Punktes übergegangen.

Für die Darstellung der Symbole interessiert uns also nicht die fortlaufende Drehung des Zeigers, sondern der für das jeweilige Symbol festgelegte Startzustand. Werden die möglichen Startzustände als Punkte in der I/Q-Ebene eingezeichnet, spricht man von einem *Konstellationsdiagramm* (vgl. Abbildung [ref:a_konstellationsdiagramm]). Jeder Punkt entspricht einem möglichen Symbol. Der Abstand eines Punktes vom Ursprung beschreibt die Amplitude des Signals. Sein Winkel gegenüber der I-Achse beschreibt die Phasenlage.

<margin>
[picture:1060:a_konstellationsdiagramm:Konstellationsdiagramm]
</margin>

<indepth>
Für mathematisch Interessierte: Eine sinusförmige Schwingung kann mathematisch auch als *komplexer Zeiger* beschrieben werden, der sich mit der Kreisfrequenz $\omega_\mathrm{c}$ dreht:

$s(t) = \Re\left\{A \cdot e^{j(\omega_\mathrm{c}t+\varphi)}\right\} = A\cos(\omega_\mathrm{c}t+\varphi)$

Dabei beschreibt $A$ die Amplitude und $\varphi$ die anfängliche Phasenlage des Signals. Der komplexe Ausdruck lässt sich in zwei Teile zerlegen:

$A \cdot e^{j(\omega_\mathrm{c}t+\varphi)} = \underbrace{A \cdot e^{j\varphi}}_{\text{Amplitude und Phase}} \cdot \underbrace{e^{j\omega_\mathrm{c}t}}_{\text{Träger}}$

In einem Konstellationsdiagramm interessiert uns der erste Teil $A \cdot e^{j\varphi}$. Er beschreibt Amplitude und Phasenlage des Signalzustands. Die fortlaufende Drehung des eigentlichen Trägers wird dabei nicht dargestellt.
</indepth>

Diese Darstellung werden wir in den folgenden Abschnitten immer wieder verwenden: Mit ihr lassen sich die möglichen Symbole digitaler Modulationsverfahren übersichtlich darstellen und später auch die Zuordnung von Bitkombinationen zu diesen Symbolen beschreiben.