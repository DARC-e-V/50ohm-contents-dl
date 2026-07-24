In der Klasse E haben wir bereits Konverter und Transverter kennengelernt, welche im Amateurfunk dazu eingesetzt werden, um mit vorhandenen Funkgeräten zusätzliche Frequenzbereiche zu erschließen, die diese Geräte ursprünglich nicht abdecken. Wie in Abbildung [ref:a_konverter_2] gezeigt, benötigt man hierzu einen Oszillator, einen Mischer und ein Bandfilter.  

[question:AF301]

Ein Problem dabei, welches wir nun vertiefen wollen, ist, dass die Amateurfunkbänder verschiedene Breiten haben. So ist z.B. das $\qty{70}{\centi\meter}$-Band von $\qtyrange{430}{440}{\mega\hertz}$ mit einer Breite von $\qty{10}{\mega\hertz}$ deutlich breiter als das $\qty{10}{\meter}$-Band von $\qtyrange{28}{29,7}{\mega\hertz}$ mit einer Breite von $\qty{1,7}{\mega\hertz}$. Dies hat zur Folge, dass ein Konverter, der den Frequenzbereich von $\qtyrange{430}{440}{\mega\hertz}$ auf den Frequenzbereich von $\qtyrange{28}{30}{\mega\hertz}$ umsetzt, nicht die gesamte Bandbreite des $\qty{70}{\centi\meter}$-Bands abdecken kann.

<margin>
[picture:651:a_konverter_2:Up-Konverter für QO-100]
</margin>

---

Deshalb muss ein Konverter ggf. umschaltbar sein, wie in Abbildung [ref:a_konverter] gezeigt, um größere Frequenzbereiche abbilden zu können. Soll z. B. ein Frequenzbereich von $\qtyrange{436}{440}{\mega\hertz}$, also $\qty{4}{\mega\hertz}$ Bandbreite, auf einen Frequenzbereich von $\qtyrange{28}{30}{\mega\hertz}$ mit $\qty{2}{\mega\hertz}$ umgesetzt werden (bei Annahme, dass sich die Oszillatorfrequenz unterhalb des Nutzsignals befindet), so benötigt man zwei umschaltbare Frequenzbereiche: den ersten von $\qtyrange{436}{438}{\mega\hertz}$ und den zweiten von $\qtyrange{438}{440}{\mega\hertz}$. 

<margin>
[picture:85:a_konverter:Konverter mit Umschaltung der Oszillatorfrequenz]
</margin>

Für den ersten Teilbereich von $\qtyrange{436}{438}{\mega\hertz}$ kann man folgende Oszillatorfrequenz berechnen: 

$f_\mathrm{OSZ} = \qty{436}{\mega\hertz}$ - $\qty{28}{\mega\hertz} = \qty{408}{\mega\hertz}$

$f_\mathrm{OSZ} = \qty{438}{\mega\hertz}$ - $\qty{30}{\mega\hertz} = \qty{408}{\mega\hertz}$

Für beide Bandgrenzen ergibt sich logischerweise eine Oszillatorfrequenz von $\qty{408}{\mega\hertz}$.

Für den zweiten Teilbereich von $\qtyrange{438}{440}{\mega\hertz}$ ergibt sich folgende Oszillatorfrequenz:

$f_\mathrm{OSZ} = \qty{440}{\mega\hertz} - \qty{30}{\mega\hertz} = \qty{438}{\mega\hertz} - \qty{28}{\mega\hertz} = \qty{410}{\mega\hertz}$.

Wird diese Oszillatorfrequenz mittels Frequenzvervielfachung erzeugt, so muss man sie bei der Rückrechnung auf die benötigte Frequenz des Quarzoszillators noch durch Teilen berücksichtigen.

Werden die oben berechneten $\qty{408}{\mega\hertz}$ bzw. $\qty{410}{\mega\hertz}$ durch Verneunfachung der Quarz-Oszillatorfrequenz gewonnen, so ergeben sich die beiden Quarz-Oszillatorfrequenzen zu $f_\mathrm{Quarz,1}=\frac{\qty{408}{\mega\hertz}}{9} = \qty{45,333}{\mega\hertz}$ und $f_\mathrm{Quarz,2}=\frac{\qty{410}{\mega\hertz}}{9} = \qty{45,556}{\mega\hertz}$ (jeweils gerundet).

Mit diesem Wissen können wir nun die folgenden Aufgaben bearbeiten.

[question:AF501]
[question:AF502]