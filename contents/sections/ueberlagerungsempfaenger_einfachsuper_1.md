Als einfachsten Empfänger haben wir den Detektorempfänger im vorherigen Kapitel kennengelernt. Beim Detektorempfänger handelt es sich um einen sog. Geradeausempfänger, den wir auch schon in der Klasse N kennen gelernt haben. Beim Geradeausempfänger wie in Abbildung [ref:e_geradeausempfänger] gezeigt, wird das Signal nach Empfang und ggf. Verstärkung nur noch demoduliert. Dieses Empfängerkonzept hat jedoch den Nachteil einer schlechten Selektivität (Trennschärfe). Um das zu verbessern könnte man den Eingangsfilterblock (2) aus mehreren Filtern kombinieren um die Trennschärfe zu erhöhen. Dann müssten aber beim Wechsel der Empfangsfrequenz alle diese Filter angepasst werden und das ist sehr aufwändig. Aus diesem Grund wurde der *Überlagerungsempfänger* (vgl. Abbildung [ref:ueberlagerungsempfaenger_einfachsuper]) entwickelt, welcher in der Fachsprache auch *Superheterodyn* oder *Superhet* genannt wird.

<margin>
[picture:736:e_geradeausempfänger:Geradeausempfänger]
</margin>

<margin>
[picture:803:ueberlagerungsempfaenger_einfachsuper:Überlagerungsempfänger mit Verstärkern]
</margin>

---

Die Idee des Überlagerungsempfängers ist ebenso einfach wie genial. Anstelle abstimmbarer Filter wird ein variabler Oszillator (VFO, engl. Variable Frequency Oscillator) eingesetzt, mit dessen Hilfe das empfangene Signal zunächst auf eine feste Frequenz, die sogenannte Zwischenfrequenz $f_\mathrm{z}$ (oft auch ZF genannt), umgesetzt wird. Für diese feste Zwischenfrequenz lassen sich sehr trennscharfe und hochwertige Filter realisieren. Abbildung [ref:ueberlagerungsempfaenger_einfachsuper_filter] veranschaulicht dieses Prinzip.

<margin>
[picture:913:ueberlagerungsempfaenger_einfachsuper_filter:Überlagerungsempfänger mit Filtern]
</margin>

Das Eingangsfilter lässt zunächst nur den gewünschten Frequenzbereich, beispielsweise den Kurzwellenbereich, passieren. Anschließend setzt ein Mischer das Eingangssignal zusammen mit der Frequenz des VFO auf die konstante Zwischenfrequenz um, zum Beispiel auf $\qty{455}{\kilo\hertz}$. Im konkreten Beispiel kann der VFO zwischen $\qty{3,455}{\mega\hertz}$ und $\qty{30,455}{\mega\hertz}$ eingestellt werden, um den gesamten Bereich der Kurzwelle heruntermischen zu können. Der entscheidende Vorteil des Überlagerungsempfängers gegenüber dem Geradeausempfänger liegt genau in dieser konstanten Zwischenfrequenz: Die Filterung des Signals kann optimal auf eine feste Frequenz abgestimmt werden, wodurch eine sehr hohe Selektivität, also Trennschärfe, erreicht wird.

---

Da die Filter nicht abstimmbar sein müssen, können sie hinsichtlich Bandbreite und Flankensteilheit gezielt optimiert werden, etwa durch den Einsatz von Quarz-, Keramik- oder digitalen Filtern. So lassen sich beispielsweise für Sprachübertragung (SSB) Filter mit einer Bandbreite von etwa $\qty{2,4}{\kilo\hertz}$ und für Telegrafie (CW) schmalbandige Filter mit etwa $\qty{300}{\hertz}$ einsetzen. Auch für andere Übertragungsverfahren wie AM, FM oder digitale Modi können entsprechend angepasste Filter verwendet werden.

Durch dieses Konzept erreicht der Überlagerungsempfänger eine deutlich höhere Trennschärfe als der Geradeausempfänger. Ein weiterer Vorteil besteht darin, dass alle nachfolgenden Baugruppen stets mit derselben Zwischenfrequenz arbeiten und daher ebenfalls nicht abstimmbar ausgeführt werden müssen, was den Aufbau vereinfacht und die Empfangsqualität verbessert.

[question:EF102]

Überlagerungsempfänger können mit einer oder mehreren Zwischenfrequenzen arbeiten. Im einfachsten Fall handelt es sich um einen Direktüberlagerungsempfänger, bei dem die Zwischenfrequenz die gewünschte NF-Frequenz ist. Zu diesem Zweck muss die Oszillatorfrequenz sehr nahe an der Empfangsfrequenz liegen.

[question:EF208]

Ein Überlagerungsempfänger hat jedoch auch einige Nachteile, insbesondere das Auftreten sogenannter Spiegelfrequenzen. Diese Problematik sowie fortgeschrittene Empfängerkonzepte wie der Mehrfachsuper mit mehreren Zwischenfrequenzen werden wir erst in der Klasse A genauer behandeln.

<indepth>
Der Erfinder des Überlagerungsempfängers lässt sich nicht eindeutig benennen. Dies liegt unter anderem daran, dass seine Entwicklung in die Zeit des Ersten Weltkriegs fällt, in der alle beteiligten Kriegsparteien intensiv an der Verbesserung der Funk- und Radiotechnik arbeiteten. Unabhängig voneinander beschäftigten sich um das Jahr 1918 mehrere Forscher mit diesem Funktionsprinzip, darunter Edwin Armstrong in den USA, Lucien Lévy in Frankreich sowie Walter Schottky in Deutschland.
  
Der Begriff Heterodyn beziehungsweise Superheterodyn ist eine Wortneubildung. Er setzt sich aus dem lateinischen super („über“) sowie den griechischen Wörtern hetero („verschieden“) und dynamis („Kraft“ bzw. „Wirkung“) zusammen. Der Name beschreibt das grundlegende Funktionsprinzip des Überlagerungsempfängers: die Mischung zweier Signale unterschiedlicher Frequenz zur Erzeugung einer neuen Frequenz.
</indepth>