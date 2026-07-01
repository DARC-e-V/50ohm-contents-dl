Oszillatoren sind eines der wichtigsten Schaltungselemente im Amateurfunk. Sie sind sozusagen das Herz eines jeden Funkgerätes. Oszillatoren dienen der Erzeugung von hochfrequenten Schwingungen in Sendern und Empfängern. Hierbei gibt es verschiedene Möglichkeiten, Oszillatoren technisch zu realisieren.

---

<margin>
[include:applet_schwingkreis]
</margin>

Die einfachste Form eines Oszillators ist der sog. *LC-Oszillator*, der als frequenzbestimmende Elemente einen Schwingkreis (bestehend aus einer Spule und einem Kondensator), welchen wir im vorherigen Kapitel kennen gelernt haben, enthält.

[question:ED501]

LC-Oszillatoren haben den Nachteil, dass sich Ihre frequenzbestimmenden Komponenten (L und C) in Abhängigkeit von der Temperatur stark ändern können, was zu großen Frequenzabweichungen führen kann.

Laut Formelsammlung ist die Formel für die Schwingungsfrequenz (Thomsonsche Schwingkreisformel):

$ f_0 = \frac{1}{2\pi \sqrt{L\cdot C}} $

Die Frequenz eines LC-Oszillators ändert sich, wenn sich der Wert des Kondensators oder der Spule z.B. durch Temperatureinwirkung ändert. Wie sich das auf die Frequenz auswirkt, kann man in der Formel erkennen:
Bei *steigender* Kapazität des Kondensators oder steigender Induktivität der Spule *verringert sich die Frequenz* des Schwingkreises. Umgekehrt *steigt die Frequenz* des Schwingkreises bei *sinkender* Kapazität oder Induktivität.

[question:ED503]
[question:ED505]
[question:ED502]
[question:ED504]

Die Geschwindigkeit der Temperaturänderung bestimmt auch die Geschwindigkeit der Frequenzänderung eines Oszillators. Hierbei ändert sich jedoch die Frequenz nicht sprunghaft, da thermische Effekte immer einer gewissen Trägheit unterliegen. Daher ändert sich die Frequenz eines Oszillators, der schwankenden Temperaturen unterworfen ist, meist langsam in die eine oder andere Richtung.

[question:EF304]

Ein wesentlich frequenzstabilerer Oszillator-Typ ist der *Quarz-Oszillator*. Hierbei wird als frequenzbestimmende Komponente ein Schwingquarz verwendet, dessen Resonanzfrequenz nur in sehr geringem Maße von dessen Temperatur abhängig ist (im Vergleich zu LC-Oszillatoren).

[question:ED506]
[question:ED507]

Um unerwünschte Abstrahlungen zu vermeiden, sollten Oszillatoren sowie Pufferstufen immer möglichst gut geschirmt werden. Dies kann z.B. durch den Einbau des Oszillators in ein geerdetes Metallgehäuse erfolgen.

[question:EF207]