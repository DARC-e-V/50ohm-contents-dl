Das Schaltnetzteil wurde in Klasse N und E schon einführend erklärt. Nun betrachten wir das vereinfachte Blockschaltbild genauer.

<margin>
[picture:35:a_schaltnetzteil:Prinzipschaltbild Schaltnetzteil]
</margin>

Der wichtige elektronische Schalter im Block E dient auch zur Regelung auf eine konstante Ausgangsspannung.
Da es keine Zustände zwischen leitendem und gesperrtem Transistor gibt, muss es eine andere Möglichkeit zur Regelung geben. Der Energietransport von der Eingangsseite auf die Lastseite kann durch die Schaltzeit variiert werden. Ist der Schalter länger geschlossen, dann wird mehr Energie zur Lastseite transportiert und die Ausgangsspannung steigt an. Um dies festzustellen, ist eine Rückmeldung der Ausgangsspannung an den Steuerblock des elektronischen Schalters erforderlich. Diese Rückführung fehlt im dargestellten, vereinfachten Schaltbild. Die Regelung der Ausgangsspannung geschieht nun über den sogenannten Impulsbreitenmodulator. Dies bedeutet, dass der leitende Zustand des Schalters verändert wird, die Schaltfrequenz bleibt dabei konstant. 

---

[question:AD311]

Wichtig ist auch die galvanische Trennung der Eingangs- und Ausgangsseite, um Netzspannungspotentiale vom Ausgang fernzuhalten. Diese Netztrennung geschieht durch den Übertrager mit Ferritkern. 
Siehe Abbildung [ref:a_innenansicht_eines_schaltnetzteils]. 

<margin>
[photo:264:a_innenansicht_eines_schaltnetzteils:Innenansicht eines Schaltnetzteils]
</margin>

---

Die Veränderung der Schaltzeit bewirkt zusätzliche Störsignale, die unbedingt von der Netzspannungsseite ferngehalten werden müssen, damit sie sich nicht über das Stromnetz ausbreiten und andere elektronische Geräte stören. Das Stromnetz wirkt auch wie eine Antenne und kann deshalb Störsignale als elektromagnetische Welle abstrahlen. Wird der elektronische Schalter mit einer Schaltfrequenz von $\qty{30}{\kilo\hertz}$ betrieben, dann ergibt sich ein Störspektrum, in dem alle $\qty{30}{\kilo\hertz}$ ein Störsignal erscheint. Die Abbildung [ref:a_störspektrum] zeigt das Störspektrum eines Schaltnetzteils. Das Störspektrum wurde direkt oberhalb des Schaltnetzteilgehäuses empfangen. In $\qty{1}{\meter}$ Entfernung ist das Störspektrum kaum messbar.

[question:AD312]

Bei ungenügend entstörten Schaltnetzteilen beeinträchtigt das Störspektrum den Funkempfang.

[question:AD313]

<margin>
[photo:277:a_störspektrum:Störspektrum eines Schaltnetzteils]
</margin>

---

Um zu verhindern, dass Störungen in das Stromnetz gelangen, muss im Schaltnetzteil ein hochwertiges Tiefpassfilter auf der Seite des Anschlusses zum $\qty{230}{\volt}$ Wechselspannungsnetzes eingebaut sein. Der typische Aufbau des Filters ist in der Abbildung [ref:a-schaltnetzteilfilter] zu sehen.

<margin>
[picture:367:a-schaltnetzteilfilter:Filter am $\qty{230}{\volt}$ Eingang eines Schaltnetzteils]
</margin>

Vergleiche auch die Filter in Abbildung [ref:a_EMV_Filter1] und [ref:a_EMV_Filter2]
*Merke:* Der PE-Leiter darf nicht mit dem L1-Leiter oder dem N-Leiter verbunden sein.
Die Drossel T darf keine Transformatorfunktion für die Netzwechselspannung bewirken.

[question:AD314]


<margin>
EMV Filter = Funkentstörfilter gegen leitungsgebundene Störungen
[photo:242:a_EMV_Filter1: Funkentstörfilter Filter für ein Schaltnetzteil]
[photo:243:a_EMV_Filter2: Filter direkt am $\qty{230}{\volt}$ AC Spannungseingang]
</margin>