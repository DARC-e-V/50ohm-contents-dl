Bei einer PLL-Frequenzsynthese wird die Ausgangsfrequenz des VCO im Rückkopplungszweig durch den Teiler *:n* heruntergeteilt und am Phasendetektor $\varphi$ mit der Referenzfrequenz an Punkt A verglichen.

Der Regelkreis sorgt dafür, dass am Phasendetektor beide Eingangsfrequenzen gleich groß sind:

$f_A = \frac{f_{VCO}}{n}$

bzw.

$f_{VCO} = n \cdot f_A$

Der Teilerfaktor *n* wird über die Eingänge B und C eingestellt und ist immer eine *ganze Zahl*. Erhöht man *n* um genau 1, so springt die Ausgangsfrequenz um genau $f_A$ weiter:

$\Delta f_{VCO} = (n+1) \cdot f_A - n \cdot f_A = f_A$

Der kleinstmögliche Frequenzschritt am Ausgang – also der *Kanalabstand* – entspricht damit direkt der Referenzfrequenz an Punkt A.

Da ein Kanalabstand von $\qty{12,5}{\kilo\hertz}$ gefordert ist, muss die Frequenz an Punkt A ebenfalls

$f_A = \qty{12,5}{\kilo\hertz}$

betragen.