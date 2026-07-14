Die Frequenz eines VFOs ist von seiner Betriebsspannung (Gleichspannung) direkt abhängig. Dies wird vor allem durch die Abhängigkeit des Arbeitspunktes des Transistors in dessen Oszillator hervorgerufen.
Zur Erreichung einer möglichst hohen Frequenzstabilität eines VFOs gegenüber Schwankungen in der Betriebsspannung ist diese möglichst gut durch geeignete schaltungstechnische Maßnahmen in deren *Spannung zu stabilisieren*. Die Betriebsspannung eines VFOs sollte daher unabhängig von Betriebsspannungen anderer Stufen sein (stabilisiert) und möglichst gut *gefiltert und entkoppelt* sein.

[question:AD612]
[question:AD608]
[question:AD607]

<margin>
[picture:497:a_osc_stab:Oszillator, bei dem mit dem Kondensator oben links und der Drosselspule oben rechts die Betriebsspannung stabilisiert wird. Beide bilden einen Tiefpassfilter, der HF-Anteile überbrückt und so die Betriebsspannung entkoppelt und stabilisiert. Langsame Änderungen der Versorgungsspannung kann diese Schaltung nicht ausgleichen; hier könnte z. B. ein Spannungsregler eingesetzt werden.]
</margin>

---

Bei schlechter Spannungsstabilisierung der Betriebsspannung eines VFOs kann es zu impulsartigen Frequenzsprüngen im Rhythmus der Tastung des Senders kommen. Dies äußert sich insbesondere bei CW-Signalen als sog. *Chirp*, einem zwitschernden Geräusch zu Beginn von Zeichen.

[question:AD609]

<margin>
Hier ein Beispiel für ein solches Chirp-Signal:

[include:applet_chirp_1]
</margin>