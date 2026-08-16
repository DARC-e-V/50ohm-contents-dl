In der Klasse N haben wir bereits gelernt, dass Remotebetrieb nur für Funkamateure der Klasse A erlaubt ist. Deshalb wollen wir hier nun einige technische Aspekte des Remotebetriebs betrachten, welche für das Betreiben und Benutzen einer Remote-Station relevant sind. 

Eine Station für Remote-Betrieb besteht aus mehreren voneinander logisch trennbaren Funktionsblöcken. Hierbei können bei modernen Geräten auch Teile dieser Funktionsblöcke in einem Gerät integriert sein (z.B. Transceiver mit Netzwerkanschluss und Remote-Interface).

Eine Anordnung für Remote-Betrieb kann mit folgenden Funktionsblöcken logisch dargestellt werden.

---

<margin>
[picture:501:a_remotebetrieb:Blockschaltbild Remote Betrieb]
</margin>

* *Computer und Bedienteil des Operators (Block 1)*: Dieses dient zur Steuerung der Remote-Station. Hierbei werden lokal Audiosignale sowie Steuersignale in Netzwerkpakete umgewandelt und an die Remote-Station übertragen. Empfangene Steuer- und Audiosignale der Remote-Station (welche über Netzwerk übertragen werden) werden durch den Computer/das Bedienteil wieder hör- und sichtbar gemacht.
* *Netzwerk*: Verbindungsnetzwerk oder Verbindungsnetzwerke zwischen Standort des Operators und der Remote-Station. Hierbei kann auch das Internet als Netzwerk zwischen den Standorten dienen.
* *Computer oder Remoteinterface am Remote-Standort (Block 2)*: Dieses setzt empfangene Netzwerkpakete des Operators in Steuersignale und Audiosignale für die weitere Steuerung des Transceivers am Remote-Standort um und überträgt im Rückweg die empfangenen Audiosignale des Transceivers über das Netzwerk zum Operator. Auch Einstellungen des Transceivers sowie rücklaufende Steuersignale werden über das Netzwerk zum Operator übertragen.
* *Transceiver/Verstärker/Tuner/Antennenrotor (Block 3)*: Diese Geräte werden durch das Remote-Interface oder einen Computer am Remote-Standort angesteuert/rückgemeldet durch Signale, die der Operator über das Netzwerk an das Remote-Interface überträgt.

[question:AF701]
[question:AF702]
[question:AF704]
[question:AF703]
[question:AF705]

---

Bei Remote-Betrieb kommt es durch Laufzeiten im Netzwerk und Verarbeitungszeiten bei der Codierung und Decodierung von Audio-Signalen zu zeitlichen Verzögerungen. Dies ist beim Funkbetrieb über Remote-Stationen zu berücksichtigen.

<tip>
[photo:342:a_remote_station:Remote-Station des DARC e. V.]

Der DARC e. V. betreibt für seine Mitglieder einige Remote-Clubstationen, die über ganz Deutschland verteilt sind. Auf [mein.darc.de](https://mein.darc.de/) können Mitglieder sich in die Remote-Stationen einwählen und über das Internet Funkbetrieb machen, falls sie eine Zulassung zur Klasse A besitzen. Für Klasse N und E ist nur SWL-Betrieb möglich.

[Jetzt Mitglied im DARC werden!](https://50ohm.de/mw)
</tip>

[question:AF709]
[question:AF710]

Um sicherzustellen, dass eine Remote-Station bei Abbruch oder Störung der Datenverbindung zwischen Benutzer/Bedienteil und Remote-Interface nicht in einen unkontrollierten Zustand/Betrieb fällt, ist eine permanente Überwachung und Rückmeldung zwischen Operator und Remote-Station mittels eines sog. Watchdogs erforderlich. Hierbei werden z.B. in zeitlichen Abständen von wenigen Sekunden Datenpakete von der Remote-Station an den Computer des Operators gesendet, die in einer bestimmten Zeit durch Rückantwort quittiert werden müssen. Erfolgt diese Rückantwort nicht, so weiß die Remote-Station, dass die Verbindung zum Operator unterbrochen ist und kann den Transceiver selbsttätig in einen definierten sicheren Zustand (z.B. Empfangsmodus) bringen und eine laufende Sendung unterbrechen.

[question:AF708]

Da auch der Transceiver selbst in einen undefinierten Zustand kommen kann (z.B. durch Software- oder Hardware-Fehler im Gerät) sollte die Versorgungsspannung des Transceivers aus der Ferne abschaltbar sein. Dies kann z.B. durch eine IP-Steckdose, welche sich durch den Operator über das Netzwerk steuern lässt, erfolgen.

[question:AF707]

Beim Betrieb einer Remote-Station ist ebenfalls zu berücksichtigen und damit zu rechnen, dass Komponenten der Remote-Station durch den Transceiver am Standort der Remote-Station gestört werden können.

[question:AF706]