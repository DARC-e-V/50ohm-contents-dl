
Sehen wir uns im Folgenden die Funktion des A/D-Umsetzers genauer an. Aus der Lektion Abtasttheorem wissen wir, dass wir, um die Information eines Signals ohne Informationsverluste abtasten zu können, mindestens mit etwas mehr als der doppelten Frequenz, die unser abzutastendes Signal enthält, abtasten müssen. Nun empfangen wir über eine Antenne in der Regel allerlei Signale - auch solche, die sich über der maximalen Frequenz, die wir verarbeiten wollen, befinden. Was passiert nun, wenn solche Signale auf den A/D-Umsetzer treffen? Rufen wir uns hierzu noch einmal das Beispiel mit der Fliege, die durchs Bild fliegt, ins Gedächtnis. Diese Signale können aufgrund der hierfür zu niedrigen Abtastfrequenz nicht mehr erfasst werden und erscheinen in unseren Samples als fehlerhaft erfasste Frequenzen. Diese nennen sich auch Aliases (zu Deutsch in etwa Pseudonyme). Ein Signal leicht oberhalb der maximalen Eingangsfrequenz würde als Alias mit einer Frequenz leicht unterhalb der maximalen Eingangsfrequenz unseres A/D-Umsetzers erscheinen und somit ein Signal darstellen, das es eigentlich gar nicht gibt. Um dies zu verhindern, müssen wir vor dem Eingang des A/D-Umsetzers ein Antialiasing-Filter (in der Regel ein Tiefpassfilter oder Bandpassfilter) schalten, so dass unerwünschte Frequenzen, die zu Aliases führen könnten, wirksam unterdrückt werden, bevor das Signal den A/D-Umsetzer erreicht.

Der A/D-Umsetzer benötigt für seine Aufgabe zudem einen Taktgenerator, welchen man auch Abtastratengenerator nennt, damit er in zeitlichen Abständen Samples des Eingangssignals generieren kann, die er dann als digitalen Datenstrom an weitere Teile einer Schaltung weitergeben kann. Die Taktrate kann fest eingestellt sein oder durch Kontrollinformationen z. B. von einem Mikrocontroller gesteuert werden.

[question:AF620]

Da ein A/D-Umsetzer stets mit einer begrenzten Zahl an möglichen digitalen Werten, welche die Größe des analogen Eingangssignals darstellen können, arbeitet, erfolgt die Erfassung der Amplitudenwerte in Stufen. Wir erinnern uns an das Beispiel mit dem Dimmer und Stufenschalter zuvor. Dadurch, dass das analoge Eingangssignal nun nur in bestimmten Stufen erfasst werden kann, kommt es zu Quantisierungsfehlern.

[question:AF607]

Die Anzahl der möglichen Stufen eines A/D-Umsetzers wird auch als dessen Auflösung bezeichnet. Man gibt diese Anzahl oft in Bit ($\unit{\bit}$) an. Kann ein Umsetzer $\num{256}$ Stufen (beispielsweise von $\num{-128}$ bis $\num{+127}$) unterscheiden, hat er $\qty{8}{\bit}$. Ein $\qty{16}{\bit}$-Umsetzer kann bereits $\num{65536}$ Stufen unterscheiden. Hierbei werden in der Regel die Hälfte der Werte für den positiven Signalbereich und die andere Hälfte der Werte für den negativen Signalbereich verwendet.

[question:AF608]

Eine weitere wichtige Eigenschaft eines A/D-Umsetzers besteht darin, das Eingangssignal möglichst exakt zu erfassen und dabei Fehler in den Zeitabständen zwischen einzelnen Samples zu vermeiden. Entscheidend hierfür ist ein möglichst stabiler Abtastratengenerator, der einen exakten zeitlichen Takt für den A/D-Umsetzer erzeugt. Leider ist dies technisch oft mit hohem Aufwand verbunden, weshalb es immer zu einem geringen Unterschied zwischen den Signalflanken des Takts kommen kann. Dies nennt man auch Jitter (zu Deutsch in etwa Zittern). Im Ergebnis führt dies zu zusätzlichem Rauschen im Abtastergebnis (dem digitalen Datenstrom) des A/D-Umsetzers.

[question:AF621]

