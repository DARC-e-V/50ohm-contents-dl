## Phasenumtastung (PSK)

* Digitales Modulationsverfahren zur Datenübertragung
* Die Symbole werden durch unterschiedliche Phasenlagen eines Trägers dargestellt
* Amplitude und Frequenz des Trägers bleiben bei idealer PSK gleich
* Beim Wechsel des Symbols kann sich die Phasenlage ändern

--- style="font-size: smaller;"

## PSK in der Zeitdarstellung

<left>
[picture:705:a_psk:Phasenumtastung (Phase-Shift Keying)]
</left>
<right>
* Die Amplitude bleibt konstant
* Die Information steckt in der *Phasenlage*
* Beim Wechsel zwischen zwei Symbolen kann sich die Phase sprunghaft ändern
* Wird dasselbe Symbol erneut übertragen, bleibt auch die Phasenlage gleich
</right>

--- style="font-size: smaller;"

## Binäre Phasenumtastung (BPSK)

<left>
[picture:1101:a_psk_mapping:BPSK im Konstellationsdiagramm]
</left>
<right>
* Zwei verschiedene Phasenlagen
* Zwei mögliche Symbole
* Damit kann $\num{1}$ Bit pro Symbol übertragen werden
* Beispiel: $\qty{0}{\degree}$ → $0$ und $\qty{180}{\degree}$ → $1$
* Die beiden Signalpunkte liegen sich im Konstellationsdiagramm gegenüber
</right>

<note>
Die einfachste Form der Phasenumtastung ist BPSK. Die beiden möglichen Symbole besitzen die gleiche Amplitude, ihre Phasen unterscheiden sich aber um 180 Grad.

Randbemerkung: Mathematisch lässt sich BPSK auch dadurch erzeugen, dass der Träger abhängig vom Bitwert mit +1 oder -1 multipliziert wird. Die Multiplikation mit -1 entspricht einer Phasenverschiebung um 180 Grad:

$-\sin(\omega t)=\sin(\omega t+\qty{180}{\degree})$

Die Wahl von 0 Grad und 180 Grad ist dabei nicht zwingend. Ebenso wären beispielsweise 90 Grad und 270 Grad möglich.
</note>

---

[question:AE401]

---

## Mehr Phasenlagen – mehr Symbole

* Mit mehr Phasenlagen können mehr unterschiedliche Symbole dargestellt werden
* Dadurch lassen sich mehrere Bits zu einem Symbol zusammenfassen

<fragment>
* *BPSK*: $\num{2}$ Symbole → $\num{1}$ Bit pro Symbol
* *QPSK*: $\num{4}$ Symbole → $\num{2}$ Bit pro Symbol
* *8-PSK*: $\num{8}$ Symbole → $\num{3}$ Bit pro Symbol
</fragment>

---

[question:AE402]

---

## Quadraturphasenumtastung (QPSK)

* QPSK verwendet vier verschiedene Phasenlagen
* Damit stehen vier verschiedene Symbole zur Verfügung
* Jeweils zwei Bits werden zu einem Symbol zusammengefasst: $00$, $01$, $10$, $11$
* Mit jedem QPSK-Symbol werden somit $\num{2}$ Bits übertragen

--- style="font-size: smaller;"

## QPSK im Konstellationsdiagramm

<left>
[picture:1059:a_qpsk:I/Q-Diagramm für ein QPSK-Mapping]
</left>
<right>
In diesem Beispiel gilt:

* $11$ → $\qty{45}{\degree}$
* $01$ → $\qty{135}{\degree}$
* $00$ → $\qty{225}{\degree}$
* $10$ → $\qty{315}{\degree}$

<fragment>
* Alle Signalpunkte besitzen die gleiche Amplitude
* Die Phasenlagen sind jeweils um $\qty{90}{\degree}$ gegeneinander versetzt
* Die vier Punkte liegen auf einem Kreis
</fragment>
</right>

<note>
Die Zuordnung der Bitkombinationen zu den einzelnen Phasenlagen ist nicht grundsätzlich festgelegt. Sender und Empfänger müssen jedoch dasselbe Mapping verwenden.

Das hier verwendete Mapping entspricht auch der Darstellung im Lehrtext und im folgenden Applet.
</note>

--- style="font-size: smaller;"

## Gray-Code bei QPSK

<left>
[picture:1059:a_qpsk_gray:I/Q-Diagramm für ein QPSK-Mapping]
</left>
<right>
* Benachbarte Symbole unterscheiden sich jeweils nur in *einem Bit*
* Eine solche Zuordnung nennt man *Gray-Code*

<fragment>
Beispiel:

$11 \leftrightarrow 01 \leftrightarrow 00 \leftrightarrow 10$
</fragment>

<fragment>
Wird durch Rauschen versehentlich ein benachbartes Symbol erkannt, entsteht dadurch häufig nur ein einzelner Bitfehler.
</fragment>
</right>

<note>
Das Mapping ist so gewählt, dass sich benachbarte Punkte im Konstellationsdiagramm nur in einem Bit unterscheiden.

Beim Übergang von 11 zu 01 ändert sich beispielsweise nur das erste Bit. Gleiches gilt für die übrigen benachbarten Signalpunkte, einschließlich 10 und 11.
</note>

--- style="font-size: smaller;"

<left>
[include:applet_qpsk]
</left>

<right>
### QPSK bei Rauschen
* Rauschen verändert Amplitude und Phase des empfangenen Signals
* Empfangswerte streuen um die idealen QPSK-Symbole
* Der Empfänger entscheidet sich für das nächstgelegene Symbol
* Wird eine Entscheidungsgrenze überschritten, entsteht ein Symbolfehler
</right>

<note>
Das Applet zeigt nicht nur die idealen QPSK-Symbole, sondern auch die Situation am Empfänger.

Die Kreuze markieren die vier idealen Signalpunkte. Die kleinen farbigen Punkte stellen verrauschte Empfangswerte dar. Durch Rauschen und andere Störungen ändern sich sowohl die Amplitude als auch die Phase des empfangenen Signals.

Die farbig hinterlegten Bereiche sind die Entscheidungsbereiche des Empfängers. Der Empfänger ordnet einen Empfangswert dem nächstgelegenen idealen Symbol zu.

Solange ein verrauschter Punkt im Entscheidungsbereich des ursprünglich gesendeten Symbols liegt, wird das Symbol richtig erkannt. Überschreitet der Punkt durch starkes Rauschen eine Entscheidungsgrenze, wird stattdessen ein anderes Symbol erkannt.

Mit „Erneut übertragen“ wird derselbe Bitstrom nochmals mit neuem Rauschen übertragen. Dadurch kann man gut erkennen, dass trotz gleicher gesendeter Symbole jedes Mal etwas andere Empfangswerte entstehen.

Mit zunehmendem Rauschen steigt die Wahrscheinlichkeit für Symbol- und damit Bitfehler. Durch geeignete Kanalkodierung können viele solcher Fehler erkannt und korrigiert werden.
</note>

---

## ASK und PSK im Konstellationsdiagramm

* Bei *ASK* unterscheiden sich die Symbole hauptsächlich durch ihre Amplitude
  * unterschiedlicher Abstand vom Ursprung
  * gleiche Phasenlage
* Bei *PSK* unterscheiden sich die Symbole durch ihre Phasenlage
  * gleicher Abstand vom Ursprung
  * unterschiedlicher Winkel
* Bei PSK liegen die Signalpunkte daher bei gleicher Amplitude auf einem Kreis.
