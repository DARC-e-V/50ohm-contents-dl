Es ist auch möglich, einen Datenstrom auf mehrere Träger zu verteilen, die auf unterschiedlichen, jedoch nahegelegenen Frequenzen liegen. Die Träger können allerdings nicht beliebig dicht nebeneinander liegen, da sie aufgrund der zwangsläufig entstehenden Seitenbänder eine gewisse Breite aufweisen.

Beim orthogonalen Frequenzmultiplexverfahren, (Orthogonal Frequency-Division Multiplexing, OFDM) werden nun die einzelnen Träger in genau dem Abstand platziert, wo ein gegenseitiges Stören untereinander (ein sogenanntes "Übersprechen") möglichst vermieden wird.

Je höher die Symbolrate pro Träger ist, umso größer muss der Abstand der Träger gewählt werden. Aus diesem Grunde wählt man oft eine kleinere Symbolrate für jeden einzelnen Träger, damit entsprechend mehr Träger Platz finden. Die übertragene Informationsmenge bleibt hierbei gleich, denn obwohl pro Träger weniger Information übertragen werden kann, können mehr Träger nebeneinander verwendet werden. Ein höherer Trägerabstand ist beispielsweise hilfreich, um das Signal toleranter gegen Frequenzfehler zu machen, sei es durch Frequenzabweichungen zwischen Sender und Empfänger, oder durch Dopplerverschiebung bei bewegten Sendern oder Empfängern.

Ein Vorteil dieses Vorgehens liegt darin, dass schmalbandige Störungen nur einen oder wenige Träger stören. Im Zusammenspiel mit Fehlerkorrekturverfahren mit redundanter Datenübertragung, die wir einige Kapitel zuvor kennengelernt haben, ist es so möglich, trotz schmalbandiger Störungen eine fehlerfreie Übertragung zu erreichen.

<margin>
[picture:704:ofdm:Frequenzspektrum eines einfachen OFDM-Signals]
</margin>

[question:AE421]

Ein weiterer Vorteil ergibt sich aus der geringeren Symbolrate jedes einzelnen Trägers. Durch die geringere Symbolrate ist die Dauer eines jeden Symbols länger. Im Falle zeitlicher Verschiebungen aufgrund von Mehrwegeausbreitung ist der Anteil der Überlagerung zwischen den Signalen (sogenannte Intersymbolinterferenz oder Symbolübersprechen) dann entsprechend geringer. Auch kann es vorkommen, dass einzelne Frequenzen durch Mehrwegeausbreitung ausgelöscht oder zumindest stark gedämpft werden (man spricht von frequenzselektivem Fading). Dies kann mit den gleichen Mechanismen kompensiert werden wie die weiter oben erwähnten schmalbandigen Störungen. Im Falle von Mehrwegeausbreitung ist OFDM daher besonders vorteilhaft.

[question:AE422]