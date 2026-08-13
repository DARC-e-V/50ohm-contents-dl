Bei der Phasenumtastung (Phase-Shift Keying, PSK) werden die verschiedenen Symbole durch unterschiedliche Phasenlagen eines Trägers dargestellt. Die Amplitude und die Frequenz des Trägers bleiben dabei gleich. Beim Wechsel von einem Symbol zum nächsten kann sich dagegen die Phasenlage ändern.

Die Abbildung [ref:a_psk] zeigt ein PSK-Signal im zeitlichen Verlauf. An den Symbolgrenzen erkennt man, dass die Schwingung mit einer anderen Phasenlage fortgesetzt wird.

<margin>
[picture:705:a_psk:Phasenumtastung (Phase-Shift Keying)]
</margin>

---

Die einfachste Form ist die binäre Phasenumtastung (Binary Phase-Shift Keying, BPSK). Dabei stehen zwei verschiedene Phasenlagen und damit zwei mögliche Symbole zur Verfügung. Beispielsweise können die Phasenlagen $\qty{0}{\degree}$ und $\qty{180}{\degree}$ verwendet und den Bitwerten $0$ und $1$ zugeordnet werden. Die Abbildung [ref:a_psk_mapping] zeigt ein mögliches Mapping der beiden Bitwerte auf die beiden BPSK-Symbole.

Da sich die beiden Symbole nur durch ihre Phasenlage unterscheiden und ihre Amplitude gleich ist, liegen die beiden Punkte im Konstellationsdiagramm gegenüberliegend auf einem Kreis.

<margin>
[picture:1101:a_psk_mapping:BPSK im Konstellationsdiagramm]
</margin>

<indepth>
Genaugenommen kann BPSK mit den Winkeln $\qty{0}{\degree}$ und $\qty{180}{\degree}$ auch als ein ASK-Verfahren betrachtet werden, bei dem die Amplitude des Trägersignals zwischen einem negativen und einem positiven Wert umgeschaltet wird. Eine Multiplikation mit $-1$ resultiert bei einem Sinus-Signal zu einer Phasenverschiebung um $\qty{180}{\degree}$:

$-\sin(\omega t)=\sin(\omega t+\qty{180}{\degree})$

Dies ist ein Spezialfall. Es wären übrigens auch andere Phasenwinkel wie z. B. $\qty{90}{\degree}$ und $\qty{270}{\degree}$ möglich, deren beide Symbolphasen ebenfalls um $\qty{180}{\degree}$ voneinander getrennt wären.
</indepth>

[question:AE401]

---

Mit mehr als zwei unterschiedlichen Phasenlagen können entsprechend mehr Symbole dargestellt werden. Dadurch lassen sich mehrere Bits zu einem Symbol zusammenfassen.

---

Bei der Quadraturphasenumtastung (Quadrature Phase-Shift Keying, QPSK) stehen vier unterschiedliche Phasenlagen und damit vier mögliche Symbole zur Verfügung. Da es vier mögliche Bitkombinationen aus zwei Bits gibt, können mit jedem Symbol zwei Bits übertragen werden.

Zum Vergleich:

* BPSK: $\num{2}$ Symbole → $\num{1}$ Bit pro Symbol
* QPSK: $\num{4}$ Symbole → $\num{2}$ Bit pro Symbol
* 8-PSK: $\num{8}$ Symbole → $\num{3}$ Bit pro Symbol

[question:AE402]

Schauen wir uns QPSK nun im Konstellationsdiagramm an. Die vier möglichen Symbole besitzen die gleiche Amplitude, unterscheiden sich aber durch ihre Phasenlage. Deshalb liegen alle vier Signalpunkte auf einem Kreis. Die Abbildung [ref:a_qpsk] zeigt ein mögliches Mapping der vier Bitkombinationen $00$, $01$, $10$ und $11$ auf die vier QPSK-Symbole.

<margin>
[picture:1059:a_qpsk:I/Q-Diagramm für ein QPSK-Mapping]
</margin>

---

In diesem Beispiel werden folgende Phasenlagen verwendet:

* $11$ entspricht $\qty{45}{\degree}$
* $01$ entspricht $\qty{135}{\degree}$
* $00$ entspricht $\qty{225}{\degree}$
* $10$ entspricht $\qty{315}{\degree}$

<margin>
Das folgende Applet veranschaulicht die digitale QPSK-Modulation. In einem echten System wird das Signal durch Rauschen und andere Störungen beeinflusst. Dadurch liegen die empfangenen Signalpunkte nicht exakt auf den idealen Positionen, sondern weichen sowohl in ihrer Amplitude als auch in ihrer Phase davon ab. Das Applet simuliert dies, indem es Rauschen hinzufügt. Die Kreuze markieren die vier idealen QPSK-Symbole. Jeder farbige Punkt ist ein verrauschter Empfangswert. Der Empfänger ordnet ihn dem nächstgelegenen Symbol zu. Die farbig hinterlegten Bereiche sind die Entscheidungsbereiche des Empfängers. Solange ein verrauschter Empfangswert im Bereich des ursprünglich gesendeten Symbols liegt, wird es richtig erkannt. Überschreitet ein Punkt durch starkes Rauschen eine Grenze zu einem benachbarten Bereich, entscheidet sich der Empfänger für das falsche Symbol. Durch Kanalkodierung können diese Fehler jedoch korrigiert werden. Damit beschäftigen wir uns in einem späteren Abschnitt.

[include:applet_qpsk]
</margin>

Die vier Phasenlagen sind jeweils um $\qty{90}{\degree}$ gegeneinander versetzt. Der Empfänger kann anhand der erkannten Phasenlage bestimmen, welches Symbol und damit welche Bitkombination übertragen wurde.

Die Zuordnung der Bitkombinationen zu den einzelnen Phasenlagen ist nicht eindeutig festgelegt. Entscheidend ist zunächst nur, dass jedem Symbol eine eindeutige Bitkombination zugeordnet wird.

In der Praxis wird das Mapping häufig so gewählt, dass sich die Bitkombinationen benachbarter Signalpunkte nur in einem Bit unterscheiden. Eine solche Zuordnung wird als *Gray-Code* bezeichnet. Wird durch Rauschen versehentlich ein benachbarter Signalpunkt erkannt, führt dies dadurch häufig nur zu einem einzelnen Bitfehler.

Das Konstellationsdiagramm macht damit einen wesentlichen Unterschied zwischen ASK und PSK unmittelbar sichtbar: Bei ASK unterscheiden sich die Symbole durch ihren Abstand vom Ursprung und liegen in der Regel nur auf der positiven I-Achse, bei PSK dagegen durch ihren Winkel. Bei PSK liegen die Signalpunkte daher bei gleicher Amplitude auf einem Kreis.
