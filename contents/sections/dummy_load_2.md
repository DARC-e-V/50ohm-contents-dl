In der Klasse E haben wir die *Dummyload* bereits kennengelernt. Eine Dummyload ist ein Lastwiderstand, der die vom Sender abgegebene HF-Leistung in Wärme umsetzt. Sie ermöglicht es beispielsweise, einen Sender zu testen oder seine Ausgangsleistung zu bestimmen, ohne dass dabei ein Signal über eine Antenne abgestrahlt wird. In der Klasse A betrachten wir nun genauer, wie eine solche Dummyload aufgebaut werden kann.

Eine Dummyload für den HF-Bereich wird häufig aus mehreren einzelnen Widerständen zusammengesetzt. Dadurch lässt sich die entstehende Verlustleistung auf mehrere Bauteile verteilen und eine entsprechend hohe Gesamtbelastbarkeit erreichen. Die Widerstände können dabei parallel, in Reihe oder in einer Kombination aus Reihen- und Parallelschaltungen verbunden werden. Werden identische Widerstände mit gleicher Belastbarkeit verwendet und die Schaltung symmetrisch aufgebaut, verteilt sich die Verlustleistung gleichmäßig auf die einzelnen Widerstände. Die erforderliche Anzahl und Verschaltung der Widerstände kann mit den bekannten Regeln für Reihen- und Parallelschaltungen bestimmt werden. Bei einer HF-Dummyload ist außerdem wichtig, dass die Schaltung auch bei hohen Frequenzen möglichst einem rein ohmschen Widerstand von $\qty{50}{\ohm}$ entspricht. Deshalb werden geeignete, möglichst induktionsarme Widerstände verwendet und die Verbindungsleitungen möglichst kurz ausgeführt.

Abbildung [ref:dummy_load_aufbau1] zeigt eine fertig aufgebaute Dummyload von 50ohm.de. Hier werden beispielsweise $\num{20}$ Widerstände mit jeweils $\qty{1}{\kilo\ohm}$ parallel geschaltet. Für $n$ identische parallel geschaltete Widerstände gilt:

$R_\mathrm{ges} = \frac{R}{n}$

Damit ergibt sich:

$R_\mathrm{ges} = \frac{\qty{1}{\kilo\ohm}}{20} = \qty{50}{\ohm}$

<warning>
Die maximal mögliche Verlustleistung der gesamten Dummyload ergibt sich näherungsweise aus der Summe der Belastbarkeiten aller Widerstände, sofern sich die Leistung gleichmäßig auf sie verteilt. Da die 50ohm.de Dummyload über keine Kühlung verfügt und nicht geschirmt ist, sollte sie nur für QRP-Sender mit geringer Ausgangsleistung verwendet werden. Für höhere Leistungen ist eine Dummyload mit Kühlung und Schirmung erforderlich, die auch für den Dauerbetrieb geeignet ist!
</warning>

Die 50ohm.de Dummyload besitzt zusätzlich einen Spitzenwertgleichrichter aus einer Diode und einem Kondensator. Damit kann aus der anliegenden HF-Spannung eine Gleichspannung erzeugt werden, die beispielsweise mit einem Multimeter gemessen werden kann. Unter Berücksichtigung des Spannungsteilers und der Dioden-Durchlassspannung kann daraus die HF-Ausgangsleistung des Senders bestimmt werden.

[question:AI602]

<margin>
[photo:340:dummy_load_aufbau1:Die fertige 50ohm.de Dummyload]
[photo:341:dummy_load_aufbau2:Aufbau der 50ohm.de Dummyload]

*Anzeige:* Möchtest du auch eine coole 50ohm.de QRP-Dummyload bauen? Dann kannst du diese im [DARC-Verlag](https://darcverlag.de/50Ohm-Dummy-Load-DIY-Kit-Bausatz) als Bausatz bestellen.
</margin>

In der folgenden Prüfungsfrage besteht die Dummyload aus einer Kombination von Reihen- und Parallelschaltungen. Werden in jedem Zweig $N_\mathrm{S}$ gleiche Widerstände in Reihe geschaltet und anschließend $N_\mathrm{P}$ solcher Zweige parallel geschaltet, ergibt sich der Gesamtwiderstand zu:

$R_\mathrm{ges} = \frac{N_\mathrm{S}}{N_\mathrm{P}} \cdot R$

Die Anzahl aller verwendeten Widerstände beträgt dabei:

$n = N_\mathrm{S} \cdot N_\mathrm{P}$

Sind alle Widerstände gleich belastet, addieren sich ihre zulässigen Verlustleistungen. Damit lässt sich eine Dummyload mit dem gewünschten Widerstand und gleichzeitig hoher Belastbarkeit aufbauen.

[question:AI601]

Eine weitere Möglichkeit zur Bestimmung der HF-Ausgangsleistung besteht darin, die Dummyload mit einer Anzapfung ihres Widerstandsnetzwerks auszustatten. Befindet sich diese Anzapfung beispielsweise nahe dem Masseanschluss, liegt dort nur ein Teil der gesamten HF-Spannung an.

Die Widerstände bilden dabei einen Spannungsteiler. Ist dessen Teilungsverhältnis bekannt, kann aus der an der Anzapfung gemessenen HF-Spannung auf die gesamte Spannung an der Dummyload zurückgerechnet werden. Die Teilspannung kann beispielsweise mit einem HF-Tastkopf und einem digitalen Multimeter gemessen werden. Aus der so bestimmten Gesamtspannung lässt sich anschließend die HF-Leistung berechnen.

[question:AI603]