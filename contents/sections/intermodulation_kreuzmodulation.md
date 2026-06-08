In einem Empfänger, an dessen Eingang zwei starke HF-Signale anliegen, können Störungen durch Intermodulation oder Kreuzmodulation verursacht werden.
Bei Intermodulation äußert sich dieser Effekt so, dass durch nichtlineares Verhalten der Empfängerstufe (Betrieb im nichtlinearen Grenzbereich), ähnlich wie in einem Mischer, zusätzliche unerwünschte Frequenzen erzeugt werden. Diese können erwünschte Empfangssignale überlagern und stören.
Bei Kreuzmodulation äußert sich dieser Effekt so, dass das gewünschte Empfangssignal durch die Modulation eines starken frequenzmäßig benachbarten AM-Signals beeinflusst wird. Hierdurch wird die Modulation des benachbarten Senders im Empfangssignal hörbar und stört dieses.

[question:AF217]
[question:AF219]
[question:AF222]
[question:AF218]

Um ein starkes unerwünschtes Signal bereits vor dem Empfängereingang zu unterdrücken kann beispielsweise ein Saugkreis, welcher auf die exakte Frequenz des störenden Signals abgestimmt wird vor dem Empfängereingang für Abhilfe sorgen.

[question:AF223]

Die Großsignalfestigkeit eines Empfängers kann durch den sog. Intercept Point dritter Ordnung (IP3) beschrieben werden. Er ist ein Maß für den Punkt an dem unerwünschte Mischprodukte 3. Ordnung den Amplitudenwert des Eingangssignales erreichen. Je höher der IP3 eines Empfängers ist, desto größere Signale kann dieser noch störungsfrei verarbeiten.

<indepth>
Wir betrachten in dieser Vertiefung den IP3 als Kenngröße für die Großsignalfestigkeit eines Empfängers. Allgemein entstehen Mischprodukte durch Nichtlinearitäten in Verstärkern, Mischern oder anderen Empfängerstufen. Bei zwei Eingangssignalen $f_1$ und $f_2$ können Intermodulationsprodukte der Form

$f_\text{mix} = \left| m \cdot f_1 \pm n \cdot f_2 \right|$

entstehen, wobei $m,n \in \mathbb{N}_0$ gilt und nicht beide Koeffizienten gleichzeitig null sein dürfen. Die Ordnung eines solchen Mischprodukts ergibt sich aus der Summe der Koeffizienten:

$\text{Ordnung} = m+n$

Besonders kritisch sind die Intermodulationsprodukte 3. Ordnung, da sie häufig wieder in der Nähe der ursprünglichen Eingangssignale liegen. Dadurch können sie in den gewünschten Empfangsbereich fallen und sind dann durch nachfolgende Filter nur schwer oder gar nicht mehr zu entfernen.

In der folgenden Abbildung [ref:a_intermodulation] ist die Intermodulation zweier Signale $f_1$ und $f_2$ dargestellt. Die Intermodulationsprodukte 3. Ordnung sind dabei besonders hervorgehoben:

[picture:1095:a_intermodulation:Intermodulation von zwei Signalen $f_1$ und $f_2$]

Wichtig ist: Diese Intermodulationsprodukte werden nicht von außen empfangen, sondern entstehen erst im Empfänger durch nichtlineares Verhalten. Mit einem Zweitontest kann man die Linearität eines Empfängers untersuchen. Dazu werden zwei definierte Eingangssignale eingespeist. Erscheinen neben diesen beiden Grundsignalen zusätzlich Intermodulationsprodukte 3. Ordnung im Spektrum, zum Beispiel im Wasserfalldiagramm, ist dies ein Hinweis auf nichtlineares Verhalten.

Die Abbildung [ref:a_zweitontest] zeigt einen Zweitontest mit einem Powersweep, bei dem die Intermodulationsprodukte 3. Ordnung deutlich sichtbar werden.

[picture:1096:a_zweitontest:Zweitontest mit Powersweep]

Trägt man die Ausgangsleistung über der Eingangsleistung auf, steigen die Grundsignale im linearen Bereich mit einer Steigung von $1{:}1$. Die Intermodulationsprodukte 3. Ordnung steigen dagegen mit einer Steigung von $3{:}1$. Verlängert man die linearen Bereiche dieser beiden Kurven, ergibt sich ein theoretischer Schnittpunkt. Dieser Punkt wird IP3, also Intercept Point 3. Ordnung, genannt.

Der IP3 beschreibt somit den extrapolierten Punkt, an dem die Intermodulationsprodukte 3. Ordnung rechnerisch die gleiche Ausgangsleistung wie die Grundsignale erreichen würden. In der Praxis wird dieser Punkt meist nicht erreicht, da der Empfänger vorher in Kompression oder Sättigung gerät.

Je höher der IP3 eines Empfängers ist, desto besser ist seine Großsignalfestigkeit. Ein hoher IP3 bedeutet, dass auch starke Nachbarsignale verarbeitet werden können, ohne dass störende Intermodulationsprodukte im gewünschten Empfangsbereich entstehen.
</indepth>

[question:AF221]

Um das Entstehen von unerwünschten Mischprodukten im Empfängereingang durch starke Signale zu verringern kann ein schaltbares Dämpfungsglied (Attenuator) am Empfängereingang vorgeschaltet werden. Hierdurch werden Intermodulationsprodukte sowie Kreuzmodulation im Empfänger verringert. Das Nutzsignal wird hierbei nur um den Faktor des Dämpfungsgliedes reduziert - störende Mischprodukte werden jedoch aufgrund der mathematischen Gegebenheiten beim Mischprozess um den Faktor $\num{3}$ (3. Ordnung) in $\unit{\dB}$ abgeschwächt. Beispielsweise reduziert ein $\qty{10}{\dB}$ Dämpfungsglied das Nutzsignal nur um $\qty{10}{\dB}$ während unerwünschte Mischprodukte bereits um $\qty{30}{\dB}$ gedämpft werden.

[question:AF220]