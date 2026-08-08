Ein Low Noise Block Converter (LNB) wird häufig bei der Verarbeitung von hohen Frequenzen im $\unit{\giga\hertz}$-Bereich beim Amateurfunkverkehr über Satelliten verwendet. Abbildung [ref:a_lnb] zeigt eine mögliche Implementierung einer QO-100-Station. Hierbei wird die sehr hohe Empfangsfrequenz, die typischerweise durch einen SAT-Spiegel empfangen wird, bereits direkt im LNB auf eine deutlich niedrigere Frequenz heruntergemischt, um hohe Kabelverluste, die bei hohen Frequenzen auftreten würden, zu vermeiden.

<margin>
[picture:1094:a_lnb:LNB (blau) und Bias-T (rot) in einem QO-100 Transceiver]
</margin>

[question:AF230]

Bei einem LNB handelt es sich um eine aktive Komponente, welche eine Spannungsversorgung benötigt. Diese erfolgt meist direkt über das Koaxialkabel, welches zum LNB führt. Hierfür wird in der Empfangsstelle ein sog. Bias-T in das Koaxialkabel eingebaut. Seine Aufgabe ist die Gleichspannungsversorgung des LNBs sowie die Trennung der Gleichspannung vom HF-Signal im weiteren Signalweg hin zum Empfänger.
Ein LNB kann entweder horizontal oder vertikal polarisierte Signale empfangen. Die Umschaltung zwischen den beiden Polarisationsrichtungen erfolgt hierbei über die Höhe der Betriebsspannung mit welcher das LNB versorgt wird. Übliche Werte sind hier z.B. $\qty{12}{\volt}$ und $\qty{18}{\volt}$.

[question:AF231]