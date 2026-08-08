Wie wir bereits in den Klassen N und E gelernt haben, befindet sich bei der Frequenzmodulation die Information des modulierenden Signals nicht in der Amplitude, sondern nur in der Frequenzänderung des Trägersignals. Daher müssen nur die Nulldurchgänge des Trägersignals im Empfänger ausgewertet werden. 

Amplitudenschwankungen werden durch einen Begrenzerverstärker hierbei ausgeblendet. Daher ist Frequenzmodulation systembedingt unempfindlich gegenüber impulsförmigen Störungen der Amplitude, die z.B. durch Zündfunken, Elektromotoren o.ä. hervorgerufen werden. FM eignet sich daher gut für den Betrieb in Kraftfahrzeugen.

[question:AE302]

In der Klasse A werden wir uns nun anschauen, wie Frequenzmodulation in einem Sender erzeugt werden kann und wie die Bandbreite eines FM-Signals berechnet werden kann.

---

Durch Änderung der Kapazität des frequenzbestimmenden Kondensators innerhalb eines Oszillators kann Frequenzmodulation erzeugt werden (vgl. [ref:fm_modulation_schaltung]). Beispielsweise kann mittels einer Kapazitätsdiode, die in Serie zu einem Schwingkreis oder Quarz liegt, Frequenzmodulation erzeugt werden. Die Amplitude der Niederfrequenz (NF), welche z.B. durch ein Mikrofon erzeugt wird, das an der Kapazitätsdiode anliegt, bestimmt hierbei direkt die Frequenzänderung des Oszillators.

[question:AE303]

<margin>
[picture:155:fm_modulation_schaltung:Einfache Schlatung zur Frequenzmodulation eines Oszillators mit Kapazitätsdiode]
</margin>

Die Modulationsfrequenz beeinflusst hierbei, wie häufig sich die Frequenz des Oszillators ändert.

[question:AE301]

In der Klasse E haben wir bereits den *Frequenzhub* kennengelernt. Er gibt an, um welchen Betrag die momentane Frequenz des FM-Signals durch das modulierende Signal gegenüber der Trägerfrequenz ausgelenkt wird. Je größer die Amplitude des modulierenden Signals ist, desto größer ist auch diese Frequenzauslenkung.

Bei der Demodulation im FM-Empfänger wird diese Frequenzauslenkung wieder in eine entsprechende Amplitude des demodulierten Signals umgesetzt. Ein größerer Frequenzhub führt daher bei ansonsten gleichen Bedingungen zu einer größeren Amplitude des demodulierten NF-Signals.

Ein größerer Frequenzhub vergrößert die benötigte Bandbreite des FM-Signals. Werden die vorgesehenen Werte überschritten, kann das ausgesendete Signal dadurch in benachbarte Kanäle hineinreichen und so Nachbarkanalstörungen verursachen.

[question:AE305]
[question:AE306]
[question:AE307]
[question:AE304]

---

Genau genommen wird die belegte Bandbreite einer FM-Aussendung nicht nur durch den Hub, sondern auch durch die maximale Modulationsfrequenz bestimmt (vgl. Abbildung [ref:fm_modulation]). In erster Näherung kann für kleinen Hub und niedrige Modulationsfrequenz die Carson-Formel angewendet werden. Sie gibt an, in welcher Bandbreite sich $\qty{99}{\percent}$ der Sendeleistung befinden.

$B\approx2 \cdot \left(\Delta f_{\textrm{T}} + f_{\textrm{mod max}} \right)$

<margin>
[picture:910:fm_modulation:Bandbreite Frequenzmodulation]
</margin>

Mittels der Carson-Formel lässt sich bei bekannten Werten für Hub und Modulationsfrequenz die belegte Bandbreite einer FM-Aussendung berechnen. Durch geeignetes Umstellen der Formel können auch jeweils die anderen Größen berechnet werden.

[question:AE309]
[question:AE308]
[question:AE311]
[question:AE312]
[question:AE310]
