Signale können auf unterschiedliche Weise dargestellt werden. Bisher haben wir häufig den *Zeitbereich* betrachtet. Dabei wird dargestellt, wie sich beispielsweise die Spannung eines Signals mit der Zeit verändert. Dasselbe Signal kann jedoch auch im *Frequenzbereich* betrachtet werden. Dabei wird nicht mehr der zeitliche Verlauf dargestellt, sondern aus welchen Frequenzanteilen sich das Signal zusammensetzt und wie stark diese jeweils vertreten sind. Diese Darstellung bezeichnet man auch als *Frequenzspektrum*. Grundlage dafür ist die Tatsache, dass sich periodische Signale als Überlagerung von Sinusschwingungen unterschiedlicher Frequenz, Amplitude und Phase beschreiben lassen. Ein reines Sinussignal besteht beispielsweise nur aus einer einzigen Frequenz und erscheint daher im Frequenzspektrum nur bei dieser Frequenz.

Die *Fourier-Transformation* ermöglicht den Wechsel zwischen Zeit- und Frequenzbereich. Sie zerlegt ein Signal mathematisch in seine einzelnen Frequenzanteile. Für digital vorliegende, zeitdiskrete Signale wird dazu die *diskrete Fourier-Transformation* (DFT) verwendet. Die direkte Berechnung einer DFT kann bei einer großen Anzahl von Samples sehr aufwändig sein. Mit der *Fast-Fourier-Transformation* (FFT) steht ein wesentlich effizienterer Algorithmus zur Berechnung der DFT zur Verfügung. Deshalb wird die FFT häufig in Software und digitaler Hardware eingesetzt, beispielsweise um das Frequenzspektrum eines Signals zu bestimmen.

<indepth>
Nicht sinusförmige Signalformen bestehen aus mehreren Frequenzanteilen. Insbesondere scharfe Änderungen und Kanten im zeitlichen Signalverlauf erfordern zusätzliche hochfrequente Anteile. Mit dem folgenden Applet kann untersucht werden, wie sich unterschiedliche Sinusschwingungen überlagern und daraus verschiedene Signalformen entstehen.

[include:fourier]
</indepth>

[question:AF630]

---

Besonders deutlich wird der Zusammenhang zwischen Zeit- und Frequenzbereich bei Signalen mit scharfen Kanten. Ein ideales Rechtecksignal lässt sich beispielsweise aus einer Grundschwingung und mehreren Oberschwingungen zusammensetzen. Neben der Grundfrequenz treten dabei die ungeradzahligen Vielfachen der Grundfrequenz auf. Ihre Amplituden werden mit zunehmender Frequenz kleiner.

Diese Oberwellen sind auch bei Sendern von Bedeutung. Würde beispielsweise ein ideales Rechtecksignal unmittelbar auf eine Antenne gegeben, würden neben der gewünschten Grundfrequenz auch dessen Oberwellen abgestrahlt. Ein Tiefpassfilter kann die unerwünschten höheren Frequenzanteile unterdrücken, sodass hauptsächlich die gewünschte Grundschwingung zur Antenne gelangt.

Für einige typische periodische Signalformen lässt sich das Frequenzspektrum besonders einfach beschreiben. Dabei betrachten wir idealisierte Signalformen ohne Gleichanteil:

* Ein *Sinussignal* besteht nur aus einer einzigen Frequenz. Im Frequenzspektrum erscheint daher nur die Grundfrequenz $f$.
* Ein *Rechtecksignal* besteht aus der Grundfrequenz und den *ungeradzahligen Vielfachen* der Grundfrequenz. Es enthält also die Frequenzen $f$, $3\cdot f$, $5\cdot f$, $7\cdot f$ usw. Die Amplituden der Oberwellen werden mit zunehmender Frequenz kleiner.
* Ein *Sägezahnsignal* enthält sowohl die geradzahligen als auch die ungeradzahligen Vielfachen der Grundfrequenz. Es enthält also $f$, $2\cdot f$, $3\cdot f$, $4\cdot f$, $5\cdot f$ usw. Auch hier werden die Amplituden mit zunehmender Frequenz kleiner.
* Ein *Dreiecksignal* enthält wie das Rechtecksignal nur die ungeradzahligen Vielfachen der Grundfrequenz, also $f$, $3\cdot f$, $5\cdot f$, $7\cdot f$ usw. Die Amplituden der höheren Frequenzanteile nehmen jedoch wesentlich schneller ab als beim Rechtecksignal.

Damit lassen sich die Signalformen auch anhand ihres Frequenzspektrums unterscheiden. Ein einzelner Spektralanteil weist auf einen Sinus hin. Treten ungeradzahlige Vielfache auf, ist es in den Prüfungsfragen immer ein Rechtecksignal.

[question:AB404]
[question:AB405]
[question:AB406]
[question:AB407]