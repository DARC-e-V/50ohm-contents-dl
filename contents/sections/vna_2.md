In der Klasse E haben wir bereits den *vektoriellen Netzwerkanalysator* (VNA) kennengelernt (vgl. Abbildung [ref:a_vna_swr]). In der Klasse A wollen wir uns seine Funktionsweise etwas genauer ansehen.

Für eine Messung erzeugt der VNA zunächst ein HF-Signal mit einer festgelegten Startfrequenz und gibt dieses an das Messobjekt, beispielsweise eine Antenne oder einen Schwingkreis, aus. Anschließend misst er das vom Messobjekt zurückkommende beziehungsweise reflektierte Signal. Dabei werden sowohl dessen Amplitude als auch dessen Phase erfasst. Um den Einfluss von Störungen zu verringern, können für einen Frequenzpunkt auch mehrere Messungen durchgeführt und gemittelt werden.

Nach der Messung wird die Frequenz um einen festgelegten Schritt erhöht und der Vorgang wiederholt. Auf diese Weise durchläuft der VNA schrittweise den gesamten Bereich von der Start- bis zur Stoppfrequenz. Man bezeichnet diesen Vorgang auch als *Frequenz-Sweep*, oder früher gelegentlich auch als *Wobbeln*.

Aus den Messwerten für die einzelnen Frequenzpunkte kann der VNA verschiedene Größen bestimmen und über der Frequenz darstellen. Dazu gehören beispielsweise die Impedanz des Messobjekts und das Stehwellenverhältnis (SWR). So lässt sich beispielsweise unmittelbar erkennen, bei welchen Frequenzen eine Antenne gut angepasst ist beziehungsweise eine Resonanz besitzt.

<margin>
[photo:323:a_vna_swr:SWR-Messung einer Endgespeisten Drahtantenne. Das SWR ist nahezu $1$ bei $\qty{14}{\mega\hertz}$]
[picture:526:a_vna_swr_2:Möglicher SWR-Verlauf einer Antenne.]
</margin>

[question:AI201]
[question:AI202]
[question:AI203]

---

Eine mögliche Anzeigeform des VNAs ist die Aufteilung der Impedanz in Wirk- und Blindanteil (Wirkwiderstand $R$ und Blindwiderstand $X$). Der Wirkwiderstand wird oft in $\unit{\ohm}$ und der Blindwiderstand gelegentlich auch als $j\unit{\ohm}$ angegeben. Die Anzeigen verschiedener Geräte sind nicht einheitlich. Das $j$ entstammt einer Schreibweise aus der Elektrotechnik, bei der dieses für die sogenannte imaginäre Einheit ($i$) der Mathematik steht. Positive Blindwiderstände stehen für induktives und negative Blindwiderstände für kapazitives Verhalten.

<indepth>
*Imaginäre Zahlen* sind ein beliebtes Hilfsmittel in der Elektrotechnik und der Mathematik. Um Gleichungen wie $x^2 = -1$ lösen zu können, hat man sich eine sogenannte imaginäre Zahl ($i$) ausgedacht, die mit sich selbst multipliziert eine negative Zahl ergibt: $i^2 = -1$. Keine reelle Zahl erfüllt eine solche Gleichung, da eine negative Zahl mal einer negativen Zahl eine positive Zahl ist. Deshalb bezeichnet man $i$ als "imaginär". Diese "ausgedachte" Zahl ergibt mit sich selbst multipliziert eine negative Zahl, nämlich $-1$. Addiert man reelle Zahlen (z. B. $54$) mit einer imaginären Zahl (z. B. $-12i$), so ergibt sich eine komplexe Zahl: $54 - 12i$. Eine komplexe Zahl kann z. B. verwendet werden, um einen Wirk- und Blindanteil eines Widerstands zu beschreiben. Auch kann man komplexe Zahlen in eine Amplitude und eine Phase umrechnen. Anstelle des Buchstabens $i$ verwendet man in der Elektrotechnik den Buchstaben $j$, um eine Verwechselung mit dem Formelzeichen $i$ (für Ströme) zu vermeiden.
</indepth>

[question:AI204]
[question:AI205]
[question:AI206]

---

Viele VNAs verfügen über die Möglichkeit, den SWR-Verlauf über die Frequenz grafisch darzustellen. Liegt die Resonanzfrequenz einer Antenne zu tief, weiß man, dass diese gekürzt werden sollte. Liegt sie zu hoch, dann müsste die Antenne verlängert werden.

[question:AI207]
[question:AI208]