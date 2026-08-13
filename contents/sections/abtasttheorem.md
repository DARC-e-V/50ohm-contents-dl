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
