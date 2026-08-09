Die *Frequenzgenauigkeit* gibt an, wie stark eine erzeugte, eingestellte oder gemessene Frequenz von ihrem tatsächlichen Wert abweichen kann. Sie wird häufig in Prozent ($\unit{\percent}$), in *parts per million* ($\unit{\ppm}$) oder direkt als relative Abweichung angegeben.

Dabei gilt:

$\qty{1}{\percent} = 1 \cdot 10^{-2}$

und

$\qty{1}{\ppm} = 1 \cdot 10^{-6}$

Bei einem Frequenzzähler hängt die erreichbare Genauigkeit wesentlich von seiner *Zeitbasis* ab. Der Frequenzzähler bestimmt die Frequenz des Eingangssignals mithilfe einer internen Referenzfrequenz. Weicht diese Referenz von ihrem Sollwert ab, wirkt sich diese Abweichung entsprechend auf das Messergebnis aus.

Als Zeitbasis werden deshalb möglichst stabile Oszillatoren eingesetzt. Hochwertige Frequenzzähler verwenden beispielsweise einen TCXO oder OCXO. Für besonders genaue Messungen kann häufig auch eine externe Frequenzreferenz angeschlossen werden, beispielsweise ein GPS-disziplinierter Oszillator (GPSDO).

Ist die relative Frequenzgenauigkeit bekannt, kann daraus die maximal zu erwartende Frequenzabweichung berechnet werden:

$\Delta f = f \cdot a$

Dabei ist $f$ die betrachtete Frequenz und $a$ die relative Frequenzgenauigkeit.

<indepth>
  Hinweis bzgl. Umrechnung/Darstellung von 10er Potenzen:
  
  $1 \cdot {\num{10^{-2}}} = \frac{1}{\num{10^2}}$
  $1 \cdot {\num{10^{-6}}} = \frac{1}{\num{10^6}}$
  
  usw.
</indepth>
  
[question:AA115]

[question:AA116]

[question:AI508]

[question:AI509]

[question:AI510]

[question:AI506]

[question:AI507]
