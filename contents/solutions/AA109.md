# Gegeben
Sender-Ausgangsleistung: $p_\text{Sender, Ausgang} = \qty{1}{\watt}$  
Verstärkung: $g_\text{Endstufe} = \qty{10}{\dezibel}$  

# Lösungsweg
Wir nutzen die $\unit{\dBm}$-Formel aus der Formelsammlung (Pegel, Leistungs- und Spannungspegel):  
$ p = 10 \cdot \log_{10}\left(\frac{P}{\qty{1}{\milli\watt}}\right)\unit{\dBm}$ 
und berechnen damit den Eingangspegel in die Endstufe:
$ p_\text{Endstufe, Eingang} = 10 \cdot \log_{10}\left(\frac{p_\text{Sender, Ausgang}}{\qty{1}{\milli\watt}}\right)\unit{\dBm}= 10 \cdot \log_{10}\left(\frac{\qty{1}{\watt}}{\qty{10^{-3}}{\watt}}\right)\unit{\dBm} \\ = 10 \cdot \log_{10}\left(10^{3}\right)\unit{\dBm}= 10 \cdot \qty{3}{\dBm}\\ = \qty{30}{\dBm}$ 
Der Ausgangspegel ergibt sich dann durch einfach Addition zu:
$ p_\text{Ausgang} = p_\text{Eingang} + g_\text{Verstärkung} = \qty{30}{\dBm} + \qty{10}{\dB} = \qty{40}{\dBm}$

# Abkürzung
Wer ein wenig mit Logarithmen und der Tabelle aus den Hilfsmittel gearbeitet hat, kann die Lösung im Kopf ausrechnen.  
$\qty{1}{\watt}$ entsprechen $\qty{1000}{\milli\watt}$ entsprechen $\qty{30}{\dBm}$ zuzüglich der Verstärkung von $\qty{10}{\dezibel}$ ergeben $\qty{40}{\dBm}$.