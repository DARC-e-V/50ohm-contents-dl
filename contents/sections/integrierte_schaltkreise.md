Integrierte Schaltungen sind komplexe Schaltungen, die auf einem Halbleitersubstrat realisiert sind. Sie sind damit eine wesentliche Erleichterung für den Aufbau von elektronischen Schaltungen.

Als spezielle Klasse der Integrierten Schaltkreise gibt es die  Monolithic Microwave Integrated Circuits (MMIC). Sie vereinen dabei sowohl aktive wie auch passive Bauelemente auf dem gleichen Substrat. Diese werden typischerweise für eine Ein- und Ausgangsimpedanz von $\qty{50}{\ohm}$ ausgelegt. Mit ihnen ist eine hohe breitbandige Verstärkung mit wenigen Bauteilen möglich.

[question:AC601]
[question:AC602]
[question:AC603]
[question:AC604]

---

Zur Berechnung der Aufgaben aus der Prüfung ist es wichtig, die bestehende Schaltung aus Abbildung [ref:a_mmic] ein bisschen zu analysieren. 

Der optimale Arbeitspunkt eines MMICs wie in dieser Schaltung, wird über die Einstellung eines Vorwiederstandes $R_\text{BIAS}$ realisiert, der mit einer Betriebsspannung $U_\text{CC}$ versorgt wird. Aus Sicht der Betriebsspannung (einer Gleichspannung), können die Kondensatoren $C_1$, $C_2$ und $C_3$ als Isolatoren betrachtet werden. Über ihnen fällt keine Spannung ab.

Das bedeutet, dass aus Sicht der Betriebsspannung der Anschluss 2 und Anschluss 4 des MMICs auf Masse liegt, der Anschluss 1 ist offen.

<margin>
[picture:773:a_mmic:MMIC-Schaltung]
</margin>

% TODO Gleichspannungs-Ersatzschaltbild für das Bild aus der Aufgabe AF427

Daraus wiederum lässt sich ableiten, dass die Betriebsspannung vollständig über den beiden Bauelementen des Vorwiderstands $R_\text{BIAS}$ und des MMICs abfällt.

Abhängig von der Aufgabenstellung kann man bei dem gegebenen Spannungsabfall über dem MMIC den Spannungsabfall über dem Vorwiderstand $R_\text{BIAS}$ berechnen. Damit lässt sich dann, bei gegebenem Widerstand, der Strom berechnen, der durch die Schaltung fließt. Der selbe Strom fließt auch durch den MMIC. Damit lässt sich dort dann zum Beispiel auch die thermische Verlustleistung berechnen.

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



