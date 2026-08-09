Dämpfungsglieder werden in der HF-Technik oft benötigt, um Signalpegel definiert abzuschwächen. Hierbei kann z.B. durch ein Leistungsdämpfungsglied die Ausgangsleistung eines Senders soweit reduziert werden, dass dessen Ausgangssignal die angeschlossenen Messgeräte nicht beschädigt oder übersteuert. Man verwendet Dämpfungsglieder auch um Eingangspegel für Verstärker und Empfänger auf ein definiertes Maß zu reduzieren.

Ein Dämpfungsglied muss hierbei immer für eine definierte Systemimpedanz bzgl. Ein- und Ausgang ausgelegt werden. Bei symmetrisch aufgebauten Dämpfungsgliedern sind die Ein- und Ausgangsimpedanzen identisch. Oft sind dies die in der HF-Technik üblichen $\qty{50}{\ohm}$. Damit ein Dämpfungsglied die geforderten Impedanzen an dessen Ein- und Ausgang zeigt ist ein impedanzrichtiger Abschluss auf beiden Seiten erforderlich. Dies wird durch ein geeignetes Widerstandsnetzwerk erreicht. 

Es gibt hierbei verschiedene Schaltungsvarianten, die sich in der Anordnung der Widerstände unterscheiden. Die beiden gängigsten Varianten sind das T- (vgl. Abbildung [ref:a_daempfungsglied_t]) und das $\pi$-Dämpfungsglied (vgl. Abbildung [ref:a_daempfungsglied_pi]). Bei beiden Varianten wird die Dämpfung durch ein Widerstandsnetzwerk erreicht, welches die eingespeiste Leistung in Wärme umwandelt.

<margin>
[picture:342:a_daempfungsglied_pi:Dämpfungsglied in PI-Konfiguration mit Quelle und Lastwiderstand]
</margin>

<margin>
[picture:341:a_daempfungsglied_t:Dämpfungsglied in T-Konfiguration mit Quelle und Lastwiderstand]
</margin>

[question:AD801]
[question:AD802]

---

Die Dämpfung eines Dämpfungsglieds wird üblicherweise in dB (Dezibel) angegeben und bezieht sich auf die Leistung. So bedeutet z. B. $\qty{20}{\dB}$ eine Dämpfung der Eingangsleistung um den Faktor $\num{100}$. Die Ausgangsleistung nach diesem Dämpfungsglied beträgt somit nur noch $\frac{1}{100}$ der Eingangsleistung was im Falle von $\qty{100}{\watt}$ Eingangsleistung einer Ausgangsleistung von $\qty{1}{\watt}$ entspricht.

Bei ohmschen Dämpfungsgliedern erfolgt die Dämpfung durch Umwandlung der eingespeisten Leistung in Wärme. Wird z.B. ein $\qty{100}{\watt}$-Signal wie vorher beschrieben um $\qty{20}{\dB}$ gedämpft so werden $\qty{99}{\watt}$ im Dämpfungsglied in Wärme umgesetzt. Die verbleibende Leistung von $\qty{1}{\watt}$ steht dann noch am Ausgang des Dämpfungsglieds zur Verfügung.

[question:AD806]
[question:AD803]
[question:AD804]
[question:AD805]

Ein symmetrisches Dämpfungsglied kann z.B. als T oder $\pi$-Netzwerk aus Widerständen aufgebaut werden. Die Namensgebung resultiert hierbei aus dem Erscheinungsbild der Widerstandsanordnung in der Schaltung.

<indepth>
Die Widerstandswerte für ein $\pi$-Dämpfungsglied für eine Impedanz von $\qty{50}{\ohm}$ können mit den folgenden Formeln berechnet werden:

$R_1 = R_3 = \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}+1}{10^{\frac{a}{20}}-1}\right)$

Dabei ist $a$ die gewünschte Dämpfung in $\unit{\dB}$.

$R_2 = \frac{\qty{50}{\ohm}}{2} \cdot \left( 10^{\frac{a}{20}} - \frac{1}{10^{\frac{a}{20}}}\right)$

Die Widerstandswerte für ein T-Dämpfungsglied für eine Impedanz von $\qty{50}{\ohm}$ können mit den folgenden Formeln berechnet werden:

$R_1 = R_2 = \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}-1}{10^{\frac{a}{20}}+1} \right)$

$R_3 = 2\cdot \qty{50}{\ohm} \cdot \left( \frac{10^{\frac{a}{20}}}{10^{\frac{a}{10}}-1} \right)$

<webonly>
[include:applet_daempfungsglied]
</webonly>

</indepth>


