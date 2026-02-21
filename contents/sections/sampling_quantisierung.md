Wie in den vorhergehenden Kapiteln erläutert, werden analoge Signale zunächst mittels Sampling in digitale Werte umgewandelt. Ein analoges Signal kann hierbei nur in bestimmten Abständen gemessen (man sagt auch abgetastet) werden. Die abgetasteten Werte stellen somit immer nur einen Momentanzustand im Zeitpunkt der Abtastung dar, und zwischen den einzelnen Abtastungsvorgängen kann sich das analoge Signal zeitlich gesehen beliebig verändern. Da analoge Signale keine kleinste zeitliche Auflösung besitzen und somit zeitlich fortlaufend sind, werden diese auch als zeitkontinuierlich bezeichnet. Im Gegensatz hierzu bezeichnet man Samples, die nur eine maximale, definierte zeitliche Auflösung eines Signals ermöglichen, als zeitdiskret, da es ein maximal mögliches und definierbares (somit diskretes) zeitliches Intervall zwischen den einzelnen gemessenen Werten gibt.

<indepth>
[include:quantisierung_und_sampling]
</indepth>

[question:AF601]
[question:AF603]

Sehen wir uns den Prozess des Samplings noch von einer anderen Seite her an. Analoge Signale können beliebige Spannungswerte annehmen und zwischen diesen ohne Zwischenstufen variieren. Da diese Änderungen bei analogen Signalen auch beliebig klein oder groß sein können, bezeichnet man diese Eigenschaft analoger Signale als wertkontinuierlich. Im Gegensatz hierzu stehen bei der Digitalisierung eines analogen Signals hinsichtlich der möglichen Werte (z. B. wie vorgenannte $\num{-128}$ bis $\num{+127}$) nur begrenzte Abstufungen für die Abbildung der gemessenen Spannungswerte zur Verfügung. Daher bezeichnet man digitale Samples in dieser Hinsicht auch als wertdiskret, da immer nur bestimmte Spannungswerte in Form von Spannungsstufen bei der Messung eines analogen Signalwertes zur Verfügung stehen. Wenn nun z.B. ein analoger Signalwert zwischen zwei Spannungsstufen liegt, so muss der A/D-Umsetzer eine Entscheidung treffen, zu welchem Signalwert der gemessene Wert eher tendiert. Diesen Prozess bezeichnet man auch als Quantisierung. Das zuvor kontinuierliche Signal wird hierbei in eine endliche Anzahl von Werten abgebildet.

Zur Veranschaulichung hier ein praktisches Beispiel anhand eines analogen Dimmers und eines Stufenschalters. Ist ein Dimmer mittels einer analogen Schaltung realisiert, kann man eine Lampe damit beliebig fein in deren Helligkeit steuern. Im Gegensatz hierzu könnte man die Lampe mit einem Stufenschalter mit z. B. $\num{5}$ Stufen nur jeweils auf $\num{5}$ Helligkeitswerte schalten - Zwischenstufen sind hierbei nicht möglich. Daher würde man diesen Stufenschalter auch als wertdiskret bezeichnen. Versucht man nun Helligkeitswerte, die man mit dem analogen Dimmer eingestellt hat, mittels des Stufenschalters nachzubilden, so ist man hier auf die festen vorgegebenen Stufen beschränkt. Man würde in diesem  Fall die passendste Einstellung am Stufenschalter wählen und somit eine Quantisierung des analogen Helligkeitswerts vornehmen.

[question:AF602]
[question:AF604]
