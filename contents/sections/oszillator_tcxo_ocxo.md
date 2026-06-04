Oszillatoren haben, bedingt durch die Temperaturabhängigkeit der in ihnen verwendeten Bauelemente, immer eine Abhängigkeit der erzeugten Frequenz von der Umgebungstemperatur. Transistoren und Dioden haben eine relativ starke Abhängigkeit ihrer Kennlinie und Charakteristik von der Umgebungstemperatur (Verstärkungsfaktor, Schwellspannung, Kapazitäten). Ebenso sind auch die elektrischen Parameter passiver Bauelemente wie Kondensatoren, Widerstände und insbesondere Schwingquarze von deren Umgebungstemperatur abhängig.
Um Oszillatoren in ihrer Frequenz möglichst stabil zu halten, gibt es verschiedene technische und physikalische Möglichkeiten:
1. Alle Oszillatoren sollten immer möglichst gut thermisch isoliert zu anderen Wärmequellen in Geräten sein.
2. Anstelle eines RC-, LC- oder VCO-Oszillators ist ein Quarzoszillator vorzuziehen, da dieser wesentlich frequenzstabiler aufgrund der hohen Güte (Q) des Quarzes ist. Diesen Oszillator-Typ nennt man *XO* - Crystal oscillator. 
3. Verwendung eines Quarzoszillators und Kompensation von thermischen Einflüssen durch Einsatz von Bauelementen in der Oszillatorschaltung, so dass sich Temperatureinflüsse im Bereich der üblichen Betriebstemperatur gegenseitig kompensieren. Diesen Oszillator-Typ nennt man *TCXO* - Temperature compensated crystal oscillator
4. Künstliche Stabilisierung der Umgebungstemperatur eines Quarzoszillators durch eine Temperaturregelung mittels Thermostatschaltung und Einbau in ein thermisch isoliertes Gehäuse sowie Isolation gegenüber externen Wärme- und Kältequellen. Diesen Oszillator-Typ nennt man *OCXO* - Oven controlled crystal oscillator. Der OCXO hat gegenüber den anderen Oszillatortypen die höchste Frequenzstabilität.

Grundsätzlich sollten frequenzstabile Oszillatoren immer gegenüber geräteinternen und externen Wärme- und Kältequellen möglichst gut thermisch isoliert sein. Dies kann z.B. durch einen möglichst großen Abstand zu internen und externen Wärme- und Kältequellen sowie Luftströmungen erfolgen.

[question:AF215]
[question:AD602]
[question:AD603]
[question:AD605]

Insbesondere beim Betrieb auf hohen Frequenzen ist die Frequenzstabilität des Referenzoszillators von Transceivern, Transvertern und Konvertern bei Nutzung von Betriebsarten, die empfindlich auf Frequenzabweichungen reagieren, sehr wichtig. Zum Erreichen der hohen Ausgangs- oder Empfangsfrequenzen findet geräteintern eine Frequenzvervielfachung des Referenzoszillators statt. Hierdurch wirken sich Frequenzabweichungen des Referenzoszillators multiplikativ auf die Sende- oder Empfangsfrequenzen aus, was zu hohen Frequenzabweichungen und Frequenzinstabilitäten (z.B. Wandern des Sende- oder Empfangssignals) führen kann.
Daher sollte immer der beste zur Auswahl stehende Oszillatortyp verwendet werden (z.B. TCXO oder OCXO).

[question:AD604]