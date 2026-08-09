Auch die Frequenzanzeige eines Empfängers kann überprüft werden. Anders als bei einem Sender lässt sich die eingestellte Empfangsfrequenz jedoch normalerweise nicht einfach an einem Ausgang des Funkgeräts mit einem Frequenzzähler messen. Das empfangene HF-Signal wird im Empfänger bereits früh weiterverarbeitet und beispielsweise auf eine Zwischenfrequenz umgesetzt.

Zur Überprüfung der Frequenzanzeige verwendet man deshalb ein möglichst genaues Referenzsignal. Dazu wird ein Frequenzgenerator oder ein genauer Referenzoszillator mit bekannter Frequenz an den Antenneneingang des Empfängers angeschlossen. Anschließend wird der Empfänger auf dieses Signal abgestimmt und seine Frequenzanzeige mit der bekannten Frequenz des Referenzsignals verglichen.

Je genauer die verwendete Referenz ist, desto genauer kann auch die Frequenzanzeige des Empfängers überprüft beziehungsweise kalibriert werden. Besonders gut eignen sich beispielsweise GPS-disziplinierte Oszillatoren oder hochwertige temperaturstabilisierte Quarzoszillatoren (OCXO).

<attention>
Ein direkt angeschlossener Frequenzgenerator kann einen Empfängereingang leicht beschädigen. Im Zweifelsfall sollte die Messung mit der niedrigsten Spannung des Generators und einem Dämpfungsglied begonnen werden.
</attention>

[question:AI511]
[question:AI504]

---

Bei Sendern ist die Frequenzmessung einfacher. Ein Frequenzzähler wird über ein Dämpfungsglied an die Antennenbuchse angeschlossen. Sinnvoll ist diese Messung natürlich nur bei einem unmodulierten Träger, also einem möglichst reinem Sinus.

<indepth>
SSB-Sender erzeugen ohne Modulation kein Signal. Um ihre Sendefrequenz zu messen, kann man ein Audiosignal mit bekannter Frequenz in die Mikrofonbuchse einspeisen. Von Messwert des Frequenzzählers am Senderausgang wird bei USB die Audiofrequenz abgezogen, um die Frequenz des nicht ausgesendeten Trägers zu erhalten. Bei LSB wird sie addiert.
</indepth>

[question:AI502]
[question:AI501]

Eine Frequenz kann auch mit einem Oszilloskop bestimmt werden. Für genaue Frequenzmessungen ist ein Oszilloskop jedoch meist weniger geeignet als ein dedizierter Frequenzzähler, da dessen Zeitbasis und Messverfahren speziell auf eine hohe Frequenzgenauigkeit und -auflösung ausgelegt sind.

[question:AI503]

---

Einfache Frequenzzähler arbeiten häufig mit einer sogenannten *Torzeit*. Während dieser Zeit zählt das Gerät die Perioden beziehungsweise Flanken oder Nulldruchgänge des Eingangssignals. Aus der Anzahl der gezählten Schwingungen und der bekannten Torzeit wird anschließend die Frequenz berechnet.

<margin>
[picture:1126:a_frequenzmessung_torzeit:Zählung eines Signals mit einer Frequenz von $\qty{1}{\kilo\hertz}$ während sehr kleinen Torzeiten]
</margin>

Bei einer Torzeit von einer Sekunde ist die Frequenzbestimmung besonders einfach: Werden beispielsweise $\num{1000}$ Perioden gezählt, beträgt die gemessene Frequenz $\qty{1000}{\hertz}$.

Welche Auswirkung die Torzeit auf das Messergebnis hat, zeigt die Abbildung [ref:a_frequenzmessung_torzeit]. In beiden Fällen wird dasselbe Signal mit einer tatsächlichen Frequenz von $\qty{1}{\kilo\hertz}$ gemessen. Bei der kurzen Torzeit werden jedoch nur wenige Perioden gezählt. Dadurch fällt bereits eine nicht vollständig erfasste Periode stark ins Gewicht und die gemessene Frequenz weicht deutlich vom tatsächlichen Wert ab.

Bei einer längeren Torzeit werden wesentlich mehr Perioden erfasst. Ein Zählfehler von etwa einer Periode hat dann relativ zur Gesamtzahl der gezählten Perioden einen deutlich geringeren Einfluss. Das Messergebnis liegt daher näher an der tatsächlichen Frequenz und die Auflösung der Frequenzmessung verbessert sich.

Eine kurze Torzeit hat dafür den Vorteil, dass die Anzeige häufiger aktualisiert werden kann. Bei der Wahl der Torzeit besteht somit ein Kompromiss zwischen schneller Aktualisierung und hoher Frequenzauflösung.

[question:AI505]