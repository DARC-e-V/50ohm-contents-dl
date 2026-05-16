Integrierte Schaltungen sind komplexe Schaltungen, die auf einem Halbleitersubstrat realisiert sind. Sie sind damit eine wesentliche Erleichterung für den Aufbau von elektronischen Schaltungen.

[question:AC601]

<margin>
[photo:334:a_ic:Kurzwellensender TinyWhisper der JKU Linz und JMU Würzburg realisiert als integrierte Schaltung in 130nm CMOS-Technologie]
</margin>

Als spezielle Klasse der integrierten Schaltkreise gibt es die Monolithic Microwave Integrated Circuits (MMIC). Sie vereinen dabei sowohl aktive wie auch passive Bauelemente auf dem gleichen Substrat. Diese werden typischerweise für eine Ein- und Ausgangsimpedanz von $\qty{50}{\ohm}$ ausgelegt. Mit ihnen ist eine hohe breitbandige Verstärkung mit wenigen Bauteilen möglich.

[question:AC602]
[question:AC603]
[question:AC604]

---

Zur Berechnung der Aufgaben aus der Prüfung ist es hilfreich, die Schaltung aus Abbildung [ref:a_mmic] zunächst genauer zu betrachten.

Die Kondensatoren $C_1$ und $C_3$ dienen als Koppelkondensatoren. Sie lassen HF-Signale passieren, sperren jedoch Gleichspannung. Dadurch wird verhindert, dass Gleichspannungen zwischen den einzelnen Schaltungsstufen übertragen werden und den Arbeitspunkt beeinflussen.

Die Drossel in der Betriebsspannungsleitung $U_\mathrm{CC}$ verhindert, dass HF-Signale über die Spannungsversorgung abfließen können. Für Hochfrequenz besitzt die Drossel einen hohen Widerstand und wirkt daher als Sperre. Der Kondensator $C_2$ dient zur HF-Abblockung der Versorgungsspannung. Er leitet verbleibende HF-Anteile gegen Masse ab und sorgt dafür, dass die Versorgungsspannung HF-mäßig stabil bleibt. Zusammen mit der Drossel bildet er eine HF-Entkopplung der Betriebsspannung. Diese Schaltung lernen wir später noch als "Bias-T" kennen.

Eine Besonderheit vieler MMICs besteht darin, dass die Versorgungsspannung über den Ausgang zugeführt wird. Der Widerstand $R_\text{BIAS}$ stellt dabei den Arbeitspunkt des MMIC ein.

<margin>
[picture:773:a_mmic:MMIC-Schaltung]
</margin>

Abhängig von der Aufgabenstellung kann aus dem Spannungsabfall über dem MMIC zunächst der Spannungsabfall über dem Widerstand $R_\text{BIAS}$ bestimmt werden. Mit dem bekannten Widerstandswert lässt sich anschließend der Strom durch die Schaltung berechnen. Derselbe Strom fließt auch durch den MMIC, sodass sich daraus beispielsweise die thermische Verlustleistung bestimmen lässt.

Die folgenden Aufgaben lassen sich daher sehr ähnlich zu den bereits bekannten Schaltungen mit Bipolartransistoren lösen.

[question:AF425]
[question:AF426]
[question:AF427]

% Eine wesentliche Erleichterung bei dem Aufbau von elektronischen Schaltung 
% ist die Verwendung von integrierten Schaltungen.
% Eine integrierte Schaltung enthält in einem Gehäuse eine komplexe elektronische Schaltung, 
% die auf einem Chip hergestellt wurde.

% "Zusatzinfo" Praktische Anwendungen:
% Operationsverstärker: siehe Abschnitt ...
% Niederfrequenzverstärker: siehe Abschnitt ...
% Mikrowellenverstärker MMIC: siehe Abschnitt ...
% Kombinierte Mischer- und Oszillatorschaltung: siehe Abschnitt ...
% Komplette Empfänger: siehe Abschnitt ...
% Digitale Schaltkreise: siehe Abschnitt ...
% PLL-Schaltungen: siehe Abschnitt ...

% Durch wenige externe Bauteile kann z.B. ein Audioverstärker, ein Oszillator mit Mischer oder sogar ein kompletter % Kurzwellenempfänger realisiert werden.
% Bild eines IC mit Typenbezeichnung und Blockschaltbild z.B. LM386
% Für Frequenzen ab ca. 100 MHz werden sogenannte Monolithic Microwave Integrated Circuit (MMIC) eingesetzt.
% Bild MMIC MSA 0686 oder ERA 3
% Hierbei handelt es sich um einen Verstärker. der breitbandig den Frequenzbereich von 100 MHz bis 2 GHz um  20dB verstärken kann
% und eingangs- und ausgangsseitug für 50 Ohm Last angepasst ist.
% Es muss lediglich der Strom für den Arbeitspunkt laut Datenblatt eingestellt werden, damit der MMIC auch nicht % thermisch überlastet wird. 
% Dazu ist bei vorgegebener Betriebsspannung ein Widerstand und dessen elektrische Belastung zu berechnen.

% Da der MMIC ein Gehäuse für SMD-Technik besitzt, ist es notwendig, auch die äußere Beschaltung in SMD- Technik auszuführen.
% Der Gesamtaufbau des Verstärkers wird so deutlich kleiner sein als früher in diskreter Schaltungstechnik.
% Bild Vergleich diskrete Schaltung und MMIC



