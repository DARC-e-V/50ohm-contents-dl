%TODO ggf. das Kapitel wo anders hinschieben 

Im Kapitel Dezibel wurde schon angedeutet, dass die Zusätze $\unit{\dBd}$ und $\unit{\dBi}$, die bei der Angabe von Antennengewinnen verwendet werden. In diesem Fall bezieht sich der Dezibelwert nicht auf eine Leistung oder Spannung, sondern auf einen bestimmten Referenzstrahler. Üblich sind dabei $\unit{\dBi}$, bezogen auf den isotropen Kugelstrahler, sowie $\unit{\dBd}$, bezogen auf den Halbwellendipol.

Der *Isotropstrahler* (vgl. Abbildung [ref:e_Kugelstrahler]) ist eine gedachte, hypothetische Antenne, die in alle Richtungen gleich stark abstrahlt. Weist eine real vorhandene Antenne eine Richtwirkung auf, so ist die Abstrahlung in bestimmten Richtungen stärker und in anderen Richtungen schwächer als sie beim hypothetischen Isotropstrahler wäre. 

<margin> 
[picture:751:e_Kugelstrahler:Isotroper Strahler in der Mitte einer Kugel, der an allen Stellen der Kugeloberfläche die gleiche Strahlungsleistung erzeugt]
</margin>

Den Gewinn in einer Richtung (z.B. der Hauptstrahlrichtung welche die Richtung mit dem maximalen Antennengewinn ist) gegenüber einem Isotropstrahler kann man in Dezibel $\unit{\dB}$ angeben. Anstelle von $\unit{\dB}$ schreibt man $\unit{\dBi}$, um zu verdeutlichen, dass man sich auf den Isotropstrahler bezieht.

[question:EG220]

Auch ein einfacher Halbwellendipol hat einen Gewinn, denn er strahlt senkrecht zum Leiter um $\qty{2,15}{\dB}$ stärker ab, als es ein Isotropstrahler tun würde. Entsprechend hat ein Halbwellendipol einen Gewinn von $\qty{2,15}{\dBi}$.

Gelegentlich interessiert der Gewinn der über den Gewinn eines Halbwellendipols hinausgeht, also den Gewinn in Bezug auf einen Halbwellendipol. Diesen gibt man in $\unit{\dBd}$ an, wobei das $\text{d}$ für Dipol steht. Ein Halbwellendipol hat entsprechend einen Gewinn von $\qty{0}{\dBd}$. Antennen, die mehr Gewinn aufweisen, als ein Halbwellendipol haben einen Gewinn größer als $\qty{0}{\dBd}$ und Antennen mit weniger Gewinn als ein Halbwellendipol entsprechend weniger als $\qty{0}{\dBd}$.

Vergleichen wir noch einmal den Gewinn eines Halbwellendipols angegeben als $\unit{\dBi}$ und angegeben als $\unit{\dBd}$: Der Halbwellendipol hat in Hauptstrahlrichtung einen Gewinn von $\qty{2,15}{\dBi}$, da er gegenüber dem Isotropstrahler $\qty{2,15}{\dB}$ stärker strahlt. In $\unit{\dBd}$ angegeben sind es jedoch $\qty{0}{\dBd}$. Die Angabe in $\unit{\dBi}$ ist stets um $\qty{2,15}{\dB}$ höher als die Angabe in $\unit{\dBd}$.

Das steht auch in der Formelsammlung: 

$g_i = g_d + \qty{2,15}{\dB}$

[question:EG221]
