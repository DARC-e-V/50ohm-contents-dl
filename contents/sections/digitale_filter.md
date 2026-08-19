Ein wesentlicher Vorteil der digitalen Verarbeitung von Signalen besteht darin, dass die digital vorliegenden Informationen nahezu beliebig bearbeitet werden können. Eine Folge von Eingangssamples wird mittels mathematischer Funktionen in eine Folge von Ausgangssamples umgerechnet. Einfache digitale Filter, wie Tief-, Band- oder Hochpässe, lassen sich dabei auf zwei unterschiedliche Arten ausführen: als FIR- und als IIR-Filter. Dabei steht FIR für *Finite Impulse Response* und IIR für *Infinite Impulse Response*.

Hauptmerkmal der FIR-Filter ist, wie auch schon die Bezeichnung "finite" (zu Deutsch endlich) besagt, dass nur eine begrenzte Anzahl an Eingangssamples für die Berechnung eines Ausgangssamples herangezogen wird. IIR-Filter verwenden hingegen zusätzlich bereits berechnete Ausgangssamples, die auf den Eingang der Berechnung zurückgeführt werden. Durch diese Rückkopplung kann ein einzelnes Eingangssample theoretisch unbegrenzt lange Einfluss auf die folgenden Ausgangssamples haben.

Digitale Filter können sowohl in Software auf einem DSP als auch in programmierbarer Hardware auf einem FPGA implementiert werden. Darüber hinaus gibt es sogenannte Mixed Signal Frontends, die verschiedene Signalverarbeitungsfunktionen, wie beispielsweise Dezimationsfilter, zusammen mit AD/DA-Wandlern in einem Chip realisieren, um sie möglichst energieeffizient auszuführen und nachfolgende Signalverarbeitungsstufen zu entlasten.

[question:AF631]

<indepth>
[picture:1133:a_fir:FIR-Filter]

Abbildung [ref:a_fir] zeigt schematisch den Aufbau eines FIR-Filters. Ein Eingangssample wird in einen Eingangsspeicher geschrieben. In jedem Takt werden die gespeicherten Werte wie bei einem Schieberegister um einen Speicherplatz weitergeschoben. Die Abgriffe der einzelnen Speicherplätze werden mit den entsprechenden Filterkoeffizienten multipliziert und anschließend summiert. Das Ergebnis wird als Ausgangssample ausgegeben.

Angenommen, die vier Filterkoeffizienten haben jeweils den Wert $\frac{1}{4}$, so werden die letzten vier Eingangssamples jeweils mit $\frac{1}{4}$ multipliziert und anschließend summiert. Das Ausgangssample ist damit der Mittelwert der letzten vier Eingangssamples. Ein solches Filter wird auch als *gleitender Mittelwert* bezeichnet.

Eine Eingangsfolge $0,0,0,4,0,0,0,0$ führt damit zur Ausgangsfolge $0,0,0,1,1,1,1,0$.

Das Filter glättet somit schnelle Änderungen, also hohe Frequenzanteile des Eingangssignals. Langsame Änderungen beziehungsweise niedrige Frequenzen werden weitgehend durchgelassen, während schnelle Änderungen beziehungsweise hohe Frequenzanteile abgeschwächt werden. Ein gleitender Mittelwert wirkt daher als sehr einfaches digitales Tiefpassfilter.

Das Filter führt eine sogenannte Faltungsoperation aus, diese ist übrigens auch die Grundlage vieler neuronaler Netze welche die Künstliche Intelligenz antreiben.
</indepth>