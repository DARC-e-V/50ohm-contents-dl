Im folgenden Abschnitt werden die einzelnen Schritte einer Sende- und Empfangskette beschrieben. Die Abbildung [ref:a_sdr_sender] zeigt beispielhaft einen SDR-Sender für die Sprachkommunikation. Im ersten Schritt wird das Mikrofonsignal durch einen A/D-Umsetzer digitalisiert. Das digitale Signal wird anschließend durch einen Quellencodierer komprimiert, um die benötigte Bandbreite zu reduzieren. Im darauffolgenden Schritt versieht ein Kanalcodierer das komprimierte Signal gezielt mit Redundanz, sodass Übertragungsfehler erkannt und korrigiert werden können. Die codierten Daten werden schließlich durch einen Mapper in Symbole umgewandelt und anschließend durch einen I/Q-Modulator moduliert. Den Abschluss der Sendekette bilden ein Leistungsverstärker sowie die Antenne, über die das Signal abgestrahlt wird.

<margin>
[picture:1062:a_sdr_sender:SDR Sender für Sprachkommunikation]
</margin>

Die in blau hervorgehobenen Blöcke in Abbildung [ref:a_sdr_sender] repräsentieren die Signalverarbeitungsschritte, die beispielsweise rein softwarebasiert oder mithilfe eines FPGAs implementiert werden können. Die Reihenfolge dieser Verarbeitungsschritte ist für einen Sender stets wie folgt und sollte für Prüfungsfragen gut eingeprägt werden:

1. Quellencodierer: Daten komprimieren
2. Kanalcodierer: Hinzufügen von Redundanz zur Fehlererkennung und -korrektur
3. Mapper: Abbilden binärer Daten auf Symbole z. B. Amplitude und Phase für QAM

[question:AF626]
[question:AF627]

---

Für einen Empfänger funktioniert das Ganze rückwärts: Die Antenne empfängt das Signal, das durch einen Leistungsverstärker verstärkt wird. Anschließend erfolgt die Demodulation durch einen I/Q-Demodulator, um die Symbole zu extrahieren. Der De-Mapper ordnet diese Symbole wieder den ursprünglichen binären Daten zu. Danach übernimmt der Kanaldecodierer die Aufgabe, Fehler zu erkennen und zu korrigieren, die während der Übertragung entstanden sein könnten. Abschließend dekomprimiert der Quellendecodierer die Daten, um das ursprüngliche Signal wiederherzustellen, welches dann über einen D/A-Umsetzer in ein analoges Signal zurückverwandelt und beispielsweise über einen Verstärker an einem Lautsprecher ausgegeben werden kann.

Wir fassen die digitale Signalverarbeitung im Empfänger in den folgenden drei Schritten zusammen:

1. De-Mapper: Abbilden der Symbole auf binäre Daten
2. Kanaldecodierer: Erkennen und korrigieren von Fehlern
3. Quellendecodierer: Daten dekomprimieren

<margin>
[picture:1063:a_sdr_empfänger:SDR Empfänger für Sprachkommunikation]
</margin>

[question:AF628]
[question:AF629]
