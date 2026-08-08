In der Klasse E haben wir ja bereits den Superheterodynempfänger kennengelernt. In dieser Klasse wollen wir uns nun mit dem Doppelsuperheterodynempfänger beschäftigen. Im Gegensatz zum Einfachsuper werden im Doppelsuper 2 Zwischenfrequenzen verwendet, wie in Abbildung [ref:doppelsuper_blockschaltbild] gezeigt.

<margin>
[picture:810:doppelsuper_blockschaltbild:Blockschaltbild eines Doppelsuper]
</margin>

Durch die Verwendung einer hohen ersten ZF ist, wie im vorherigen Abschnitt beschrieben, eine gute Spiegelfrequenzunterdrückung möglich. Die beiden möglichen Empfangsfrequenzen liegen hierdurch sehr weit auseinander und eine Unterdrückung der ungewünschten Empfangsfrequenz (Spiegelfrequenz) ist durch Eingangsfilter vor dem ersten Mischer leicht möglich. 

Durch die Verwendung einer niedrigen 2. ZF kann im 2. Schritt eine hohe Trennschärfe des Empfängers erreicht werden, da für niedrige Frequenzen Filter mit hoher Güte und steilen Flanken technisch sehr gut realisierbar sind.

Die erste ZF und die höchste gewünschte Empfangsfrequenz sollten bei einem Kurzwellenempfänger, je nach Empfängerkonzept, auch möglichst weit voneinander entfernt sein, um einen Direktempfang der ZF über die Antenne zu vermeiden. Die 1. ZF sollte daher das Doppelte der maximalen Empfangsfrequenz betragen.

<tip>
Eine Erweiterung des Doppelsuper-Konzeptes wäre der Dreifach-Super, bei dem eine niedrige 3. ZF gebildet wird. Dies kann sinnvoll sein für spezielle Demodulationsverfahren oder für die Realisierung von Störunterdrückungsverfahren (Notchfilter). Die Berechnung der Zwischenfrequenzen und Oszillatorfrequenzen erfolgt hierbei entsprechend dem des Doppelsupers.
</tip>

[question:AF112]
[question:AF113]

Nach dem ersten Mischer kann zur Verbesserung der Großsignalfestigkeit ein sehr schmales Filter, welches auf die 1. ZF abgestimmt ist, eingesetzt werden. Man nennt dieses Filter *Roofing Filter*. Die Bandbreite des Roofing-Filters muss hierbei mindestens so groß wie die größte benötigte Bandbreite der vorgesehenen Betriebsarten sein.

[question:AF114]
[question:AF116]

Der Doppelsuper setzt sich aus folgenden Funktionsblöcken zusammen:

1. HF-Teil mit Vorselektion
2. Erster Mischer mit VFO zur Bildung der ersten ZF. Hierbei kann die Frequenz des VFO sowohl oberhalb als auch unterhalb der gewünschten Empfangsfrequenz liegen (jeweils um die 1. ZF versetzt)
3. Erster ZF-Verstärker mit Filter (Roofing-Filter)
4. Zweiter Mischer mit CO (Quarzoszillator) zur Bildung der zweiten ZF. Hierbei kann die Frequenz des CO sowohl oberhalb als auch unterhalb der 1. ZF liegen (jeweils um die 2. ZF versetzt)
5. Zweiter ZF-Verstärker mit Filter (ZF-Filter je nach Modulationsart/Betriebsart, meist schaltbar).
6. Produktdetektor oder Demodulator (je nach Betriebsart) ggf. mit BFO. Diese Stufe dient auch der Erzeugung einer Regelspannung für die Steuerung der Eingangsempfindlichkeit des Empfangszweigs (AGC)
7. NF-Verstärker mit Lautsprecher-Ausgang oder Kopfhörer-Anschluss

[question:AF209]
[question:AF117]
[question:AF210]

Um die benötigten Oszillator-Frequenzen in Abhängigkeit einer gewünschten Empfangsfrequenz zu berechnen, muss man sich vergegenwärtigen, dass die Oszillatorfrequenzen jeweils ober- oder unterhalb der gewünschten Eingangsfrequenz des Mischers liegen können. Daher existieren für jede Mischerstufe jeweils zwei Lösungsmöglichkeiten.

1. Oszillatorfrequenz = Eingangsfrequenz + Ausgangsfrequenz
2. Oszillatorfrequenz = Eingangsfrequenz - Ausgangsfrequenz

Mit diesem Wissen lassen sich die folgenden Fragen beantworten.

[question:AF120]
[question:AF118]
[question:AF119]