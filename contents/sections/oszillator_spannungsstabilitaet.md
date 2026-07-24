Die Frequenz eines VFOs ist von seiner Betriebsspannung (Gleichspannung) direkt abhängig. Dies wird vor allem durch die Abhängigkeit des Arbeitspunktes des Transistors in dessen Oszillator hervorgerufen.
Zur Erreichung einer möglichst hohen Frequenzstabilität eines VFOs gegenüber Schwankungen in der Betriebsspannung ist diese möglichst gut durch geeignete schaltungstechnische Maßnahmen in deren *Spannung zu stabilisieren*. Die Betriebsspannung eines VFOs sollte daher unabhängig von Betriebsspannungen anderer Stufen sein (stabilisiert) und möglichst gut *gefiltert und entkoppelt* sein. Dies kann z.B. durch einen Festspannungsregler erreicht werden (vgl. Abbildung [ref:a_osc_stab]).

[question:AD612]
[question:AD608]
[question:AD607]

<margin>
[picture:200:a_osc_stab:Festspannungsregler]
</margin>

---

Bei schlechter Spannungsstabilisierung der Betriebsspannung kann es bei sehr einfachen CW-Sendern zu einer Tonhöhenstörung kommen, die als *Chirp* bezeichnet wird: Zu Beginn jedes einzelnen Dits oder Dahs ist die Tonhöhe zunächst etwas höher oder etwas tiefer und nähert sich dann der eigentlichen Tonhöhe an. Das englische Wort „Chirp" bedeutet wörtlich übersetzt „Zwitschern". Wenn sich die Tonhöhe von oben annähert, hat der akustische Effekt tatsächlich etwas von Zwitschern.

[question:AD609]

<margin>
Hier ein Beispiel für ein solches Chirp-Signal:

[include:applet_chirp_1]

Ein weiteres Beispiel, ein QSO zwischen RA1OW und OM3YCY, bei dem der Chirp-Effekt im zweiten Druchgang deutlich zu hören ist:

[include:applet_chirp_2]

</margin>