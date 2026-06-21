## Erklärung

Ein hochohmiger Entladewiderstand dient der kontrollierten Entladung von Netzteilkondensatoren. Er begrenzt den Entladestrom und reduziert damit die Gefahr von Lichtbogenbildung, Bauteilbeschädigung sowie elektrischer Gefährdung.

### Warum ein hochohmiger Widerstand?

Bei der Entladung eines Kondensators fließt der Strom über den Entladewiderstand $R$. Dieser wird so dimensioniert, dass:

* dass der Anfangsstrom begrenzt bleibt:

    $I_0 = \frac{U_0}{R}$

* keine gefährlich hohen Stromspitzen auftreten,
* keine Lichtbogenbildung entsteht,
* Bauteile und Leiterbahnen vor Überlastung geschützt werden,
* die Entladung dennoch innerhalb einer praxisgerechten Zeit erfolgt.

Ein niederohmiger Widerstand oder ein Kurzschluss würde dagegen zu:

* sehr hohen Anfangsströmen,
* möglichen Schäden an Kondensator und Leiterbahnen,
* unkontrollierten Strom- und Spannungsspitzen,
* erhöhter Brand- und Verletzungsgefahr

führen.

### Warum muss die Leistung des Widerstands ausreichend sein?

Die im Kondensator gespeicherte Energie beträgt:

$E = \frac{1}{2} \cdot C \cdot {U_0}^2$

Diese wird beim Entladen vollständig in Wärme im Widerstand umgesetzt.

Die anfängliche Verlustleistung beträgt:

$P_0 = \frac{{U_0}^2}{R}$

Für $R = \qty{100}{\kilo\Ohm}$ und $U_0 = \qty{400}{\volt}$ ergibt sich somit eine Leistung von $P_0 = \qty{1,6}{\watt}$.

Daher muss der Widerstand:

* eine ausreichende Nennleistung besitzen,
* kurzzeitig überlastbar sein (Pulsbetrieb),
* thermisch sicher dimensioniert werden, um Überhitzung zu vermeiden.
