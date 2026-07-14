Im vorigen Kapitel haben wir gesehen, dass es verschiedene Oszillatortypen mit unterschiedlicher Frequenzstabilität und -genauigkeit gibt. Eine besonders hohe Stabilität erreichen Quarzoszillatoren in Form eines TCXO und insbesondere eines OCXO. Moderne Funkgeräte erreichen beispielsweise mit einem TCXO eine Frequenzgenauigkeit von $\pm\qty{0,5}{\ppm}$. Bei einer gewünschten Frequenz von $\qty{10}{\mega\hertz}$ liegt die tatsächliche Frequenz damit im Bereich von $\qtyrange{9,999995}{10,000005}{\mega\hertz}$, also höchstens $\pm\qty{5}{\hertz}$ neben der Sollfrequenz. Diese Abweichung ist gering und für den Betrieb auf Kurzwelle in der Regel mehr als ausreichend.

Arbeiten wir jedoch nicht bei $\qty{10}{\mega\hertz}$, sondern bei $\qty{10}{\giga\hertz}$, erhöht sich die mögliche Abweichung auf $\pm\qty{5000}{\hertz}$. Sie kann damit bereits größer als die Bandbreite eines üblichen SSB-Filters sein. Bei einer Funkverbindung auf einer fest vereinbarten Frequenz kann das Signal deshalb außerhalb des Empfangsbereichs liegen. Für solche Anwendungen, z. B. beim geostationären SAT QO-100 welcher auf $\qty{10}{\giga\hertz}$ sendet, werden daher noch genauere Frequenzreferenzen benötigt. 

<margin>
[picture:1081:a_gpsdo:GPS-Disciplined Oscillator (GPSDO) im Kontext einer QO-100 Station]
</margin>

Man könnte einen hohen Aufwand betreiben, um einen OCXO weiter zu stabilisieren, oder andere Oszillatortypen wie Rubidium-Frequenznormale verwenden, die insbesondere über längere Zeiträume eine höhere Stabilität als Quarzoszillatoren erreichen. Solche Frequenznormale haben jedoch häufig Nachteile wie eine höhere Stromaufnahme, größere Abmessungen und einen höheren Preis, da sie vor allem für professionelle Anwendungen entwickelt werden.

Glücklicherweise gibt es eine weitere Möglichkeit: Satellitennavigationssysteme, englisch Global Navigation Satellite Systems (GNSS), wie GPS oder Galileo benötigen sehr genaue Zeitreferenzen. Die Position des Empfängers wird anhand der Laufzeiten von Signalen bestimmt, die von mehreren Satelliten zum Empfänger übertragen werden. Da jede präzise Uhr einen stabilen Oszillator als Zeitbasis benötigt, können wir die aus den Satellitensignalen gewonnene Zeitreferenz zur Stabilisierung unseres eigenen TCXO oder OCXO verwenden. Ein solcher Oszillator wird als GPS-synchronisierter Oszillator oder englisch als GPS-Disciplined Oscillator (GPSDO) bezeichnet. Wie diese Regelung technisch funktioniert, betrachten wir in einem späteren Kapitel zu Phasenregelschleifen (PLLs). In Abbildung [ref:a_gpsdo] ist ein GPSDO im Kontext einer QO-100 Station dargestellt, welches das Software Defined Radio (SDR) mit einer stabilen Referenzfrequenz versorgt. Ein selbst gebautes Modul ist in Abbildung [ref:a_gpsdo_homebrew] zu sehen.

---

Nun könnte man sich fragen, warum wir die von GPS bereitgestellte Zeitreferenz nicht direkt als Oszillatorsignal verwenden. Der GPS-Empfänger gewinnt aus den schwachen und modulierten Satellitensignalen üblicherweise ein präzises Zeitsignal, beispielsweise einen Impuls pro Sekunde. Der genaue Zeitpunkt dieses Impulses kann kurzfristig jedoch durch Rauschen, Mehrwegeausbreitung, atmosphärische Einflüsse und Verzögerungen im Empfänger schwanken. Über längere Zeiträume betrachtet ist die daraus abgeleitete Frequenz dagegen sehr genau.

Ein TCXO oder OCXO besitzt wiederum eine gute beziehungsweise sehr gute Kurzzeitstabilität, kann jedoch langfristig durch verbleibende Temperatureinflüsse und die Alterung seiner Bauelemente langsam von der Sollfrequenz abweichen. In einem GPSDO werden deshalb beide Eigenschaften miteinander kombiniert: Der lokale TCXO oder OCXO liefert ein kurzzeitig stabiles und rauscharmes Ausgangssignal, während eine langsame Regelschleife seine langfristige Abweichung mithilfe der GPS-Zeitreferenz korrigiert. Auf diese Weise erreicht ein GPSDO sowohl eine sehr gute Kurzzeitstabilität als auch eine hohe Langzeitstabilität und Frequenzgenauigkeit.

[question:AD606]

<margin>
[photo:335:a_gpsdo_homebrew:Selbstgebautes GPSDO mit TCXO]
</margin>