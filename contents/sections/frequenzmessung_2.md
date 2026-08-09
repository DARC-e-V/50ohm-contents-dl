Auch die Frequenzanzeige eines Empfängers kann überprüft werden. Anders als bei einem Sender lässt sich die eingestellte Empfangsfrequenz jedoch normalerweise nicht einfach an einem Ausgang des Funkgeräts mit einem Frequenzzähler messen. Das empfangene HF-Signal wird im Empfänger bereits früh weiterverarbeitet und beispielsweise auf eine Zwischenfrequenz umgesetzt.

Zur Überprüfung der Frequenzanzeige verwendet man deshalb ein möglichst genaues Referenzsignal. Dazu wird ein Frequenzgenerator oder ein genauer Referenzoszillator mit bekannter Frequenz an den Antenneneingang des Empfängers angeschlossen. Anschließend wird der Empfänger auf dieses Signal abgestimmt und seine Frequenzanzeige mit der bekannten Frequenz des Referenzsignals verglichen.

Je genauer die verwendete Referenz ist, desto genauer kann auch die Frequenzanzeige des Empfängers überprüft beziehungsweise kalibriert werden. Besonders gut eignen sich beispielsweise GPS-synchronisierte Oszillatoren oder hochwertige temperaturstabilisierte Quarzoszillatoren (OCXO).

<attention>
Ein direkt angeschlossener Frequenzgenerator kann einen Empfängereingang leicht beschädigen. Im Zweifelsfall sollte die Messung mit der niedrigsten Spannung des Generators und einem Dämpfungsglied begonnen werden.
</attention>

[question:AI511]
[question:AI504]

---

Bei Sendern ist die Frequenzmessung einfacher. Ein Frequenzzähler wird über ein Dämpfungsglied an die Antennenbuchse angeschlossen. Sinnvoll ist diese Messung natürlich nur bei einem unmodulierten Träger, also einem möglichst reinen Sinus.

<indepth>
SSB-Sender erzeugen ohne Modulation kein Signal. Um ihre Sendefrequenz zu messen, kann man ein Audiosignal mit bekannter Frequenz in die Mikrofonbuchse einspeisen. Vom Messwert des Frequenzzählers am Senderausgang wird bei USB die Audiofrequenz abgezogen, um die Frequenz des nicht ausgesendeten Trägers zu erhalten. Bei LSB wird sie addiert.
</indepth>

[question:AI502]
[question:AI501]

Eine Frequenz kann auch mit einem Oszilloskop bestimmt werden. Für genaue Frequenzmessungen ist ein Oszilloskop jedoch meist weniger geeignet als ein dedizierter Frequenzzähler, da dessen Zeitbasis und Messverfahren speziell auf eine hohe Frequenzgenauigkeit und -auflösung ausgelegt sind.

[question:AI503]

---

Einfache Frequenzzähler arbeiten häufig mit einer sogenannten *Torzeit*. Während dieser Zeit zählt das Gerät die Perioden beziehungsweise Flanken oder Nulldurchgänge des Eingangssignals. Aus der Anzahl der gezählten Schwingungen und der bekannten Torzeit wird anschließend die Frequenz berechnet. Beispiel: Bei einer Torzeit von einer Sekunde ist die Frequenzbestimmung besonders einfach: Werden beispielsweise $\num{1000}$ Perioden gezählt, beträgt die gemessene Frequenz $\qty{1000}{\hertz}$.

<margin>
[picture:1126:a_frequenzmessung_torzeit:Zählung eines Signals mit einer Frequenz von $\qty{1,1}{\kilo\hertz}$ bei sehr kleinen Torzeiten]
</margin>

Die *Frequenzauflösung* $\Delta f$ gibt an, wie klein der Frequenzunterschied zwischen zwei Messwerten sein kann, den der Frequenzzähler noch unterscheiden beziehungsweise anzeigen kann. Bei einem einfachen direkt zählenden Frequenzzähler wird die Frequenzauflösung durch die Torzeit $T_\mathrm{G}$ bestimmt:

$\Delta f = \frac{1}{T_\mathrm{G}}$

Welche Auswirkung die Torzeit beziehungsweise die Frequenzauflösung auf das Messergebnis hat, zeigt die Abbildung [ref:a_frequenzmessung_torzeit]. In beiden Fällen wird dasselbe Signal mit einer tatsächlichen Frequenz von $\qty{1,1}{\kilo\hertz}$ gemessen.

Bei einer Torzeit von nur $\qty{1}{\milli\second}$ wird lediglich eine Periode gezählt. Der Frequenzzähler ermittelt daraus einen Messwert von $\qty{1}{\kilo\hertz}$. Die kurze Torzeit erlaubt hier also nur eine Frequenzauflösung von $\qty{1}{\kilo\hertz}$.

Wird die Torzeit auf $\qty{10}{\milli\second}$ verlängert, können bereits $\num{11}$ Perioden gezählt werden. Daraus ergibt sich ein Messwert von $\qty{1,1}{\kilo\hertz}$. Die Frequenzauflösung beträgt nun $\qty{100}{\hertz}$, sodass auch die zusätzliche Stelle der Frequenz angezeigt werden kann.

Je länger die Torzeit ist, desto mehr Perioden werden gezählt und desto feiner wird die Frequenzauflösung. Eine kurze Torzeit hat dagegen den Vorteil, dass die Anzeige häufiger aktualisiert werden kann. Bei der Wahl der Torzeit besteht somit ein Kompromiss zwischen schneller Aktualisierung und hoher Frequenzauflösung. Die Genauigkeit der Frequenzmessung ist von der Auflösung zu unterscheiden. Sie hängt insbesondere von der Genauigkeit der Zeitbasis des Frequenzzählers ab.

[question:AI505]