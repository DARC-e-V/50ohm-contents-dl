Die *Direkte Digitale Synthese*, englisch *Direct Digital Synthesis* oder kurz DDS [index:Direkte Digitale Synthese] [index:DDS], dient zur Erzeugung periodischer Signale mit einer sehr fein einstellbaren Frequenz. Sie wird heute neben der Frequenzsynthese mit PLL-Schaltungen häufig in modernen Amateurfunkgeräten eingesetzt. Ein wesentlicher Vorteil einer DDS besteht darin, dass sich die Ausgangsfrequenz digital mit einer sehr hohen Auflösung einstellen lässt. Außerdem kann sehr schnell zwischen unterschiedlichen Frequenzen gewechselt werden, da keine Regelschleife auf eine neue Frequenz einrasten muss, wie es bei einer klassischen PLL der Fall ist.

<margin>
[picture:1082:a_dds_aufbau:Blockschaltbild einer DDS (Direct Digital Synthesizer)]
</margin>

Der grundlegende Aufbau einer DDS ist in [ref:a_dds_aufbau] dargestellt. Ein Taktgenerator erzeugt ein Taktsignal mit einer festen Frequenz $f_\mathrm{Takt}$. Mit jedem Takt erhöht ein Phasenakkumulator [index:DDS:Phasenakkumulator], vereinfacht auch Adresszähler genannt, seinen aktuellen Phasenwert um das Phaseninkrement $K$:

$\varphi_{n+1} = \varphi_n + K$

Das Phaseninkrement $K$ wird auch als *Tuning Word* bezeichnet. Es bestimmt, um wie viele Phasenschritte der Phasenakkumulator bei jedem Takt weitergeschaltet wird. Der aktuelle Wert des Phasenakkumulators dient als Adresse für eine Wertetabelle, die auch als *Lookup-Tabelle* bezeichnet wird. Für die Erzeugung einer Sinusschwingung enthält diese Tabelle die digitalen Amplitudenwerte einer vollständigen Sinusperiode. Zu jedem Phasenwert wird der zugehörige Amplitudenwert aus der Sinustabelle ausgelesen. Durch die Größe des Phaseninkrements $K$ wird bestimmt, wie schnell die Sinustabelle durchlaufen wird und damit die Frequenz des Ausgangssignals. Das Phaseninkrement kann z. B. von einem Mikrocontroller gesteuert werden. Ein Register übernimmt den digitalen Amplitudenwert synchron zum Taktsignal und übergibt ihn an einen D/A-Wandler. Dieser wandelt die Folge der digitalen Amplitudenwerte in ein analoges, zunächst stufenförmiges Signal um. Ein nachgeschalteter Tiefpass entfernt unerwünschte hochfrequente Signalanteile und glättet das Ausgangssignal.

---

Durch das folgende Beispiel wird es anschaulich dargestellt: Bei einem Phaseninkrement von $K=1$ wird der Phasenwert mit jedem Takt um genau einen Schritt erhöht ($\varphi_{n+1} = \varphi_n + 1$). Die Sinustabelle wird dadurch schrittweise durchlaufen. Ist eine vollständige Periode erzeugt, wird der Adresszähler zurückgesetzt und der Phasenakkumulator beginnt erneut von vorne. Das entstehende Ausgangssignal ist in [ref:a_dds_phaseninkrement_k1] dargestellt.

<margin>
[picture:1083:a_dds_phaseninkrement_k1:Vergleichssignal]
</margin>

---

Wird das Phaseninkrement auf $K=2$ verdoppelt, erhöht sich der Phasenwert mit jedem Takt um zwei Schritte ($\varphi_{n+1} = \varphi_n + 2$). Dadurch wird nur jeder zweite Phasenwert aufgerufen und die Sinustabelle doppelt so schnell durchlaufen. Die Periodendauer des Ausgangssignals halbiert sich und seine Frequenz verdoppelt sich. Dies ist in [ref:a_dds_phaseninkrement_k2] dargestellt.

<margin>
[picture:1084:a_dds_phaseninkrement_k2:Doppeltes Phaseninkrement und doppelte Ausgangsfrequenz]
</margin>

[question:AD620]

<indepth>
Besitzt der Phasenakkumulator eine Breite von $N$ Bit, kann er $2^N$ unterschiedliche Phasenwerte darstellen. Wird der größte Wert überschritten, läuft der Zähler über und beginnt wieder am Anfang:

$\varphi_{n+1} = \left(\varphi_n + K\right) \bmod 2^N$

Dieser Überlauf entspricht dem Übergang von $\qty{360}{\degree}$ zurück zu $\qty{0}{\degree}$. Das Phaseninkrement $K$ kann nahezu beliebig gewählt werden und muss keine Zweierpotenz sein. Dadurch lassen sich auch Ausgangsfrequenzen erzeugen, die keine ganzzahligen Teiler der Taktfrequenz sind.

Eine DDS ist außerdem nicht auf Sinusschwingungen beschränkt. Enthält die Wertetabelle beispielsweise die Amplitudenwerte einer Dreieck- oder Sägezahnschwingung, kann die DDS auch diese Signalformen erzeugen.

Die Qualität des Ausgangssignals hängt vor allem von der Stabilität und dem Jitter [index:Jitter] des Taktgenerators sowie von der Auflösung und Linearität des D/A-Wandlers ab. Durch die begrenzte Anzahl an Phasen- und Amplitudenwerten entstehen Quantisierungsfehler und zusätzliche spektrale Anteile. Ein nachgeschalteter Tiefpass unterdrückt einen großen Teil dieser unerwünschten Signalanteile.
</indepth>