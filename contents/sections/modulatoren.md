Bisher kennen wir Halbleiter-Dioden nur in ihrer Funktion als Gleichrichter einer Wechselspannung. In Modulatoren zur Erzeugung von AM- und SSB-Signalen spielen Dioden eine neue Rolle: Durch eine angelegte NF-Spannung wird ihr Widerstand im Takt der NF-Frequenz vergrößert oder verkleinert; je größer die NF-Spannung, umso größer der Diodenstrom und umso kleiner der resultierende Widerstand. In einem Amplituden-Modulator wird dieser Widerstand eingesetzt, um die Amplitude eines HF-Signals (aus einem Lokaloszillator) zu beeinflussen; der HF-Strom durch die Diode wird groß, wenn der Dioden-Widerstand klein ist und umgekehrt. Das HF-Signal wird in seiner Amplitude im Takt des NF-Signals „moduliert“! Im einfachsten Fall, wenn man nur eine einzige Diode verwendet, enthält das Spektrum des Signals einen Träger (bei der ursprünglichen HF-Frequenz) und zwei Modulations-Seitenbänder im Abstand der NF-Frequenz oberhalb und unterhalb der Trägerfrequenz – ein Signal mit Amplituden-Modulation (AM). 

Dieses Prinzip wird in der folgenden Frage deutlich: Eine Diode wird mit einem NF-Signal und einem HF-Signal gleichzeitig beaufschlagt und das Ausgangs-Signal wird mit einem LC-Schwingkreis ausgefiltert.

[question:AD507]

Mit einer Schaltung aus vier Dioden in einer Ring-Anordnung kann aber der Träger auch unterdrückt werden, und nur die beiden Seitenbänder bleiben übrig; dazu muss der Dioden-Ring in eine Gegentakt- Schaltung eingebaut sein, die so ausbalanciert (bzw. symmetriert) ist, dass sich die Ströme des Trägersignals am Ausgang aufheben. Im Kapitel "Mischer II" wurde so eine Schaltung als „Balancemischer“ (engl. „balanced mixer“) bereits gezeigt, allerdings dort zur Umsetzung eines HF-Eingangssignals in eine Zwischenfrequenz-Lage. 

Der Balancemodulator ist die erste Stufe eines Einseitenband-Modulators - er erzeugt aus einem Lokaloszillator-Signal und einem NF-Signal (Modulation) ein Doppelseitenband-Signal (DSB). Dahinter folgt ein Bandpass-Filter, das nur eines der beiden Seitenbänder durchlässt, und damit am Ausgang ein SSB-Signal erzeugt.  

Man denke an die beiden notwendigen Stufen des SSB-Modulators.

[question:AE206]

[question:AF302]

---

Man erkennt einen Balancemischer bzw. Balancemodulator an dem Dioden-Ring. In dieser Schaltung besteht keine vollständige Gegentakt Anregung, da nur ein Transformator verwendet wird, allerdings gibt es das Äquivalent zu einer Mittelanzapfung eines Transformators in der Einspeisung des Oszillator-Signals im Mittelpunkt eines Spannungsteilers (Poti).

[question:AF308]

<indepth>
Im Sender wird aus dem Balancemischer ein Balancemodulator durch Vertauschung der Eingänge: Die niederfrequente Modulation wird in den Brückenzweig der Gegentakt-Schaltung zwischen der Mittelanzapfung von T2 und Masse eingekoppelt. Das Lokaloszillator-Signal wird über T1 in den Diodenring eingespeist und das Doppelseitenband-Signal über T2 ausgekoppelt. Ohne eine Modulations-Spannung werden die Dioden-Paare D1, D2 und D3, D4 abwechselnd durchgeschaltet und bilden dabei 1:1 - Spannungsteiler, so dass ihre Mittelpunkte auf Masse-Potential liegen. Somit liegen auch abwechselnd das obere und untere Ende der Wicklung von T2 auf Masse-Potential während das jeweils andere Ende der Wicklung durch gesperrte Dioden ohne Verbindung bleibt. Somit fließt kein Strom in der Wicklung und auf der Ausgangsseite entsteht keine Spannung - das macht die "Trägerunterdrückung" aus!

Bei Anlegen einer Modulationsspannung fließt zusätzlicher Strom durch die Dioden, so dass das Mittelpunkts-Potential der Spannungsteiler verschoben wird - damit kann Strom in den Transformator T2 fließen und ein Ausgangssignal entsteht. Im Bild werden die Spannungsverläufe gezeigt, die sich ergeben, wenn das Oszillator-Signal vereinfacht als Rechteck-Funktion angenommen wird.
</indepth>

