In der Klasse E haben wir gelernt, das ein Oszilloskop stellt den zeitlichen Verlauf von Spannungen darstellt. Wir können also mit einem Oszilloskop Signalverläufe prüfen. 

[question:AI301]

<margin>
[picture:1005:a_impulsbreite:Bestimmung der Impulsbreite eines nicht-idealen Rechtecksignals]
</margin>

---

Neben den Sinusförmingen Wechselspannugen kommen durch die Digitaltechnik auch  rechteckförmige Spannungen vor.  Einen exakt rechteckigen Spannungsverlauf kann es aber nicht geben. Die Kanten sind immer ein bisschen schräg oder verformt. Die Zeit zwischen dem Ansteigen und dem Abfallen eines Rechtecks, die man Pulsbreite oder Impulsdauer nennt, wird deshalb immer bei halber Höhe, also bei 50% der Spannung, gemessen. So  ist sichergestellt, dass beim gleichen Signal alle zum gleichen Messergebnis kommen.

<indepth>
Grund für diese Verformungen sind die unvermeidlichen Kapazitäten und Induktivitäten in Leitungen und Bauteilen, die wie Filter wirken und die hohen Frequenzanteile eines Rechtecksignals dämpfen.
</indepth>

[question:AI303]
[question:EI303]


Oszilloskope können Signale mit unterschiedlichsten Frequenzen und Verläufen darstellen. Damit diese Signale auf dem Bildschirm stabil erscheinen, besitzen Oszilloskope eine sogenannte Triggereinrichtung (engl. trigger = „auslösen“). Dabei überwacht das Gerät das Eingangssignal kontinuierlich und startet die Aufnahme genau dann, wenn eine zuvor festgelegte Bedingung erfüllt ist – zum Beispiel, wenn das Signal eine bestimmte Spannung, die sogenannte Triggerspannung, überschreitet. Ab diesem Moment beginnt die Abtastung und Speicherung der Messwerte, die anschließend als Kurve auf dem Bildschirm dargestellt werden.


Durch dieses Verfahren startet jede Darstellung stets am gleichen Signalzustand, sodass periodische Signale wie Sinusschwingungen oder Rechteckimpulse scheinbar eingefroren und klar erkennbar sind. Digitale Oszilloskope können darüber hinaus auch Einzelbilder anzeigen, den Bildschirm also „einfrieren“. Das erleichtert die Analyse nichtperiodischer Signale. Die dafür vorgesehene Taste ist meist mit SINGLE beschriftet. Außerdem lassen sich mehrere Messungen überlagern, um beispielsweise zeitliche Schwankungen eines Signals (engl. jitter) sichtbar zu machen.

[question:AI302]

%<indepth>
%Abbildung [ref:a_oszilloskop_einzelbild] zeigt ein Einzelbild aus der Musikaufnahme von Abbildung [ref:a_oszilloskop_ueberlagerung]. Es wurde von einem älteren Oszilloskop abfotografiert, das hauptsächlich analog arbeitet und zusätzlich einen kleinen digitalen %Speicher besitzt.
%[photo:222:a_oszilloskop_einzelbild:Einzelbild aus einer Musikaufnahme]
%</indepth>

Nicht jede Leitung eignet sich für Hochfrequenzsignale – das gilt auch für die Verbindung zwischen Messobjekt und Oszilloskop. Dafür verwendet man in der Regel sogenannte Tastköpfe. Sie stellen die Verbindung her und sorgen dafür, dass das Signal möglichst unverfälscht übertragen wird, ohne die Schaltung stark zu belasten. Dazu reduzieren sie die Signalspannung (z. B. im Verhältnis 10:1), passen Widerstand und Kapazität an und enthalten oft eine Kompensation für hohe Frequenzen.

Ein Tastkopf besteht aus einem griffähnlichen Gehäuse, vergleichbar mit einem Kugelschreiber. An seiner Spitze können verschiedene Haken oder Nadeln angebracht werden, um die Messstelle zu kontaktieren. Die Masseverbindung erfolgt über eine Krokodilklemme (siehe Abbildung [ref:a_oszilloskop_messung]). Abbildung [ref:a_oszilloskop_tastkoepfe] zeigt drei Beispiele solcher Tastköpfe. Hochwertige Modelle sind entsprechend teuer, da sie hohe Bandbreiten, minimale Signalverfälschung und eine präzise Mechanik bieten müssen.

<margin>
[photo:224:a_oszilloskop_messung:Messung mit einem Tastkopf. Zwischen den Dioden D1 und D2 ist die Prüfspitze zu sehen und weiter links die Krokodilklemme für die Masseverbindung.]
</margin>

<margin>
[photo:223:a_oszilloskop_tastkoepfe:Tastköpfe mit verschiedenen Prüfspitzen. Die Krokodilklemmen wurden für diese Aufnahme abgenommen.]
</margin>

Die einfachsten Tastköpfe verbinden die Prüfspitze direkt mit dem Messeingang. Man spricht von 1:1-Tastköpfen, weil die an der Spitze anliegende Spannung unverändert zum Oszilloskop gelangt. Tastköpfe für hohe Frequenzen sind aufwändiger gebaut. Sie teilen die Eingangsspannung auf einen kleineren Wert, oft ein Zehntel, herunter. Wenn man mit so einem 10:1-Tastkopf eine Spannung von 10 Volt misst, wird auf dem Bildschirm 1 Volt angezeigt.

<indepth>
Bei manchen Oszilloskopen kann man einstellen, welches Teilverhältnis der Tastkopf hat. Dann wird auf dem Bildschirm die tatsächliche Spannung anzezeigt. Passive 10:1-Tastköpfe enthalten unter anderem einen $\qty{9}{\mega\ohm}$-Widerstand, der im Signalweg liegt. Oszilloskope haben in der Regel einen Innenwiderstand von $\qty{1}{\mega\ohm}$. So ergibt sich ein 10:1-Spannungsteiler. Außerdem ist im Tastkopf oder im Stecker ein kleiner Drehkondensator vorhanden. Er dient zur Anpassung der Kapazität von Tastkopf und Kabel an den Messeingang und wird so eingestellt, dass ein Rechtecksignal möglichst unverfälscht auf dem Bildschirm erscheint. Neben den hier beschriebenen, passiven Tastköpfen existieren mehrere andere Varianten. Es gibt zum Beispiel Tastköpfe mit angepasstem $\qty{50}{\ohm}$-Koaxkabel. Sie sind besonders gut für sehr hohe Frequenzen geeignet, haben aber nur einen relativ kleinen Innenwiderstand. Aktive Ausführungen lösen dieses Problem, indem das Signal direkt im Tastkopf verstärkt wird.
</indepth>
