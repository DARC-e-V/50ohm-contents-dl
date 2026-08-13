
%%% TODO diese beiden textblöcke müssen verbunden werden. 


Wie zuvor schon kurz angesprochen, muss vor dem A/D-Umsetzer ein entsprechendes Filter zur Unterdrückung von Signalanteilen höherer Frequenzen eingefügt werden. Man nennt ein solches Filter auch Antialiasingfilter. Als Filtertypen können hier sowohl Tiefpassfilter als auch Bandpassfilter Anwendung finden. Das Filter muss hierbei so beschaffen sein, dass Signalanteile, die sich oberhalb der halben Sampling-Frequenz befinden, wirksam unterdrückt werden. Wir erinnern uns, dass für die Abtastung eines Signals mehr als die doppelte Abtastfrequenz der zu erfassenden Signalfrequenz erforderlich ist.

[question:AF622]
[question:AF623]



Aus der Lektion zum Abtasttheorem wissen wir, dass ein Signal mit einer ausreichend hohen Abtastrate abgetastet werden muss. Über eine Antenne empfangen wir jedoch in der Regel viele unterschiedliche Signale – auch solche mit Frequenzen oberhalb des Frequenzbereichs, den wir eigentlich verarbeiten wollen.

Treffen solche Signale auf den A/D-Umsetzer, obwohl seine Abtastrate für diese Frequenzen nicht ausreichend ist, können sie als andere, nicht tatsächlich vorhandene Frequenzen im digitalen Signal erscheinen. Diese werden als *Aliase* bezeichnet.

Um dies zu verhindern, wird vor dem Eingang des A/D-Umsetzers ein *Antialiasing-Filter* eingesetzt. Dabei handelt es sich in der Regel um einen Tiefpass- oder Bandpassfilter, der unerwünschte Frequenzen unterdrückt, bevor das Signal den A/D-Umsetzer erreicht.

Der A/D-Umsetzer benötigt außerdem einen Taktgenerator, den man auch als Abtastratengenerator bezeichnet. Dieser legt fest, zu welchen Zeitpunkten das Eingangssignal abgetastet wird. Der A/D-Umsetzer erzeugt daraus einen digitalen Datenstrom, der anschließend von weiteren Teilen der Schaltung verarbeitet werden kann. Die Taktrate kann fest eingestellt sein oder beispielsweise durch einen Mikrocontroller gesteuert werden.

[question:AF620]