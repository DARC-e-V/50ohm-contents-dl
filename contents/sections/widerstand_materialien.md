% TODO: Wenn der Fragenkatalog 4 kommt, dann fallen hier einige Fragen weg! 

Den elektrischen Widerstand haben wir bereits im Zusammenhang mit dem ohmschen Gesetz kennengelernt. Widerstände können aus unterschiedlichen Materialien realisiert werden. Aus diesem Grund unterscheidet man verschiedene Widerstandsmaterialien, z. B.:

- Drahtwiderstände
- Kohleschichtwiderstände
- Metallschichtwiderstände
- Metalloxidschichtwiderstände
- ...

<margin>
| l: Widerstand | X: Eigenschaft |
| Drahtwiderstände | Hochlastwiderstände für niedrige Frequenzen |
| Metallschichtwiderstände | Geringe Fertigungstoleranzen und Temperaturabhängigkeit, Präzisionswiderstände |
| Metalloxidschichtwiderstände | Für Frequenzen oberhalb von $\qty{30}{\mega\hertz}$ |
[table:e_eigenschaften_widerstaende:Übersicht der Eigenschaften]
</margin>

Im Folgenden gehen wir auf diese Materialien genauer ein - eine Zusammenfassung ist in Tabelle [ref:e_eigenschaften_widerstaende].

*Drahtwiderstände* zählen zu den ältesten Formen elektrischer Widerstände. Aufgrund ihrer günstigen Eigenschaften – wie hoher Überlastbarkeit und geringem Temperaturkoeffizienten – werden sie auch heute noch eingesetzt. Häufig werden sie auch als Wickelwiderstände bezeichnet, da lackisolierter Widerstandsdraht, beispielsweise aus Manganin oder Konstantan, auf einen Wickelkörper aus Keramik aufgewickelt wird. Ein einfach gewickelter Drahtwiderstand wirkt jedoch stets auch als Spule und besitzt daher eine vergleichsweise hohe Induktivität. Auf Spulen gehen wir in einem späteren Kapitel noch genauer ein; vorweg sei jedoch erwähnt, dass dadurch die Impedanz des Widerstands frequenzabhängig wird. In der Funktechnik ist dieses Verhalten in der Regel unerwünscht. Deshalb eignen sich Drahtwiderstände vor allem als Hochlastwiderstände für Gleichstrom oder für Anwendungen mit niedrigen Frequenzen.

%EC101 Hochlast niedrige Frequenz -> Drahtwiderstand
[question:EC101]

Bei Kohleschichtwiderständen wird als Widerstandswerkstoff eine dünne Kohleschicht auf einen Träger aufgedampft. Kohleschichtwiderstände sind kostengünstig, weisen jedoch eine vergleichsweise große Fertigungstoleranz auf.

Bei *Metalloxidschichtwiderständen* wird das Widerstandsmaterial in Form einer dünnen Schicht auf ein Trägermaterial aufgebracht. Diese Widerstandsart ist weitgehend induktionsarm und weist eine gute Temperaturstabilität auf, sodass sie sich besonders für den Einsatz bei höheren Frequenzen oberhalb von $\qty{30}{\mega\hertz}$ eignet.

%EC103 induktionsarm 30Mhz - >Metalloxid
[question:EC103]

*Metallschicht*widerstände können mit hoher Genauigkeit das heißt mit geringer Fertigungstoleranz gefertigt werden. Sie eignen sich als Präzisionswiderstände. Sie sind temperaturunabhängig, allerdings weniger induktionsarm.

%EC102 Präzisionswiderstand >Metallschichtwiderstand
[question:EC102]


Künstliche Antennen, also Dummyloads, haben wir bereits in der Klasse N kennengelernt. Für hohe Frequenzen (z. B. VHF) empfiehlt es sich, eine Dummyload vorzugsweise aus ungewendelten Metalloxidschichtwiderständen aufzubauen. Für niedrigere Frequenzen (z. B. $\qty{50}{\mega\hertz}$ oder $\qty{28}{\mega\hertz}$) können jedoch auch Kohleschichtwiderstände verwendet werden. Entscheidend ist vor allem, dass der Widerstand keine Windungen, also keine Eigeninduktivität besitzt und daher nicht als parasitäre Spule wirkt, denn eine solche Induktivität würde den Widerstandswert frequenzabhängig machen – genau das ist bei einer Dummyload unerwünscht. Der Widerstand soll unabhängig von der Frequenz stets etwa $\qty{50}{\ohm}$ betragen. Deshalb sollten _keine_ Drahtwiderstände verwendet werden. Auch die Eigenkapazität sollte aus diesem Grund möglichst gering sein. Zudem müssen die eingesetzten Widerstände ausreichend temperaturbeständig sein, da sie die aufgenommene Leistung in Wärme umsetzen.

%EC107 DL
[question:EC107]
%EC104 DL
[question:EC104]

Für die Lösung der folgenden Fragen muss man wissen, dass zehn parallel geschaltete Widerstände mit jeweils $\qty{500}{\ohm}$ zusammen einen Gesamtwiderstand von $\qty{50}{\ohm}$ ergeben. Auf diesen Zusammenhang gehen wir in einem späteren Kapitel noch genauer ein, wenn wir über Reihen- und Parallelschaltungen von Widerständen sprechen.

%EC106
[question:EC106]
%EC105 DL
[question:EC105]