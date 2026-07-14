Die Frequenz eines Oszillators ist stets von der Umgebungstemperatur abhängig, da sich die Eigenschaften der verwendeten Bauelemente mit der Temperatur verändern. Bei Transistoren und Dioden betrifft dies beispielsweise den Verstärkungsfaktor, die Schwellspannung und die Kapazitäten. Auch passive Bauelemente wie Kondensatoren, Widerstände und insbesondere Schwingquarze weisen temperaturabhängige elektrische Eigenschaften auf.

Um die Frequenz eines Oszillators möglichst stabil zu halten, sollte er im Gerät gut von anderen Wärme- und Kältequellen möglichst thermisch abgeschirmt werden. Dies kann z.B. durch einen möglichst großen Abstand zu internen und externen Wärme- und Kältequellen sowie Luftströmungen erfolgen. Zudem ist ein Quarzoszillator gegenüber einem RC-, LC- oder VCO-Oszillator vorzuziehen, da er aufgrund der hohen Güte des Quarzes eine deutlich höhere Frequenzstabilität aufweist.

[question:AF215]

Es gibt verschiedene arten von Quarzoszillatoren, die sich in ihrer Frequenzstabilität unterscheiden:

* Der einfachste Quarzoszillator (vgl. Abbildung [ref:a_xo]) wird als *XO* bezeichnet, kurz für Crystal Oscillator.
* Ein *TCXO* (Temperature Compensated Crystal Oscillator) gleicht Temperatureinflüsse durch zusätzliche Bauelemente in der Oszillatorschaltung aus, sodass sich deren temperaturabhängige Effekte innerhalb des üblichen Betriebstemperaturbereichs weitgehend gegenseitig kompensieren.
* Ein *OCXO* (Oven-Controlled Crystal Oscillator) stabilisiert die Temperatur des Quarzoszillators mithilfe einer geregelten Heizung. Dazu befindet sich der Oszillator in einem thermisch isolierten Gehäuse, das ihn weitgehend vor äußeren Wärme- und Kälteeinflüssen schützt. Von den genannten Oszillatortypen bietet der OCXO die höchste Frequenzstabilität. 

<margin>
[photo:333:a_xo:XO Quarzoszillator mit $\qty{433,75}{\mega\hertz}$]
[photo:337:a_ocxo:OCXO Quarzoszillator mit $\qty{10}{\mega\hertz}$]
</margin>

[question:AD602]
[question:AD603]
[question:AD605]

Insbesondere beim Betrieb auf hohen Frequenzen ist die Frequenzstabilität des Referenzoszillators von Transceivern, Transvertern und Konvertern bei Nutzung von Übertragungsverfahren, die empfindlich auf Frequenzabweichungen reagieren, sehr wichtig. Zum Erreichen der hohen Ausgangs- oder Empfangsfrequenzen findet geräteintern eine Frequenzvervielfachung des Referenzoszillators statt. Hierdurch wirken sich Frequenzabweichungen des Referenzoszillators multiplikativ auf die Sende- oder Empfangsfrequenzen aus, was zu hohen Frequenzabweichungen und Frequenzinstabilitäten (z.B. Wandern des Sende- oder Empfangssignals) führen kann. Daher sollte z. B. auf dem $\qty{3}{\centi\meter}$-Band bzw. $\qty{10}{\giga\hertz}$-Band mindestens ein TCXO verwendet werden.

[question:AD604]