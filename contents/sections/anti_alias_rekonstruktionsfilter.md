Bei der A/D- und D/A-Umsetzung werden analoge und digitale Signalverarbeitung miteinander verbunden. Dabei werden sowohl vor dem A/D-Umsetzer als auch nach dem D/A-Umsetzer analoge Filter benötigt. Die Abbildung [ref:a_adc_dac_filter] zeigt die gesamte Signalkette. Auf der Eingangsseite befindet sich vor dem A/D-Umsetzer ein *Anti-Aliasing-Filter*. Es begrenzt den Frequenzbereich des analogen Eingangssignals, bevor dieses abgetastet wird. Nach der digitalen Signalverarbeitung erzeugt der D/A-Umsetzer wieder ein analoges Signal. Ein nachgeschaltetes *Rekonstruktionsfilter* entfernt dabei unerwünschte hochfrequente Signalanteile. Warum beide Filter benötigt werden, betrachten wir in dem folgenden Abschnitt.

<margin>
[picture:1131:a_adc_dac_filter:A/D- und D/A-Umsetzung mit Anti-Aliasing- und Rekonstruktionsfilter]
</margin>

---

Aus der Lektion zum Abtasttheorem wissen wir, dass ein Signal mit einer ausreichend hohen Abtastrate abgetastet werden muss. Für ein Signal mit der höchsten zu erfassenden Frequenz $f_\mathrm{max}$ muss die Abtastrate größer als $2\cdot f_\mathrm{max}$ sein.

Über eine Antenne empfangen wir jedoch in der Regel viele unterschiedliche Signale – auch solche mit Frequenzen oberhalb des Frequenzbereichs, den wir eigentlich verarbeiten wollen. Treffen solche Signalanteile auf den A/D-Umsetzer, obwohl dessen Abtastrate für diese Frequenzen nicht ausreichend ist, können sie im digitalen Signal als andere, tatsächlich nicht vorhandene Frequenzen erscheinen. Diese werden als *Aliase* bezeichnet.

Um dies zu verhindern, wird vor dem Eingang des A/D-Umsetzers ein *Anti-Aliasing-Filter* eingesetzt. Dabei handelt es sich je nach Anwendung beispielsweise um einen Tiefpass- oder Bandpassfilter. Ein Bandpassfilter könnte z. B. für Sprache verwendet werden. Das Filter muss unerwünschte Signalanteile, die beim Sampling zu Aliasing führen könnten, ausreichend unterdrücken. Insbesondere dürfen Frequenzanteile oberhalb der halben Samplingfrequenz nicht ungehindert zum A/D-Umsetzer gelangen.

[question:AF622]
[question:AF623]

<indepth>
Ein anschauliches Beispiel für *Aliasing* begegnet uns auch im Alltag bei digitalen Bildern. Fotografiert man mit einer Kamera sehr feine, regelmäßig wiederkehrende Strukturen, beispielsweise ein engmaschiges Gitter, einen Stoff mit feinen Streifen oder ein Fliegengitter, können im Bild plötzlich größere Muster entstehen, die im Original gar nicht vorhanden sind. Diese werden als *Moiré-Muster* bezeichnet.

Die Ursache ist ähnlich wie beim Abtasten eines elektrischen Signals. Ein Kamerasensor kann ein Bild nicht an beliebig vielen Stellen erfassen, sondern besitzt nur eine endliche Anzahl von Bildpunkten. Ist eine Struktur feiner als die räumliche Auflösung des Sensors, wird sie nicht mehr eindeutig abgetastet. Aus der eigentlich vorhandenen feinen Struktur kann dadurch scheinbar eine andere, gröbere Struktur entstehen.

Beim A/D-Umsetzer geschieht das gleiche Prinzip auf der Zeitachse: Wird eine zu hohe Signalfrequenz mit einer zu niedrigen Samplingrate abgetastet, erscheint im digitalisierten Signal eine andere, niedrigere Frequenz, die ursprünglich gar nicht vorhanden war.

Ein Moiré-Muster kann daher als sichtbares Beispiel dafür betrachtet werden, wie durch eine unzureichende Abtastung neue, scheinbare Strukturen entstehen.

% TODO: Bild besorgen
%<margin>
%[picture:XXXX:a_moire:Moiré-Muster als Beispiel für räumliches Aliasing]
%</margin>
</indepth>

---

Der A/D-Umsetzer benötigt außerdem einen Taktgenerator, den man auch als Abtasttaktgenerator bezeichnet. Dieser legt fest, zu welchen Zeitpunkten das Eingangssignal abgetastet wird und bestimmt damit die Samplingrate. Die Samplingrate kann fest eingestellt sein oder beispielsweise durch einen Mikrocontroller gesteuert werden.

<margin>
[picture:1132:a_anit_alias:Anti-Aliasing-Filter, A/D-Umsetzer und Taktgenerator]
</margin>

[question:AF620]

---

Auf der anderen Seite der digitalen Signalverarbeitung übernimmt der D/A-Umsetzer den umgekehrten Vorgang. Er setzt die digitalen Samples wieder in analoge Spannungswerte um. Da die einzelnen Werte nur in festen zeitlichen Abständen ausgegeben werden, entsteht am Ausgang des D/A-Umsetzers zunächst kein ideal glatter Signalverlauf.

Durch die zeitdiskrete Ausgabe entstehen neben dem gewünschten Nutzsignal auch unerwünschte höherfrequente Signalanteile (z.B. in Abbildung [ref:a_adc_4bit], die schnellen Übergänge zwischen den diskreten Werten des Ausgangssignals enthalten die hohen Frequenzanteile). Um diese zu unterdrücken, wird hinter dem D/A-Umsetzer ein *Rekonstruktionsfilter* eingesetzt. Auch hierbei kann je nach Anwendung beispielsweise ein Tiefpass- oder Bandpassfilter verwendet werden.

Das Rekonstruktionsfilter lässt den gewünschten Nutzfrequenzbereich passieren und unterdrückt die unerwünschten höherfrequenten Signalanteile des D/A-Umsetzers. Dadurch entsteht am Ausgang wieder ein möglichst sauberes analoges Signal (vgl. Abbildung [ref:a_adc_12bit], das Rekonstruktionsfilter glättet das Signal).

[question:AF624]
[question:AF625]

<margin>
[picture:300:a_adc_4bit:Signal vor dem Rekonstruktionsfilter]
[picture:299:a_adc_12bit:Signal nach dem Rekonstruktionsfilter]
</margin>
