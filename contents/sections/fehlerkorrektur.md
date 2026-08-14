Erkennt der Empfänger einen Übertragungsfehler, zum Beispiel mithilfe von Prüfbits, kann er den Sender um eine erneute Übertragung der Daten bitten. Bei der *Vorwärtsfehlerkorrektur* ist dagegen häufig keine Neuübertragung erforderlich. Dazu werden den Nutzdaten zusätzliche Informationen hinzugefügt, zum Beispiel mehrere Prüfbits. Damit kann der Empfänger unter bestimmten Voraussetzungen nicht nur erkennen, dass ein Fehler aufgetreten ist, sondern auch bestimmen, welches Bit fehlerhaft ist, und dieses korrigieren. Im Englischen wird dieses Verfahren als *Forward Error Correction* (FEC) bezeichnet.

Wie das im Detail funktionieren kann, zeigt die nebenstehende Vertiefung am Beispiel eines Hamming-Codes. Das genaue Verfahren ist nicht prüfungsrelevant.

[question:AE413]
[question:AE414]

<indepth>
Der Hamming-Code ist ein Fehlerkorrekturverfahren, das mehrere Paritätsbits verwendet. Nehmen wir an, wir wollen die folgenden $\num{11}$ Datenbits übertragen:

[picture:683:hamming1: ]

Damit ein einzelner Bitfehler nicht nur erkannt, sondern auch korrigiert werden kann, müssen wir feststellen können, an welcher Stelle der Fehler aufgetreten ist. Dazu betrachten wir zunächst die Positionen der einzelnen Bits und benennen sie alphabetisch:

[picture:682:hamming2: ]

Nun ordnen wir die Datenbits etwas anders an und fügen vier zusätzliche Paritätsbits $p_1$ bis $p_4$ hinzu:

[picture:684:hamming3: ]

Die vier Paritätsbits überprüfen unterschiedliche, sich überlappende Gruppen von Bits:

[picture:685:hamming4: ]

Jedes Paritätsbit sichert dabei eine bestimmte Gruppe ab:

[picture:686:hamming5: ]

Für jede dieser Gruppen berechnen wir nun das zugehörige Paritätsbit mit *Even Parity*:

[picture:687:hamming6: ]

Tritt bei der Übertragung ein einzelner Bitfehler auf, schlagen bestimmte Paritätsprüfungen fehl. Aus der Kombination der fehlgeschlagenen Prüfungen lässt sich bestimmen, an welcher Position der Fehler aufgetreten ist. Das fehlerhafte Bit kann anschließend umgekehrt und damit korrigiert werden.

Wird zum Beispiel das Bit $k$ bei der Übertragung zu einer $\num{0}$, schlagen alle vier Paritätsprüfungen $p_1$ bis $p_4$ fehl. Nur Bit $k$ gehört zu allen vier überprüften Gruppen. Der Fehler muss daher bei Bit $k$ liegen.

Tritt dagegen ein Fehler im Bit $a$ auf, schlagen nur die Paritätsprüfungen von $p_1$ und $p_2$ fehl, während die Prüfungen von $p_3$ und $p_4$ erfolgreich sind. Aus diesem Muster kann der Empfänger erkennen, dass Bit $a$ fehlerhaft ist.

Auch ein Fehler in einem Paritätsbit selbst kann erkannt und korrigiert werden. Ist beispielsweise $p_1$ fehlerhaft, schlägt nur die zu $p_1$ gehörende Paritätsprüfung fehl, während die Prüfungen von $p_2$, $p_3$ und $p_4$ erfolgreich sind. Der Fehler muss daher bei $p_1$ liegen.

Der hier gezeigte Hamming-Code ist für die Korrektur eines einzelnen Bitfehlers ausgelegt. Treten mehrere Bitfehler gleichzeitig auf, kann aus den Paritätsprüfungen nicht mehr zuverlässig auf die tatsächliche Fehlerposition geschlossen werden. Erweiterte Hamming-Codes können zusätzlich beispielsweise zwei gleichzeitig auftretende Bitfehler sicher erkennen.
</indepth>