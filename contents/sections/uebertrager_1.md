Warum gibt es ein $\qty{230}{\volt}$-Wechselspannungsnetz? Wechselspannung bietet gegenüber Gleichspannung einen entscheidenden Vorteil: Sie lässt sich mithilfe von Transformatoren einfach und mit geringen Verlusten auf andere Spannungswerte umsetzen. Dadurch ist eine effiziente Anpassung der Spannung für Übertragung und Nutzung möglich.

Auf Grund der Selbstinduktion in Spulen läßt sich Energie bei Wechselspannung zwischen zwei Spulen, wie in Abbildung [ref:e_netztrafo] gezeigt, übertragen. Es entsteht ein neues Bauelement, der *Übertrager* oder *Transformator*, kurz *Trafo*. Er besteht aus zwei Spulen, die über einen Eisen- oder Ferritkern magnetisch gekoppelt sind. Damit die Seiten auseinandergehalten werden können, spricht man von Primärseite mit der Windungszahl $N_P$ und der Sekundärseite mit der Windungszahl $N_S$.

<margin>
[picture:1017:e_netztrafo:Schaltbild Transformator]
</margin>

<margin>
[photo:239:e_Trafo mit getrennten Wicklungen:Trafo mit sichtbar getrennten Wicklungen]
</margin>

Ein Transformator dient zur Umsetzung einer hohen Wechselspannung z. B. $\qty{230}{\volt}$ in eine 
niedrigere Wechselspannung z. B. $\qty{13,8}{\volt}$. Ein Transformator kann nur Wechselspannungen übertragen. Legt man unerlaubt eine Gleichspannung an einen Transformator an, wirkt dieser aufgrund des geringen ohmschen Widerstands der Primärwicklung wie ein Kurzschluss. Der Transformator kann dadurch stark überhitzen und im schlimmsten Fall durchbrennen.

---

Das Übersetzungsverhältnis eines Transformators lässt sich wie folgt angeben:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S}$

Das Verhältnis der Windungszahlen entspricht somit dem Verhältnis der Spannungen. Durch Umstellen dieser Grundgleichung lassen sich sowohl die Spannungen $U$ als auch die Windungszahlen $N$ auf der Primär- oder Sekundärseite berechnen.

<indepth>
Diese Beziehungen gelten für den Idealfall eines unbelasteten Transformators, also für den sogenannten Leerlauffall. Leerlauf bedeutet, dass an der Sekundärseite keine Last angeschlossen ist.
</indepth>

[question:EC401]

Wir rechnen: 

$ü = \frac{15}{1} = 15 = \frac{\qty{230}{\volt}}{U_S} \quad\quad\quad |~\cdot~U_S$

$15 \cdot U_S = \qty{230}{\volt} \quad\quad\quad |~:~15$

$U_S = \frac{\qty{230}{\volt}}{15} = \qty{15,33}{\volt}$ 

[question:EC402]

Wir stellen erstmal fest, dass $N_P = 5\cdot N_S$ und das $U_P = \qty{230}{\volt}$ gegeben ist. Gesucht ist wieder die Spannung $U_S$.

$ü = \frac{5\cdot N_S}{N_S} = \frac{\qty{230}{\volt}}{U_S}$ 

Die $N_S$ kürzen sich weg so bleibt nur übrig:

$ü = 5 = \frac{\qty{230}{\volt}}{U_S}$ 

Wir multiplizieren auf beiden Seiten mit $U_S$ und teilen auf beiden Seiten durch 5.

$U_S = \frac{\qty{230}{\volt}}{5}$ 

Bei der Folgenden Frage ist die Sekundärwindungszahl gesucht. 

[question:EC403]

Gegeben ist $N_P=600$, $U_P=\qty{230}{\volt}$ und $U_S=\qty{11,5}{\volt}$. Gesucht wird die Sekundärwindungszahl $N_S$.

$\frac{600}{N_S} = \frac{\qty{230}{\volt}}{\qty{11,5}{\volt}}$ 

Das vereinfacht sich zu:

$\frac{600}{N_S} = 20$ 

Wir multiplizieren auf beiden Seiten mit $N_S$ und teilen auf beiden Seiten durch 20.

$N_S = \frac{600}{20} = 30$

Der folgende Trafo setzt die Ausgangsspannung $U_S$ hoch, deshalb muss die Sekundärwindungszahl größer als die Primärwindungszahl sein.

[question:EC404]

Gegeben ist $N_P= 150$, $U_P=\qty{45}{\volt}$ und  $U_S=\qty{180}{\volt}$. Gesucht wird $N_S$.

Wir setzen ein:

$ \frac{150}{N_S} = \frac{\qty{45}{\volt}}{\qty{180}{\volt}}$

Dies vereinfacht sich zu 

$ \frac{150}{N_S} =0,25 $

Wir multiplizieren wieder auf beiden Seiten mit $N_S$ und teilen auf beiden Seiten durch $0,25$.

$ N_S= \frac{150}{0,25} = 600$