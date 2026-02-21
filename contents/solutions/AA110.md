# Gegeben
Pegel: $\qty{0}{\dBm}$, $\qty{3}{\dBm}$, $\qty{20}{\dBm}$  

# Lösungsweg
Wir nutzen die $\unit{\dBm}$-Formel aus der Formelsammlung (Pegel, Leistungs- und Spannungspegel):  
$ p = 10 \cdot \log_{10}\left(\frac{P}{\qty{1}{\milli\watt}}\right)\unit{\dBm}$ 
und lösen nach $P$ auf:
$P = \qty{1}{\milli\watt}\cdot 10^{\frac{p}{\qty{10}{\dBm}}}$
Wir setzten die Werte aus der Frage ein und erhalten:  

$P = \qty{1}{\milli\watt}\cdot 10^{\frac{\qty{0}{\dBm}}{\qty{10}{\dBm}}}= \qty{1}{\milli\watt}\cdot 10^{0}= \qty{1}{\milli\watt}$

$P = \qty{1}{\milli\watt}\cdot 10^{\frac{\qty{3}{\dBm}}{\qty{10}{\dBm}}}= \qty{1}{\milli\watt}\cdot 10^{0,3}= \qty{1,995}{\milli\watt}$

$P = \qty{1}{\milli\watt}\cdot 10^{\frac{\qty{20}{\dBm}}{\qty{10}{\dBm}}}= \qty{1}{\milli\watt}\cdot 10^{2}= \qty{100}{\milli\watt}$

# Abkürzung
Wer ein wenig mit Logarithmen und der Tabelle aus den Hilfsmittel gearbeitet hat, kann im Ausschlussverfahren schnell zur korrekten Lösung gelangen.  
$\qty{0}{\dBm} \rightarrow \qty{1}{\milli\watt}$ (damit bleiben nur noch zwei mögliche Antworten).  
$\qty{3}{\dB}$ entsprechen einer Verdopplung. Damit entsprechen $\qty{3}{\dBm} \rightarrow  \qty{2}{\milli\watt}$ (damit bleibt nur noch eine Antwort übrig). 
