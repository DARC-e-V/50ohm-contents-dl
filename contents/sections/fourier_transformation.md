
% du kennst die zeitdarstellung
% du kennst die frequenzdarstellung
% fourier hat sich damit beschaeftigt wie man vom einen zum anderen kommt
% das zeitliche signal wir analysiert dahingehend wie "stark" welche sinusfrequenz enhalten ist
% zusammenfassung: jedes signal laesst sich in eine menge von sinusförmigen schwingungen aufteilen
% phase nicht vergessen

Kommen wir nun zu einem spannenden Thema, das komplizierter klingt, als es eigentlich ist. Man kann Signale auf verschiedene Arten und Weisen darstellen. Bekannt sein dürfte die Darstellung eines Signals im Zeitbereich. Hierbei wird auf der X-Achse die Zeit und auf der Y-Achse ein Spannungs- oder Leistungswert dargestellt.

Wusstest du, dass sich jedes Signal aus einzelnen Sinus-Schwingungen zusammensetzen lässt? Das klingt verrückt, aber so ist es. Jedes Signal kann durch eine Überlagerung von reinen Sinus-Schwingungen, die eine bestimmte Amplitude und Phase haben, beschrieben werden.

Die Fourier-Transformation ist eine mathematisch komplexe Funktion (die wir hier nicht näher erklären wollen), die ein Signal, das im Zeitbereich vorliegt, analysiert und im Anschluss darstellt, aus welchen einzelnen Sinus-Schwingungen sich das Signal aufbaut. Anschließend kann diese Information in einem Diagramm im Frequenzbereich oder auch Frequenzspektrum dargestellt werden. Hierbei beschreibt die X-Achse nun die Frequenz und die Y-Achse den Spannungswert oder auch Leistungswert der enthaltenen Frequenz im Ausgangssignal. Ein reines sinusförmiges Signal einer festen Frequenz stellt somit, im Frequenzspektrum dargestellt, einen Strich bei dessen Frequenz dar.

Die Fourier-Transformation (auch diskrete Fourier-Transformation kurz DFT benannt) ist in Ihrer ursprünglichen Form eine mathematisch aufwändige und komplexe Funktion. Diese ist in Software nur sehr ineffizient abzubilden. Über die Zeit hat man eine wesentlich effizientere Methode gefunden, diese mathematisch komplexe Funktion auf einfachere Art und Weise abzubilden - die Fast-Fourier-Transformation oder auch FFT genannt. Hiermit wird deren Berechnung, insbesondere in Soft- und Hardware, wesentlich vereinfacht.

<indepth>
Signalformen, welche nicht sinusförmig sind und insbesondere scharfe "Ecken und Kanten" enthalten, bestehen aus vielen verschiedenen Sinus-Frequenzanteilen und enthalten viele Oberwellenanteile. Mit diesem Applet lässt sich der Sachverhalt jedoch bereits ausprobieren.

[include:fourier]
</indepth>

[question:AF630]

Wir erinnern uns, dass Signale, die sehr eckig und kantig sind, höhere Frequenzanteile (sog. Oberschwingungen) enthalten. Sieht man sich ein solches Signal, beispielsweise ein rechteckiges Signal, nun im Frequenzbereich an, so fällt auf, dass dieses aus einem starken Sinus-Signal bei dessen Grundschwingung besteht als auch mehreren, immer schwächer werdenden Sinus-Signalen bei ungeradzahligen Vielfachen der Grundfrequenz. Dies ist im Übrigen auch der Grund, warum man Rechteck-Signale keinesfalls auf eine Antenne geben darf, bevor diese nicht ein Tiefpassfilter durchlaufen haben. Das Tiefpassfilter sorgt in diesem Fall dafür, dass höhere Signalanteile unterdrückt werden und an dessen Ausgang nur noch die Grundschwingung in Form eines Sinus-Signals austritt. Würde man das Rechtecksignal direkt auf die Antenne geben, so wäre eine Aussendung auf allen ungradzahligen Vielfachen der Grundfrequenz zu empfangen und würde sicherlich andere Funkdienste massiv stören.

[question:AB404]
[question:AB405]
[question:AB406]
[question:AB407]
