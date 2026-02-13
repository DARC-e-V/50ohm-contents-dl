### Halbleiter-Dioden in Modulatoren

* Bisher als Gleichrichter bekannt
* NF-Spannung ändert den Diodenwiderstand
* NF-Signal steuert den Diodenstrom
* HF-Signal wird im Takt des NF-Signals moduliert
* Einfachste Variante hat einen Träger und zwei Seitenbänder

---
### Diode im Amplitudenmodulator
<left>
[picture:772:a_modulatoren_am_modulator:AM-Modulator]
</left>
<right>
* Eine Diode wird gleichzeitig mit einem NF- und HF-Signal beaufschlagt
* Ein LC-Schwingkreis filtert das Ausgangssignal
</right>

---
[question:AD507]

---
### Balancemischer zur Trägerunterdrückung
* Vier Dioden in Ring-Anordnung unterdrücken den Träger
* Eine Gegentakt-Schaltung hebt Trägersignale auf
* Es bleiben nur die Seitenbänder übrig
* Bereits als Balancemischer im Kapitel "Mischer&nbsp;II" gezeigt

---
### Balancemodulator im SSB-Modulator
* Der Balancemodulator erzeugt ein Doppelseitenband-Signal (DSB)
* Ein Bandpassfilter lässt nur ein Seitenband durch
* Daraus entsteht ein SSB-Signal
* Zwei Stufen sind notwendig
 
---
[question:AE206]

---
[question:AF302]

---
### Erkennung eines Balancemischers
<left>
[picture:759:a_modulatoren_dsb:Modulator für AM-Signale mit unterdrücktem Träger]
</left>
<right>
* Ein Dioden-Ring kennzeichnet den Balancemischer
* Es gibt keine vollständige Gegentaktanregung
* Ein Transformator liefert das Äquivalent zu einer Mittelanzapfung
</right>

---
[question:AF308]

<note>
* NF-Modulation wird in den Brückenzweig zwischen T2-Mittelanzapfung und Masse eingespeist
* Das Oszillator-Signal wird über T1 in den Diodenring eingespeist
* Das DSB-Signal wird über T2 ausgekoppelt
* Ohne Modulation liegen die Spannungsteiler auf Masse
* So wird der Träger unterdrückt
* Mit Modulation verschiebt sich das Potential und Strom fließt in T2
* Das Ausgangssignal entsteht
</note>

---
### Trägerunterdrückung und Ausbalancierung

* Trägerunterdrückung bewirkt die Auslöschung unerwünschter Signale
* Die Modulator-Schaltung muss ausbalanciert sein

---
[question:AD510]

---
### Justierung im Modulator

<left>
[picture:762:a_modulatoren_rc_traegerunterdrueckung:$R_1$ und $C_1$ zur Einstellung der Trägerunterdrückung nach Betrag und Phase]
</left>
<right>
* Amplituden werden mit Potis justiert
* Phasen werden mit C-Trimmern eingestellt
</right>

---
[question:AF309]

---
### Symmetrierung im Modulator

* Der Modulator wird symmetriert um den Träger zu unterdrücken
* Die Modulations-Seitenbänder bleiben erhalten

---
[question:AF304]

---
[question:AF303]

---
### Zweite Stufe des SSB-Modulators

<left>
[picture:98:a_modulatoren_blockschaltbild_sender:Blockschaltbild eines Senders]
</left>
<right>
* Hinter dem Balancemodulator folgt die zweite Stufe
* Durch Filterung wird das gewünschte Seitenband gewählt
</right>

---
[question:AF305]

---
### Quarz-Frequenz und Seitenbandlage

<left>
[picture:500:a_modulatoren_quarzfilter:Quarzfilter zur Auswahl des Seitenbands]
</left>
<right>
* Quarze bestimmen die Frequenz des unterdrückten Trägers
* Beim LSB liegt der Träger 1,5 kHz über der 9 MHz-Mitte
* Bei maximal 3 kHz NF liegt das LSB 1,5 kHz unter der Mitte
* Für das USB gilt das umgekehrt
</right>

---
[question:AF306]

---
[question:AF307]
---
#### Lösungsweg
* gegeben: $f_Q = 9MHz$
* gegeben: $f_{LSB} = 9,0015MHz$
* gesucht: $f_{USB}$

<fragment>
$\begin{split}f_{USB} &= f_Q - (f_{LSB} - f_Q)\\ &= 9MHz - (9,0015MHz - 9MHz)\\ &= 9MHz - 0,0015MHz\\ &=8,9985MHz\end{split}$ 
</fragment>

---
### Kapazitäts-Dioden in FM-Modulatoren

<left>
[picture:155:a_modulatoren_fm_modulator:FM-Modulator mit Varicap]
</left>
<right>
* FM-Modulatoren nutzen Kapazitäts-Dioden
* Die Diode ist Teil eines Oszillator-Schwingkreises
* Die Sperrspannung stellt eine feste Dioden-Kapazität ein
* Ein NF-Signal ändert die Oszillator-Frequenz im Takt
</right>

---
[question:AD508]

---
### Einfluss der Kapazitäts-Diode

<left>
[picture:158:a_modulatoren_fm_varicap:Varicap zur Beeinflussung Oszillator-Frequenz]
</left>
<right>
* Die Kapazitäts-Diode beeinflusst die Oszillator-Frequenz
* Sie ist parallel zum Schwingkreis geschaltet
</right>

---
[question:AF310]

---
### FM-Hub-Begrenzung
* Hohe NF-Spannungen führen zu übermäßigen Frequenzänderungen
* Eine Hub-Begrenzung ist notwendig
* Anti-parallel geschaltete Dioden begrenzen die Spannung auf die Knickspannung

---
[question:AD509]

---
### Signal‑Analyse einer Diode
<left>
[picture:142:a_modulatoren_regelspannung:Schaltung mit einem Ausgang für eine Regelspannung]
</left>
<right>
* Ein einzelnes Signal weist auf keinen Modulator hin
* Ein Elko am Ausgang zeigt Gleichspannung an
</right>

---
[question:AD503]

