<margin>
[picture:911:e_digitale_signalverarbeitung_blockschaltbild:Prinzip der digitalen Signalverarbeitung]
</margin>

In den letzten 25 Jahren hat sich die Welt technologisch massiv verändert. Die Rechenleistung von Computern hat um ein Vielfaches zugenommen, und immer mehr Aufgaben in technischen Geräten werden durch Mikrochips auf kleinstem Raum durchgeführt. Auch in den kommenden Jahren wird sich diese Entwicklung in einem rasanten Tempo weiter fortsetzen. Dies alles verändert die Art und Weise, wie Geräte, insbesondere auch die Signalverarbeitung in modernen Funkgeräten, realisiert ist. Digitale Signalverarbeitung ist mittlerweile Stand der Technik, und jedes moderne Gerät basiert auf dieser Technologie. Hierbei spielen insbesondere digitale Signalprozessoren und das Grundprinzip der digitalen Signalverarbeitung eine wesentliche Rolle.

Die digitale Signalverarbeitung ist hierbei nicht nur im Bereich der Funktechnik zu finden. Viele Geräte, seien es Handys, Stereoanlagen, bildgebende Systeme im medizinischen Bereich sowie praktisch alle modernen Funkapplikationen profitieren von dieser faszinierenden Technik und ermöglichen nie gekannte Möglichkeiten und Funktionen in diesen Geräten kostengünstig zu realisieren.

Im Bereich der Funktechnik spricht man bei Geräten, die mittels digitaler Signalverarbeitung Signale verarbeiten von sogenannten SDR-Geräten. In diesen Geräten ist zumindest ein Teil der Signalverarbeitung in Software realisiert.

[question:EF603]

Um kontinuierliche analoge Signale digital verarbeiten zu können, müssen diese zunächst mittels eines Analog-Digital-Umsetzers (A/D-Umsetzer) abgetastet und in digitale Werte umgesetzt werden. Man spricht hierbei von Digitalisierung des analogen Eingangssignals.

[question:EF602]

---
<margin>
[picture:411:e_digitale_signalverarbeitung:Einfache Darstellung einer Sinuswelle aus $\num{16}$ Samples und $\num{7}$ Werten]
</margin>

Hierbei wird das analoge Signal in festen Zeitintervallen abgetastet und in einem digitalen Wertebereich (z. B. von $\num{-128}$ bis $\num{+127}$) abgebildet. Jeder Wert repräsentiert eine bestimmte gemessene Signalspannung, wobei in der Regel negativen Werten negative Spannungen und positiven Werten positive Spannungen zugeordnet werden. Man kann sich das in etwa so vorstellen wie z.B. bei einer Filmkamera, die in festen Abständen Bilder einer Szene aufnimmt. Hierbei haben die aufgenommenen Bilder immer einen festen zeitlichen Abstand zum vorherigen und nächsten Bild und stellen die momentane Szene in zeitlich kleinen Abständen dar. Dieser Prozess nennt sich Sampling (in Deutsch könnten man dies mit dem Wort Probenahme übersetzen). Die einzelnen gemessenen Signalwerte werden als Samples bezeichnet. Im nächsten Abschnitt werden wir uns diesen Prozess noch etwas genauer ansehen.

Nach der A/D-Umsetzung können die als digitale Werte vorliegenden Samples mittels digitaler Signalverarbeitung beliebig weiter verarbeitet werden.

Im Anschluss an die digitale Signalverarbeitung wird man aus den digital verarbeiteten Signalen wieder ein analoges Signal z.B. für die Ausgabe über einen Lautsprecher oder für die Aussendung über eine Antenne machen wollen. Um die digitalen Werte wieder in ein analoges Signal zu verwandeln, benötigt man an dieser Stelle einen Digital-Analog-Umsetzer (D/A-Umsetzer), welcher praktisch das Gegenstück zum vorbeschriebenen A/D-Umsetzer darstellt. Der D/A-Umsetzer setzt digitale Werte wieder in analoge Spannungswerte um und ermöglicht somit die Rekonstruktion eines analogen Signals aus den digitalen Werten.

[question:EF601]