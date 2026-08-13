Im vorherigen Kapitel haben wir die I/Q-Darstellung und den I/Q-Modulator kennengelernt. In einem digitalen System werden die beiden Komponenten I und Q als zwei getrennte digitale Datenströme verarbeitet. Diese können durch digitale Signalverarbeitung erzeugt, verändert und ausgewertet werden.

Auf der Empfängerseite wird das Eingangssignal dazu mit zwei Signalen gleicher Frequenz gemischt, die um $\qty{90}{\degree}$ gegeneinander phasenverschoben sind. Dadurch entstehen ein I- und ein Q-Signal. Beide Signale werden anschließend jeweils mit einem A/D-Umsetzer digitalisiert und können danach digital weiterverarbeitet werden. Auf der Senderseite funktioniert der Vorgang umgekehrt: Digitale I- und Q-Datenströme werden mit zwei D/A-Umsetzern in analoge Signale umgewandelt und anschließend einem I/Q-Modulator zugeführt.

Ein digitaler I/Q-Datenstrom kann einen Frequenzbereich um eine bestimmte Mittenfrequenz herum darstellen. Dabei werden Frequenzen unterhalb der Mittenfrequenz durch negative und Frequenzen oberhalb der Mittenfrequenz durch positive Frequenzabweichungen beschrieben.

Wird ein Eingangssignal beispielsweise mit zwei um $\qty{90}{\degree}$ gegeneinander phasenverschobenen Signalen von jeweils $\qty{435}{\mega\hertz}$ gemischt, repräsentiert der entstehende I/Q-Datenstrom einen Frequenzbereich um die Mittenfrequenz von $\qty{435}{\mega\hertz}$.

Wie groß dieser Frequenzbereich ist, hängt von der Abtastrate ab. Werden sowohl I als auch Q mit einer Abtastrate von $f_\mathrm{S}$ abgetastet, kann idealerweise ein Frequenzbereich von

$-\frac{f_\mathrm{S}}{2}$ bis $+\frac{f_\mathrm{S}}{2}$

um die Mittenfrequenz dargestellt werden. Die insgesamt darstellbare Bandbreite entspricht damit der Abtastrate $f_\mathrm{S}$.

Werden beispielsweise I und Q jeweils mit $\qty{10}{\mega\sample\per\second}$ abgetastet, kann der I/Q-Datenstrom einen Frequenzbereich von $\qty{-5}{\mega\hertz}$ bis $\qty{+5}{\mega\hertz}$ um die Mittenfrequenz darstellen. Bei einer Mittenfrequenz von $\qty{435}{\mega\hertz}$ entspricht dies einem Frequenzbereich von $\qty{430}{\mega\hertz}$ bis $\qty{440}{\mega\hertz}$.

[question:AF634]
[question:AF635]
[question:AF636]