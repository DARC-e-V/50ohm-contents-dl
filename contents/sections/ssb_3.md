Zur Reduzierung der maximalen Bandbreite eines ausgestrahlten SSB-Signals und effizienten Nutzung des vorhandenen Frequenzspektrums, sollte die maximale NF-Modulationsbandbreite eines SSB-Signals nicht mehr als $\qty{2,7}{\kilo\hertz}$ betragen. Dies ermöglicht einen minimalen Abstand zwischen SSB-Signalen von $\qty{3}{\kilo\hertz}$, für störungsfreien Betrieb.

[question:AE208]
[question:AE209]

Wird ein SSB-Signal im Modulator des Senders übersteuert, so entstehen hierbei Verzerrungen, die zu Nebenaussendungen führen. Diese Nebenaussendungen werden umgangssprachlich auch als "Splatter" bezeichnet und können benachbarte Aussendungen stören, da die Bandbreite des Sendesignals in diesem Fall die geforderten $\qty{2,7}{\kilo\hertz}$ überschreitet.
[question:AE205]

Die Sprache jedes Menschen hat ein individuelles Frequenzspektrum. Für die bestmögliche Verständlichkeit bei SSB-Aussendungen sollten Sprachfrequenzen im höheren Bereich angehoben werden und in tieferen Frequenzbereichen abgeschwächt werden. Hierfür dient ein Equalizer im Mikrofonverstärker des Senders, der eine individuelle Einstellung des Frequenzgangs des Modulationssignals ermöglicht. Hierdurch wird der Frequenzgang des Mikrofons optimal auf den jeweiligen Operator angepasst.
[question:AE213]

---

Um die Hüllkurvenform eines SSB-Senders bzgl. Qualität und Linearität beurteilen zu können kann ein Zweiton-Signal zur Modulation des SSB-Senders verwendet werden. Hierbei wird der SSB-Sender mit einem NF-Signal moduliert, das aus zwei überlagerten NF-Frequenzen besteht. Diese NF-Frequenzen dürfen in keinem ganzzahligen Verhältnis zueinander stehen. Durch die Überlagerung entstehen in der ausgesendeten HF Maxima und Minima (Nulldurchgänge) des HF-Signals. Zur Modulation können z.B. ein $\qty{700}{\hertz}$ und ein $\qty{1200}{\hertz}$ Ton verwendet werden. Hieraus ergibt sich bei Messung des HF-Signals mittels eines Oszilloskops (an einem Lastwiderstand) eine Schwebung der HF von $\qty{500}{\hertz}$, die im Idealfall sinusförmig sein sollte. Das Zweiton-Signal ermöglicht auch die Messung der Hüllkurvenleistung (PEP) eines SSB-Senders mittels Darstellung der Kurvenform auf dem Oszilloskop.

[question:AI304]

<margin>
[picture:1092:a_ssb_zweiton:Zweiton-Signal zur Beurteilung der Hüllkurvenform eines SSB-Senders]
</margin>

Die Abbildung [ref:a_ssb_zweiton] zeigt in 1. ein Eintonsignal, also einen einfachen sinusförmigen NF-Ton. In 2. und 3. ist dargestellt, wie dieses Eintonsignal bei AM beziehungsweise SSB auf die HF umgesetzt wird. Das SSB-Signal in 3. besteht aus einer einzelnen HF-Komponente mit konstanter Amplitude und erscheint damit wie ein unmodulierter HF-Träger auf einer gegenüber dem unterdrückten Träger verschobenen Frequenz. An einem solchen Eintonsignal lassen sich die Qualität und Linearität eines SSB-Senders jedoch nur eingeschränkt beurteilen; insbesondere treten keine aussagekräftigen Intermodulationsprodukte zwischen mehreren Nutzsignalen auf.

In 4. ist ein Zweiton-Nutzsignal zu sehen, das aus der Überlagerung zweier Sinustöne mit $\qty{700}{\hertz}$ und $\qty{1200}{\hertz}$ besteht. In 5. und 6. wird gezeigt, wie dieses Zweitonsignal bei AM beziehungsweise SSB auf die HF umgesetzt wird. Beim SSB-Zweitonsignal in 6. entstehen zwei HF-Komponenten im Abstand von $\qty{500}{\hertz}$. Durch deren Überlagerung entsteht eine periodische Schwebung der HF-Hüllkurve mit der Differenzfrequenz von $\qty{500}{\hertz}$. Diese Hüllkurve ermöglicht die Messung der Spitzen-Hüllkurvenleistung (PEP) und dient gleichzeitig zur Beurteilung der Linearität des Senders, da Nichtlinearitäten zu zusätzlichen Intermodulationsprodukten im Spektrum führen.

[question:AE207]

Für die folgenden Aufgaben muss die Senderausgangsleistung als Spitzen-Hüllkurvenleistung (PEP) bestimmt werden. Die PEP beschreibt die effektive Leistung, die der Sender während der Spitze der Modulationshüllkurve abgibt. Sie bezieht sich also nicht auf die mittlere Leistung über die gesamte Modulation, sondern auf den Leistungswert im Maximum der Hüllkurve, wie in Abbildung [ref:a_pep_hüllkurve] dargestellt. Die Spitzenspannung zur Berechnung der Effektivleistung kann man im Oszillogramm ablesen. Dabei muss man auf das Tastkopfverhältnis achten.

<margin>
[picture:875:a_pep_hüllkurve:Modulationshüllkurve zur Leistungsberechnung]
</margin>

% Tastkopf 1:1 PEP
[question:AI305]

% Tastkopf 10:1 PEP
[question:AI306]