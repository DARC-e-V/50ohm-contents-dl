Das Schaltnetzteil wurde in Klasse N und E schon einführend erklärt. Nun betrachten wir das vereinfachte Blockschaltbild genauer.
<margin>
[picture:35:a_schaltnetzteil:Prinzipschaltbild Schaltnetzteil]
</margin>

% AUS KLASSE E:
% Die Wechselspannung wird zuerst gleichgerichtet und dann mit einem elektronischen Schalter mit hoher Schatfrequenz (z.B. 120 kHz) zerhackt. Die höherfrequente Wechselspannung lässt sich nun mit einem kleinen Ferritkernübertrager ohne große Verluste auf einen anderen Spannungswert übertragen. Danach erfolgt wieder eine Gleichrichtung und Stabilisierung der Gleichspannung. Die Gleichspannungsstabilisierung erfolgt über einen Regelkreis von der Sekundärseite des Trafos auf die Primärseite, wobei die Schaltzeit des Schalttransistors verändert wird. Die Schaltfrequenz bleibt dabei konstant. Diese Regelung nennt man auch Pulsbreitenmodulation (PWM).  Da der Schalttransistor entweder gesperrt oder sehr niederohmig leitend betrieben wird, gibt es an ihm kaum Wärmeverluste.

<margin>
[photo:264:a_innenansicht_eines_schaltnetzteils:Innenansicht eines Schaltnetzteils]
</margin>
Der wichtige elektronische Schalter im Block E dient auch zur Regelung auf eine konstante Ausgangsspannung.
Da es keine Zustände zwischen leitendem und gesperrtem Transistor gibt, muss es eine andere Möglichkeit zur Regelung geben. Der Energietransport von der Eingangsseite auf die Lastseite kann durch die Schaltzeit variiert werden. Ist der Schalter länger geschlossen, dann wird mehr Energie zur Lastseite transportiert und die Ausgangsspannung steigt an. Um dies festzustellen, ist eine Rückmeldung der Ausgangsspannung an den Steuerblock des elektronischen Schalters erforderlich. Diese Rückführung fehlt im dargestellten, vereinfachten Schaltbild. Die Regelung der Ausgangsspannung geschieht nun über den sogenannten Impulsbreitenmodulator. Dies bedeutet, dass der leitende Zustand des Schalters verändert wird, die Schaltfrequenz bleibt dabei konstant. 

[question:AD311]

Wichtig ist auch die galvanische Trennung der Eingangs- und Ausgangsseite, um Netzspannungspotentiale vom Ausgang fernzuhalten. Diese Netztrennung geschieht durch den Übertrager mit Ferritkern. 
Siehe Abbildung [ref:a_innenansicht_eines_schaltnetzteils]. 
Die Veränderung der Schaltzeit bewirkt zusätzliche Störsignale, die unbedingt von der Netzspannungsseite ferngehalten werden müssen, damit sie sich nicht über das Stromnetz ausbreiten und andere elektronische Geräte stören. Das Stromnetz wirkt auch wie eine Antenne und kann deshalb Störsignale als elektromagnetische Welle abstrahlen. Wird der elektronische Schalter mit einer Schaltfrequenz von 30 kHz betrieben, dann ergibt sich ein Störspektrum, in dem alle 30 kHz ein Störsignal erscheint.

[question:AD312]
---


In jedem Schaltnetzteil muss ein hochwertiges Tiefpassfilter auf der Seite des Anschlusses zum 230V Wechselspannungsnetzes eingebaut sein. Der typische Aufbau des Filters ist hier zu sehen.
[picture:367:a-schaltnetzteilfilter:Filter am 230V Eingang eines Schaltnetzteils]
Vergleiche auch die Filter in Abbildung [ref:a_EMV_Filter1] und [ref:a_EMV_Filter2]
*Merke:* Der PE-Leiter darf nicht mit dem L1-Leiter oder dem N-Leiter verbunden sein.
Die Drossel T darf keine Transformatorfunktion für die Netzwechselspannung bewirken.

[question:AD314]
[question:AD313]
Bei ungenügend entstörten Schaltnetzteilen beinträchtigt das Störspektrum den Funkempfang.
<margin>
[photo:277:a_störspektrum:Störspektrum eines Schaltnetzteils]
Das Störspektrum wurde direkt oberhalb des Schaltnetzteilgehäuses empfangen. In 1m Entfernung ist das Störspektrum kaum messbar.

%todo: Audioton einer Schaltnetzteilstörung
</margin>

<margin>
EMV Filter = Funkentstörfilter gegen leitungsgebundene Störungen
[photo:242:a_EMV_Filter1: Funkentstörfilter Filter für ein Schaltnetzteil]
[photo:243:a_EMV_Filter2: Filter direkt am 230 V  AC Spannungseingang]
</margin>

<tip>
  Es gibt ein Experiment zur Erkundung unterschiedlicher Störquellen.
</tip>