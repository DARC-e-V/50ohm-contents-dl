[question:AC401]

Die pn-Diode besteht aus zwei Halbleiterbereichen, die durch den Vorgang der Dotierung entweder einen Überschuss an freien Elektronen (n) oder freien Löchern (p) haben. Rechts und links der Grenzfläche entsteht eine sogenannte Raumladungszone, die praktisch keine freien Ladungsträger enthält. Das n-Gebiet stellt die Kathode, das p-Gebiet die Anode dar. 

Wird die Diode mit einer Durchlassspannung beaufschlagt (positiv an der Anode, negativ an der Kathode), so werden Elektronen vom n-dotierten Gebiet in Richtung p-Gebiet und Löcher vom p-Gebiet in Richtung n-Gebiet geschickt. So ergibt sich die richtige Antwort.

Etwas verwirrend ist gegebenenfalls, dass die technische Stromrichtung entgegengesetzt zur Richtung des Elektronenflusses ist. Der Strompfeil zeigt also von der Anode zur Kathode, obwohl der Elektronenfluss von der Kathode zur Anode verläuft.

[question:AC403]

pn-Dioden zeigen eine exponentielle Abhängigkeit des Diodenstroms von der Diodenspannung. Der Sättigungsstrom steigt mit steigender Temperatur. Dies sorgt dafür, dass die für einen bestimmten Diodenstrom notwendige Diodenspannung mit steigender Temperatur kleiner wird. Die "Durchlassspannung" sinkt also (als Faustformel um $\qty{-2}{\milli\volt\per\kelvin}$ Temperaturerhöhung).
<indepth>

Der Diodenstrom ist:
  
$I_D(T) = I_S(T) \cdot \exp \left( \frac{U_D}{U_T}\right)$
  
$I_S$ ist der Sättigungsstrom, $U_T = k T/q$ die sogenannte Temperaturspannung. Hier ist $k$ die Boltzmann-Konstante, $q$ die Elementarladung.
  
Mit steigender Temperatur steigt der Sättigungsstrom und die Exponentialfunktion sinkt. Es überwiegt allerdings die Temperaturabhängigkeit des Sättigungsstroms.

</indepth>

[question:AC404]

Die Kapazitätsdiode nutzt die Kapazität zwischen den n- und p-Gebieten über die Raumladungszone hinweg, analog zu einem Plattenkondensator. Dabei darf aber kein nennenswerter Gleichstrom fließen, also muss die Diode in Sperrrichtung gepolt werden.

Je negativer die Diodenspannung (bzw. je höher die Sperrspannung), umso mehr dehnt sich die Raumladungszone aus und umso geringer wird die Diodenkapazität.

In den Fragen AC405 und AC406 werden *antiparallele Dioden* eingesetzt, um die Amplitude einer Wechselspannung zu begrenzen. Solche Schaltungen werden z.B. eingesetzt, um Empfängereingänge vor Spannungen zu schützen, die die Eingangstransistoren zerstören könnten.

[question:AC405]

Hier handelt es sich um Silizium-Dioden, die eine Schwellspannung von etwa $\qty{0,6}{\volt}$ haben. Wenn die Eingangsspannung also $\qty{0,6}{\volt}$ überschreitet, schaltet die rechte Diode durch. Unterschreitet sie $\qty{-0,6}{\volt}$, schaltet die linke Diode durch.

Bei der ersten Halbwelle wird die nötige Spannung noch nicht erreicht, sie wird also unverändert übertragen. Die beiden nächsten Halbwellen allerdings haben Amplituden, die die Schwellspannung überschreiten. Die Amplituden werden bei $\qty{\pm 0,6}{\volt}$ "geklippt".

[question:AC406]

Die Lösung verläuft analog zur vorhergehenden Aufgabe - aber die Dioden sind hier *Germanium-Dioden*, die Schwellspannung beträgt etwa $\qty{0,3}{\volt}$. Daher werden alle Halbwellen geklippt.

[question:AC407]

Hier werden zwei Bauelemente genannt, die mit Licht interagieren: der Fotowiderstand und die Fotodiode.

Der Fotowiderstand ist ein Bauelement, das über zwei nicht-sperrende Kontakte verfügt. Es verhält sich wie ein konventioneller Ohmscher Widerstand - der Strom steigt linear mit der angelegten Spannung. Der Widerstandswert kann durch Absorption von Licht verringert werden - die absorbierten Photonen erhöhen die Dichte der freien Ladungsträger. Liegt keine Spannung an, fließt auch kein Strom.

Die Fotodiode dagegen ist eine pn-Diode. Das Licht wird hier in der Raumladungszone absorbiert, es entstehen Elektron-Loch-Paare, die im elektrischen Feld der Raumladungszone getrennt werden. Dieses Feld existiert auch ohne äußere Vorspannung. Es fließt auch für $U_D=0$ ein Strom (ein Kurzschlussstrom). Dieser Strom hat die entgegengesetzte Richtung wie der konventionelle Diodenstrom. 

[question:AC408]

Optokoppler vereinen eine Leuchtdiode und eine Fotodiode in einem Gehäuse, wobei die Eingangsseite (Leuchtdiode) und die Ausgangsseite (Fotodiode) voneinander isoliert sind (galvanisch getrennt).

Diese Bauelemente werden eingesetzt, um Schnittstellen galvanisch zu trennen, zum Beispiel, um Masseschleifen zu verhindern, die für eingekoppeltes Netzbrummen sorgen können.