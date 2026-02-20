Ein einfaches Multimeter ist nicht geeignet, um frequenzabhängige Widerstände zu messen. Stattdessen kann man einen vektoriellen Netzwerkanalysator (VNA) verwenden. Hierbei handelt es sich um ein aktives Messgerät, welches für eine Vielzahl von Frequenzen (einen einstellbaren Frequenzbereich) bestimmt, wie sich Strom und Spannung zu einander Verhalten (Verhältnis der Amplituden und die Phasenverschiebung zwischen Spannung und Strom).

<margin>
[photo:201:e_vna_tiefpassmessung:Messung eines Tiefpassfilters von $\qty{0}{\mega\hertz}$ bis $\qty{100}{\mega\hertz}$ mit Grenzfrequenz bei $\qty{30}{\mega\hertz}$]
</margin>

---

So lässt sich beispielsweise bestimmen, bei welcher Frequenz ein Schwingkreis oder Filter einen besonders hohen oder besonders niedrigen Widerstand (bzw. Impedanz) aufweist (vgl. Abbildung [ref:e_vna_tiefpassmessung]). Ebenso kann ermittelt werden, bei welcher Frequenz eine Antenne in Resonanz ist, indem man das SWR über einen Frequenzbereich hinweg betrachtet, wie in Abbildung [ref:e_vna_swr] dargestellt.

<margin>
[photo:323:e_vna_swr:SWR-Messung einer Endgespeisten Drahtantenne. Das SWR ist nahezu $1$ bei $\qty{14}{\mega\hertz}$]
</margin>

[question:EI201]
[question:EI202]
[question:EI203]
[question:EI204]

Viele VNAs sollten vor der Benutzung kalibriert werden, um ein möglichst genaues Messergebnis zu erhalten.

[question:EI205]

---

Zur Kalibrierung als auch zum Funktionstest misst man oft die Zustände "offen" (unendlicher Widerstand), "Kurzschluss" (Widerstand nahe Null) und "angepasst" (Lastwiderstand entsprechend des Ausgangswiderstands des Messgeräts).

<margin>
[photo:327:e_vna_solt:SOL(T)-Kalibierkit. Von links nach rechts: Load, Open, Closed]
</margin>

Bei angeschlossenem Leitungsabschluss (z. B. $\qty{50}{\ohm}$ Abschlusswiderstand) sollte der VNA ein SWR von nahe $\num{1}$ anzeigen, da keine Leistung reflektiert wird. Ist nichts am Messanschluss angeschlossen oder wird dieser kurzgeschlossen, so ergibt sich ein SWR von nahe unendlich (vollständige Reflexion).

[question:EI206]