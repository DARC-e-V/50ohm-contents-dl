Bei der Digitalisierung eines analogen Signals müssen zwei Eigenschaften betrachtet werden: Zu welchen Zeitpunkten wird das Signal gemessen und mit welcher Genauigkeit können die gemessenen Werte dargestellt werden? Die beiden dazugehörigen Schritte werden als *Sampling* und *Quantisierung* bezeichnet.

Die Begriffe *zeitkontinuierlich*, *zeitdiskret*, *wertkontinuierlich* und *wertdiskret* beschreiben dabei zwei voneinander unabhängige Eigenschaften eines Signals. Einerseits kann betrachtet werden, ob das Signal zu jedem beliebigen Zeitpunkt definiert ist. Andererseits kann betrachtet werden, ob es beliebige Werte annehmen kann.

Ein ideales analoges Signal ist sowohl *zeitkontinuierlich* als auch *wertkontinuierlich*. Es ist zu jedem beliebigen Zeitpunkt definiert und kann innerhalb seines Wertebereichs beliebige Zwischenwerte annehmen. Ein solches Signal zeigt die Abbildung [ref:a_wertkont_zeitkont].

---

Analoge Signale besitzen keine kleinste zeitliche Auflösung und sind zeitlich fortlaufend. Sie werden daher als *zeitkontinuierlich* bezeichnet. Beim Sampling wird ein solches Signal dagegen nur zu bestimmten Zeitpunkten gemessen, also abgetastet. Die einzelnen Abtastwerte bezeichnet man als *Samples*.

Die Samples stellen jeweils nur den Momentanzustand des Signals zum Zeitpunkt der Abtastung dar. Zwischen zwei Abtastzeitpunkten kann sich das analoge Signal weiter verändern. Da nach dem Sampling nur noch einzelne, zeitlich voneinander getrennte Werte vorliegen, bezeichnet man das abgetastete Signal als *zeitdiskret*.

Die Abbildung [ref:a_wertkont_zeitdisk] zeigt ein solches ideal abgetastetes Signal. Es ist *zeitdiskret*, da nur zu bestimmten Abtastzeitpunkten Werte vorliegen. Die einzelnen Samples können zunächst jedoch noch beliebige Werte annehmen und sind daher *wertkontinuierlich*.

<margin>
[picture:408:a_wertkont_zeitkont:Wert- und Zeitkontinuierliches Signal]
[picture:409:a_wertkont_zeitdisk:Wertkontinuierliches und Zeitdiskretes Signal]
</margin>

[question:AF601]
[question:AF603]

Den Vorgang, bei dem ein zeitkontinuierliches Signal zu bestimmten Zeitpunkten abgetastet und dadurch in ein zeitdiskretes Signal überführt wird, bezeichnet man als *Sampling*.

[question:AF606]

Die Geschwindigkeit, mit der die Abtastung eines analogen Signals vorgenommen wird, wird als *Samplingrate* oder *Abtastrate* bezeichnet. Sie gibt an, wie viele Samples pro Zeiteinheit, beispielsweise pro Sekunde, aufgenommen werden.

Analoge Tonsignale werden bei digitalen Datenträgern wie CDs beispielsweise mit einer Samplingrate von $\num{44100}$ Samples pro Sekunde abgetastet. Dies entspricht $\qty{44,1}{\kilo\sps}$.

[question:AF615]

---

Neben der zeitlichen Auflösung spielt bei der Digitalisierung auch die Auflösung der gemessenen Werte eine Rolle. Analoge Signale können beliebige Spannungswerte annehmen und zwischen diesen ohne feste Zwischenstufen variieren. Man bezeichnet sie deshalb als *wertkontinuierlich*.

Bei der Digitalisierung steht dagegen nur eine begrenzte Anzahl möglicher Zahlenwerte zur Verfügung. Ein gemessener Spannungswert muss daher einer dieser festen Stufen zugeordnet werden. Das Signal ist danach *wertdiskret*.

Liegt ein analoger Signalwert zwischen zwei möglichen Stufen, muss entschieden werden, welcher Stufe der gemessene Wert zugeordnet wird. Diesen Vorgang bezeichnet man als *Quantisierung*. Das zuvor wertkontinuierliche Signal wird dabei auf eine endliche Anzahl möglicher Werte abgebildet.

Die Abbildung [ref:a_wertdisk_zeitkont] zeigt zur Veranschaulichung ein *wertdiskretes, aber zeitkontinuierliches Signal*. Das Signal ist weiterhin zu jedem Zeitpunkt definiert, kann jedoch nur bestimmte, fest vorgegebene Werte annehmen. Die möglichen Werte sind also bereits quantisiert, die Zeit hingegen noch nicht diskretisiert.

Werden Sampling und Quantisierung miteinander kombiniert, entsteht ein *wert- und zeitdiskretes Signal*, wie es in Abbildung [ref:a_wertdisk_zeitdisk] dargestellt ist. Es liegen nur zu bestimmten Zeitpunkten Samples vor, und auch deren mögliche Werte sind auf feste Stufen beschränkt. Dies entspricht der digitalen Darstellung eines zuvor analogen Signals.

<tip>
Zur Veranschaulichung kann man einen analogen Dimmer mit einem Stufenschalter vergleichen. Mit einem analogen Dimmer lässt sich die Helligkeit einer Lampe beliebig fein einstellen. Mit einem Stufenschalter mit beispielsweise $\num{5}$ Stufen stehen dagegen nur $\num{5}$ verschiedene Helligkeitswerte zur Verfügung. Zwischenwerte sind nicht möglich.

Soll eine mit dem analogen Dimmer eingestellte Helligkeit mit dem Stufenschalter nachgebildet werden, muss die am besten passende Stufe gewählt werden. Genau dies entspricht dem Prinzip der Quantisierung: Ein kontinuierlicher Wert wird einem von mehreren fest vorgegebenen Werten zugeordnet.
</tip>

<margin>
[picture:410:a_wertdisk_zeitkont:Wertdiskretes und Zeitkontinuierliches Signal]
[picture:411:a_wertdisk_zeitdisk:Wert- und Zeitdiskretes Signal]
</margin>

[question:AF602]
[question:AF604]
[question:AF605]

<indepth>
Hier gibt es die Möglichkeit das Ganze nochmal auszuprobieren. Ein zeitkontinuierliches Sinus-Signal wird von einem AD-Umsetzer digitalisiert und anschließend wieder von einem DA-Umsetzer in ein analoges Signal gewandelt. An den Reglern kann man die Zeitquantisierung und die Wertquantisierung der AD/DA-Umsetzer einstellen.

[include:quantisierung_und_sampling]
</indepth>