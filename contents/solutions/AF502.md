Der Frequenzbereich von $\qtyrange{430}{434}{\mega\hertz}$ besitzt eine Bandbreite von $\qty{4}{\mega\hertz}$. Da der angeschlossene Empfänger jedoch nur den Bereich von $\qtyrange{28}{30}{\mega\hertz}$ und damit eine Bandbreite von $\qty{2}{\mega\hertz}$ verarbeitet, muss der gewünschte Empfangsbereich in zwei Teilbereiche aufgeteilt werden:

* Teilbereich 1: $\qtyrange{430}{432}{\mega\hertz}$
* Teilbereich 2: $\qtyrange{432}{434}{\mega\hertz}$

Da die Oszillatorfrequenz unterhalb des Nutzsignals liegen soll, gilt für die Mischung:

$f_\mathrm{ZF} = f_\mathrm{HF} - f_\mathrm{OSZ}$

Für den ersten Teilbereich von $\qtyrange{430}{432}{\mega\hertz}$ ergibt sich:

$f_\mathrm{OSZ} = \qty{430}{\mega\hertz} - \qty{28}{\mega\hertz} = \qty{402}{\mega\hertz}$

Auch an der oberen Bandgrenze erhalten wir:

$f_\mathrm{OSZ} = \qty{432}{\mega\hertz} - \qty{30}{\mega\hertz} = \qty{402}{\mega\hertz}$

Für den zweiten Teilbereich von $\qtyrange{432}{434}{\mega\hertz}$ ergibt sich entsprechend:

$f_\mathrm{OSZ} = \qty{432}{\mega\hertz} - \qty{28}{\mega\hertz} = \qty{404}{\mega\hertz}$

Auch an der oberen Bandgrenze erhalten wir:

$f_\mathrm{OSZ} = \qty{434}{\mega\hertz} - \qty{30}{\mega\hertz} = \qty{404}{\mega\hertz}$

Die benötigten Oszillatorfrequenzen betragen somit $\qty{402}{\mega\hertz}$ und $\qty{404}{\mega\hertz}$.

Da diese Frequenzen durch eine Verneunfachung der Quarzoszillatorfrequenz erzeugt werden, müssen sie durch den Faktor $\num{9}$ geteilt werden:

$f_\mathrm{Quarz,1} = \frac{\qty{402}{\mega\hertz}}{9} \approx \qty{44,667}{\mega\hertz}$

$f_\mathrm{Quarz,2} = \frac{\qty{404}{\mega\hertz}}{9} \approx \qty{44,889}{\mega\hertz}$

Der Quarzoszillator muss daher zwischen $\qty{44,667}{\mega\hertz}$ und $\qty{44,889}{\mega\hertz}$ umschaltbar sein.