---

Träger-Unterdrückung hat mit Auslöschung eines unerwünschten Signals zu tun - dazu muss eine Modulator-Schaltung "ausbalanciert" sein.

[question:AD510]

Genau zu dieser Ausbalancierung gehört eine Justierung der Amplituden (Poti) und der Phasen (C-Trimmer)

[question:AF309]

"Symmetriert" oder "ausbalanciert" wird ein Modulator, um den Träger zu unterdrücken - die Modulations-Seitenbänder werden dabei nicht unterdrückt.

[question:AF304]

[question:AF303]

Hinter dem Balancemodulator folgt die zweite Stufe eines SSB-Modulators.

[question:AF305]

[question:AF306]

Die Quarze bestimmen die Frequenz des durch den Balancemodulator unterdrückten Trägers. Man erkennt an der Quarzfrequenz für das untere Seitenband (LSB): Der Träger liegt $\qty{1,5}{\kilo\hertz}$ über der $\qty{9}{\mega\hertz}$-Bandfilter-Mittenfrequenz. Mit der maximalen NF-Frequenz von $\qty{3}{\kilo\hertz}$ liegt das untere Seitenband dann $\qty{1,5}{\kilo\hertz}$ unter der Mittenfrequenz und die NF-Frequenz $\qty{200}{\hertz}$ legt das Seitenband dann bei $\qty{1,3}{\kilo\hertz}$ über der Mittenfrequenz des Filters. Für das obere Seitenband (USB) gilt das umgekehrt.

[question:AF307]

Das Kreuz- oder X-Symbol in dem Funktionsblock hinter dem NF-Verstärker steht für die mathematische Multiplikation - Modulatoren, Demodulatoren und Mischer-Schaltungen werden so gekennzeichnet, weil ihre Funktion mathematisch als die Multiplikation von Signal-Funktionen beschrieben werden kann.

Ein Modulator für die Frequenzmodulation (FM) verwendet dagegen einen anderen Dioden-Typ, die Kapazitäts-Diode (in den Schaltungen erkennbar an dem kleinen Kondensator-Symbol neben dem Dioden-Symbol). Dabei ist die Diode immer Teil einer Oszillator-Schaltung, deren Schwingungsfrequenz durch einen Resonanzkreis bestimmt wird, der die Kapazitäts-Diode enthält. Die Diode wird mit einer Gleichspannung in Sperr-Richtung beaufschlagt, so dass sich eine feste Dioden-Kapazität einstellt und damit auch eine Oszillator-Frequenz. Zum Frequenz-Modulator wird die Schaltung, wenn der Gleichspannung ein NF-Signal überlagert wird – dann ändert der Oszillator seine Frequenz im Takt des NF-Signals.


Hier taucht die Kapazitäts-Diode auf - und die Transistor-Schaltung daneben ist ein Oszillator mit LC-Schwingkreis.

[question:AD508]

Eine in Sperrspannung betriebene Kapazitäts-Diode, die auf der einen Seite mit NF beaufschlagt wird und auf der anderen Seite parallel zum Schwingkreis einer Oszillator-Schaltung liegt, beeinflusst die Frequenz des Oszillators.

[question:AF310]

Mit großen NF-Spannungen kann man leicht viel größere Frequenzänderungen des Oszillators bewirken (FM-„Hub“) als zulässig. Daher ist eine „Hub“- Begrenzung durch eine Einstellung und Begrenzung der NF-Amplitude notwendig. Anti-parallel geschaltete Dioden begrenzen die Spannung auf etwa die Dioden-Knickspannung.

[question:AD509]

Dies ist offenbar kein Modulator - es gibt nur ein einziges Signal! Ein Elko am Ausgang der Diode deutet auf Gleichspannung hin!

[question:AD503]

% TODO aus E hier her kopiert ... muss eingeflegt werden.
<margin>
[picture:500:e_ssb_modulation:Blockschaltbild zur Modulation von SSB mit der Filtermethode]
[picture:831:e_ssb_modulation_lsb:Frequenzen mit der Filtermethode bei LSB]
[picture:940:e_ssb_modulation_lsb:Spektrum mit der Filtermethode bei LSB]
[picture:832:e_ssb_modulation_usb:Frequenzen mit der Filtermethode bei USB]
[picture:941:e_ssb_modulation_usb:Spektrum mit der Filtermethode bei USB]
</margin>