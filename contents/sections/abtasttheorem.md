Sehen wir uns nun den Prozess des Samplings mal etwas genauer an und rufen uns noch einmal das vorgenannte Beispiel der Kamera, die in bestimmten Abständen Bilder einer Szene aufnimmt, ins Gedächtnis. Nehmen wir zum Beispiel an, dass unsere Kamera 24 Bilder pro Sekunde einer bestimmten Szene aufnimmt. Wenn man sich nun z. B. vorstellt, dass wir einen Läufer beim Laufen filmen, so werden wir feststellen, dass zwischen den einzelnen Bildern immer eine ruckartige Bewegung der Beine und des Körpers unseres Läufers gegenüber dem vorigen Bild stattfindet. Lassen wir die Bilder zeitlich schnell hintereinander ablaufen, entsteht ein optisch kontinuierlicher Bewegungsablauf. Die Information, die wir bei 24 Bildern pro Sekunde erfassen, ist jedoch zeitlich begrenzt (merke: zeitdiskret). Was wäre wenn nun zwischen 2 aufeinanderfolgenden Bildern plötzlich eine Fliege schnell vor der Linse unserer Kamera hindurchfliegt? Würden wir dies noch wahrnehmen können? Dies hängt davon ab, ob die Fliege den richtigen Zeitpunkt zwischen zwei Bildern für ihren Durchflug wählt. Würde sie erst nach Aufnahme eines Bildes in den Sichtbereich der Kamera kommen und diesen vor Aufnahme des darauffolgenden Bildes bereits wieder verlassen haben, so könnten wir dieses Ereignis in den von uns aufgenommenen Bildern nicht nachvollziehen. Es bliebe uns Information verborgen.

<webonly>
<margin>
[include:applet_nyquist]
</margin>
</webonly>

Genauso verhält es sich mit dem Sampling bei analogen Signalen. Werden diese mit einer bestimmten Abtastrate $f_\text{s}$ erfasst (gesampelt), so können wir zeitlich schnelle Änderungen des Signals zwischen 2 Samples ggf. nicht mehr erfassen. Sampling bedeutet somit auch immer einen Verlust an zeitlicher Information. Nun kann man sich überlegen, welche zeitliche Auflösung erforderlich ist, um ein analoges Signal einer bestimmten Frequenz (Wechsel der Signalamplitude pro Sekunde) noch ohne Verlust von Information (alle Wechsel sollen erfasst werden) abzutasten. Hierfür kann man folgende Überlegung anstellen. Um mindestens jeden Wechsel des Signals einwandfrei erfassen zu können, muss man (wie bei unserem vorgenannten Beispiel mit der Kamera), in der Lage sein sicherzustellen, dass mindestens vor und nach jedem Wechsel des Signals ein Sample genommen wird. Im Fall unserer Fliege, die durch das Bild fliegt, wäre die Voraussetzung, dass die Fliege nur so schnell durch das Bild fliegen darf, dass sie mindestens auf 2 Bildern zu sehen ist. Ansonsten könnte man nicht sagen, von wo sie durch das Bild geflogen ist und in welche Richtung. Ist diese Voraussetzung nicht erfüllt, entgeht uns diese Information. Man spricht in diesem Fall auch davon, dass eine fehlerfreie Rekonstruktion nicht möglich ist.

Man kann mathematisch zeigen, dass für die Erfassung eines Signals mit der höchsten vorkommenden Frequenz $f_{\mathrm{max}}$ die Abtastrate $f_\text{s}$ mehr als das Doppelte, also etwas mehr als $f_\text{s} > 2 \cdot f_{\mathrm{max}}$, betragen muss, damit wir unser Signal wieder einwandfrei rekonstruieren können. Diese Erkenntnis nennt sich in der digitalen Signalverarbeitung auch Abtasttheorem und ist nach dessen Entdeckern Nyquist und Shannon auch als Nyquist-Shannon-Abtasttheorem oder Nyquist-Bedingung bekannt. Das Abtasttheorem bestimmt also die für eine fehlerfreie Rekonstruktion eines Signals theoretisch notwendige minimale Abtastrate $f_\text{s}$.

[question:AF618]

[question:AF616]

---

Wird das Theorem nicht erfüllt, treten sogenannte Alias-Effekte, bzw. Aliasing-Effekte auf. 

[question:AF617]

<webonly>
Das nebenstehende Applet ermöglicht es, mit der Abtastrate zu experimentieren. Fällt die Abtastrate unter $\qty{2}{\kilo\hertz}$, ist die Nyquist-Bedingung nicht mehr erfüllt, und das Signal kann nicht mehr eindeutig rekonstruiert werden.
Interessant ist auch, dass selbst bei einer Abtastfrequenz von genau $\qty{2}{\kilo\hertz}$ die Rekonstruktion nicht zuverlässig funktioniert. Daher wählt man üblicherweise eine Abtastrate, die etwas oberhalb der Nyquist-Bedingung liegt, um eine sichere Signalrekonstruktion zu gewährleisten.
</webonly>

<indepth>
Nehmen wir ein praktisches Beispiel wie im Fall eines CD-Players, der mit einer Abtastrate von z. B. $\qty{44,1}{\kilo\sps}$ arbeitet. Wenn man das Abtasttheorem wie oben beschrieben zugrunde legt, bedeutet dies, dass mit einer Abtastrate von $\qty{44,1}{\kilo\sps}$ nur Frequenzen unterhalb von $\qty{22,05}{\kilo\hertz}$ abgebildet werden können. Somit können Frequenzen bis ca. $\qty{22}{\kilo\hertz}$ noch korrekt abgebildet werden. Dies entspricht dem HiFi-Frequenzbereich von guten Stereoanlagen. 
</indepth>

Mit der folgenden Aufgabe kannst du dein Wissen zum Abtasttheorem testen.

[question:AF619]

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