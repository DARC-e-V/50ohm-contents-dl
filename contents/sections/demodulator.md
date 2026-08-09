Im Gegensatz zur Modulation, die auf der Senderseite stattfindet, bewirkt die Demodulation von Signalen im Empfänger, dass ein moduliertes Signal z. B. wieder in NF umgewandelt wird und somit hörbar wird oder eine Bitfolge bei einer digitalen Übertragung entsteht.

Je nachdem welche Modulationsart auf der Senderseite verwendet wurde muss auf der Empfängerseite eine entsprechende Demodulation stattfinden. Hierfür gibt es unterschiedliche Schaltungskonzepte, die die Demodulation ermöglichen. Wie Modulation im Digitalen funktioniert, werden wir uns in einem späteren Kapitel anschauen. In diesem Kapitel werden wir uns zunächst mit der Demodulation von analogen Signalen beschäftigen.

Die einfachste Form der Demodulation eines Hochfrequenz-Signals stellt die Amplituden-Modulation (AM) dar.
AM-Signale können mittels eines sog. Hüllkurven-Demodulator wie in Abbildung [ref:demodulator_huellkurvendemodulator_am] demoduliert werden. Hierzu wird das hochfrequente Signal zunächst nach der gewünschten Empfangsfrequenz selektiert z. B. mittels eines angepassten Schwingkreises und anschließend über eine Diode gleichgerichtet. Ein der Diode nachgeschalteter Kondensator wird auf den momentanen Spitzenwert des Signals aufgeladen und gleichzeitig über einen zu diesem parallel geschalteten Widerstand mit einer geeigneten Zeitkonstante entladen. Diese Zeitkonstante liegt deutlich über der Periodendauer des HF-Signals jedoch deutlich unter der Periodendauer des NF-Signals.

<margin>
[picture:141:demodulator_huellkurvendemodulator_am:Hüllkurvendemodulator zur Demodulation von AM-Signalen]
</margin>

[question:AD501]

Am Anschluss X in Abbildung [ref:demodulator_huellkurvendemodulator_am_2] wird jeweils die gleichgerichtete Spitzenspannung des HF-Signals abgebildet, die zwischen den Spitzen des HF-Signals entsprechend der Zeitkonstante des parallel zum Kondensator geschalteten Widerstandes leicht abfällt. Die Hüllkurve des Signals entspricht damit der aufmodulierten NF, die aufgrund der Zeitkonstante des Kondensators mit einem Sägezahn-Signal (Trägerfrequenz) überlagert ist und entspricht dem Signal in Abbildung [ref:demodulator_huellkurvendemodulator_am_abbx]. In den nachfolgenden NF-Verarbeitungsstufen (nicht abgebildet) werden die Reste dieser Trägerfrequenz dann ausgefiltert, so dass die reine NF als Ausgangssignal verbleibt (vgl. Abbildung [ref:demodulator_huellkurvendemodulator_am_clean]).

<margin>
[picture:607:demodulator_huellkurvendemodulator_am_2:Hüllkurvendemodulator zur Demodulation von AM-Signalen mit Darstellung des ZF-Eingangssignals welches am Eingang des Demodulators anliegt]
[picture:146:demodulator_huellkurvendemodulator_am_abbx:Demoduliertes Signal am Punkt X des Hüllkurvendemodulators]
[picture:147:demodulator_huellkurvendemodulator_am_clean:Gefiltertes Signal am Ausgang des Hüllkurvendemodulators]
</margin>

[question:AD502]

---
<margin>
[picture:841:demodulator_flankendiskriminator:Schwingkreis der als Flankendiskriminator verwendet wird]

[picture:149:demodulator_flankendiskriminator_schaltung:FM-Flankendiskriminator]
</margin>

Eine sehr ähnliche Schaltung wie der vorgenannte Hüllkurven-Demodulator kann zur Demodulation von FM-Signalen verwendet werden.
Ausgehend von der Zwischenfrequenz im FM-Empfänger läuft, wie in Abbildung [ref:demodulator_flankendiskriminator], das Signal in einen Schwingkreis, der mit seiner Resonanzfrequenz $f_\text{res}$ leicht oberhalb oder unterhalb der ZF-Frequenz $f_\text{ZF}$ abgestimmt ist. Hierdurch liegt das zu demodulierende FM-Signal auf der Flanke des Schwingkreises und wandelt Frequenzänderungen der FM in Amplitudenänderungen um. Mittels des nachgeschalteten AM-Demodulators wird das nunmehr in ein AM-Signal umgewandelte FM-Signal dann demoduliert und hörbar gemacht. Diese Schaltung, gezeigt in Abbildung [ref:demodulator_flankendiskriminator_schaltung] wird Flankendiskriminator genannt.

