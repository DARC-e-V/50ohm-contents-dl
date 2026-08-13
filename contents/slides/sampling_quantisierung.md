## Sampling und Quantisierung

Bei der Digitalisierung eines analogen Signals müssen zwei Eigenschaften betrachtet werden:

* **Wann** wird das Signal gemessen?
  * Sampling
  * zeitkontinuierlich → zeitdiskret
* **Wie genau** wird der gemessene Wert dargestellt?
  * Quantisierung
  * wertkontinuierlich → wertdiskret

<note>
Sampling und Quantisierung sind zwei unterschiedliche Schritte.

Beim Sampling wird die Zeitachse diskretisiert: Wir betrachten das Signal nur noch zu bestimmten Abtastzeitpunkten.

Bei der Quantisierung wird dagegen die Wertachse diskretisiert: Ein gemessener Wert wird einer von endlich vielen möglichen Stufen zugeordnet.
</note>

---

## Analoges Signal

[picture:408:a_wertkont_zeitkont:Wert- und Zeitkontinuierliches Signal]

* Zu jedem beliebigen Zeitpunkt ist ein Signalwert vorhanden
* Der Signalwert kann beliebige Zwischenwerte annehmen
* Ein ideales analoges Signal ist daher *zeit-* und *wertkontinuierlich*

--- style="font-size: smaller;"

## Sampling

<left>
[picture:408:a_wertkont_zeitkont:Wert- und Zeitkontinuierliches Signal]
</left>
<right>
[picture:409:a_wertkont_zeitdisk:Wertkontinuierliches und Zeitdiskretes Signal]
</right>

<fragment>
* Das Signal wird nur zu bestimmten Zeitpunkten abgetastet
* Die einzelnen Abtastwerte heißen *Samples*
* Aus einem zeitkontinuierlichen Signal wird ein *zeitdiskretes* Signal
* Die Werte selbst können zunächst weiterhin beliebige Werte annehmen
</fragment>

<note>
Beim idealisierten Sampling verändert sich zunächst nur die Zeitachse.

Vor dem Sampling ist das Signal zu jedem Zeitpunkt definiert. Danach liegen nur noch zu bestimmten Abtastzeitpunkten Werte vor.

Die einzelnen Samplewerte müssen an dieser Stelle noch nicht quantisiert sein. Deshalb ist das Signal rechts zeitdiskret, aber noch wertkontinuierlich.
</note>

---

[question:AF601]

---

[question:AF603]

---

## Sampling

* Der Vorgang der zeitlichen Abtastung wird als *Sampling* bezeichnet
* Die einzelnen Abtastwerte heißen *Samples*
* Zwischen zwei Samples kann sich das analoge Signal weiter verändern

<fragment>
Sampling bedeutet somit:

**zeitkontinuierlich → zeitdiskret**
</fragment>

---

[question:AF606]

---

## Samplingrate

* Die *Samplingrate* oder *Abtastrate* gibt an, wie viele Samples pro Zeiteinheit aufgenommen werden
* Einheit: Samples pro Sekunde

<fragment>
Beispiel Audio-CD:

$\num{44100}$ Samples pro Sekunde

entsprechen

$\qty{44,1}{\kilo\sps}$
</fragment>

<note>
Je höher die Samplingrate ist, desto kleiner ist der zeitliche Abstand zwischen zwei aufeinanderfolgenden Samples.

Welche Samplingrate mindestens erforderlich ist, behandeln wir anschließend beim Abtasttheorem.
</note>

---

[question:AF615]

---

## Quantisierung

* Analoge Signalwerte können beliebige Zwischenwerte annehmen: *wertkontinuierlich*
* Digital stehen nur endlich viele mögliche Werte zur Verfügung: *wertdiskret*
* Ein Messwert muss einer der verfügbaren Stufen zugeordnet werden

<fragment>
Diesen Vorgang bezeichnet man als *Quantisierung*.
</fragment>

<note>
Nach dem Sampling wissen wir, zu welchen Zeitpunkten wir das Signal betrachten.

Nun müssen wir noch entscheiden, mit welchem digitalen Zahlenwert der jeweils gemessene analoge Wert dargestellt werden soll.

Liegt der tatsächliche Wert zwischen zwei möglichen Stufen, wird er einer geeigneten Stufe zugeordnet.
</note>

--- style="font-size: smaller;"

## Wertkontinuierlich und wertdiskret

<left>
[picture:410:a_wertdisk_zeitkont:Wertdiskretes und Zeitkontinuierliches Signal]
</left>
<right>
[picture:411:a_wertdisk_zeitdisk:Wert- und Zeitdiskretes Signal]
</right>

* Links: Werte sind bereits diskret, die Zeit ist noch kontinuierlich
* Rechts: Werte und Zeit sind diskret

<fragment>
Durch die Kombination von **Sampling und Quantisierung** entsteht die digitale Darstellung eines analogen Signals.
</fragment>

<note>
Die linke Darstellung dient vor allem dazu zu zeigen, dass Zeitdiskretheit und Wertdiskretheit zwei unabhängige Eigenschaften sind.

Für die Digitalisierung besonders wichtig ist die rechte Darstellung: Nach Sampling und Quantisierung liegen nur noch einzelne Samples vor, die zusätzlich nur endlich viele mögliche Werte annehmen können.
</note>

---

[question:AF602]

---

[question:AF604]

---

[question:AF605]

---

## Praktisches Beispiel: Dimmer vs. Stufenschalter

* Ein analoger Dimmer erlaubt feine, stufenlose Helligkeitseinstellungen  
* Ein Stufenschalter (z. B. $\num{5}$ Stufen) ermöglicht nur feste Helligkeitswerte – Zwischenstufen sind nicht möglich
* Quantisierung: Auswahl der nächstpassenden Stufe, um den analogen Wert abzubilden

---
## Zusammenfassung

<left>
[include:quantisierung_und_sampling]
</left>
<right>
* Sampling bestimmt, **wann** ein Wert betrachtet wird
* Quantisierung bestimmt, **welcher digitale Wert** daraus wird
* Erst beide Schritte zusammen ergeben ein zeit- und wertdiskretes Signal
</right>

<note>
Mit dem Applet können Sampling und Quantisierung gemeinsam betrachtet werden.

Die Samplingrate beeinflusst den zeitlichen Abstand der Samples. Die Quantisierung bestimmt dagegen, welche möglichen Werte die Samples annehmen können.

Damit lassen sich die beiden zunächst unabhängigen Schritte noch einmal gemeinsam nachvollziehen.
</note>