[question:AD504]

---

FM-modulierte Signale lassen sich ebenfalls mittels einer PLL (Phase Locked Loop) demodulieren (vgl. Abbildung [ref:demodulator_pll]). In einer PLL wird ein spannungsgesteuerter Oszillator (VCO) über eine Phasenregelschleife frequenzfolgend an ein Eingangssignal gekoppelt. Wenn sich die Frequenz des Eingangssignals ändert (FM-Modulation) folgt die Regelspannung des VCO der FM-Modulation. Diese Regelspannung entspricht dann genau der Modulation des FM-Signals und somit der aufmodulierten NF und kann an der PLL abgegriffen werden zur weiteren Verarbeitung.

<margin>
[picture:77:demodulator_pll:PLL zur Demodulation von FM-Signalen]
</margin>

[question:AD505]

---

Um SSB-modulierte Signale zu demodulieren verwendet man einen sog. Produktdetektor. Dieser ist im Wesentlichen ein Ringmischer, welchen wir schon im Empfängerkapitel kennen gelernt haben, der als Eingangssignale die ZF des Empfängers sowie einen BFO (Beat Frequency Oscillator) verwendet. Durch Mischung (Produkt) dieser beiden Eingangssignale entsteht als eines der Mischprodukte das gewünschte NF-Signal (SSB-Signal), welches am Ausgang zur weiteren Verarbeitung abgegriffen werden kann. Für bestmögliche Verständlichkeit der demodulierten NF muss der BFO auf die Frequenz des unterdrückten Trägers des SSB-Signals abgestimmt werden.


<indepth>
[picture:153:demodulator_produktdetektor:Produktdetektor zur Demodulation von SSB-Signalen]
[picture:1125:a_produktdetektor_spannung:Beispiel für Spannungen am Produktdetektor]

Zur Demodulation eines SSB-Signals wird häufig ein sogenannter *Produktdetektor* eingesetzt. Dieser kann beispielsweise als Ringmischer aufgebaut sein. Als Eingangssignale erhält er das SSB-Signal auf der Zwischenfrequenz (ZF) und das Signal eines *Beat Frequency Oscillators (BFO)*.

Die Funktionsweise lässt sich vereinfacht mit einem schaltenden Mischer erklären. Das BFO-Signal schaltet den Ringmischer abwechselnd in zwei Zustände. Vereinfacht kann man sich das BFO daher als ein Signal vorstellen, das zwischen den Werten $+1$ und $-1$ umschaltet, wie im oberen Verlauf der Abbildung [ref:a_produktdetektor_spannung] dargestellt.

Das ZF-Signal wird dadurch abwechselnd unverändert durchgeschaltet oder in seiner Polarität umgekehrt. In der vereinfachten Darstellung kann das ZF-Signal deshalb als Produkt aus dem NF-Signal und dem BFO-Schaltsignal betrachtet werden:

$u_\mathrm{ZF}(t)=u_\mathrm{NF}(t)\cdot s_\mathrm{BFO}(t)$

Im Produktdetektor wird dieses Signal erneut mit dem BFO-Signal multipliziert:

$u_\mathrm{ZF}(t)\cdot s_\mathrm{BFO}(t)=u_\mathrm{NF}(t)\cdot s_\mathrm{BFO}(t)\cdot s_\mathrm{BFO}(t)$

Da das vereinfachte BFO-Schaltsignal nur die Werte $+1$ und $-1$ annimmt, gilt:

$s_\mathrm{BFO}^2(t)=1$

Damit bleibt als niederfrequenter Anteil wieder das ursprüngliche NF-Signal übrig:

$u_\mathrm{NF}(t)=u_\mathrm{ZF}(t)\cdot s_\mathrm{BFO}(t)$

Neben dem gewünschten NF-Signal entstehen beim Mischvorgang weitere hochfrequente Mischprodukte. Diese werden am Ausgang des Produktdetektors durch einen Tiefpass unterdrückt.

Damit das ursprüngliche NF-Signal mit der richtigen Tonhöhe wiedergewonnen wird, muss die Frequenz des BFO passend zur Frequenz des unterdrückten Trägers des SSB-Signals eingestellt sein.
</indepth>

[question:AD506]

