Jede ortsfeste Amateurfunkanlage muss bei einer Äquivalenten Isotropen Strahlungsleistung (EIRP) von $\qty{10}{\watt}$ oder mehr bei der BNetzA, nach § 9 BEMFV, angezeigt werden. Dies hat vor Aufnahme des Funkbetriebs zu geschehen. Der Funkamateur hat dabei den Nachweis zu erbringen, dass er die Grenzwerte einhält und die dazu notwendigen Sicherheitsabstände ermittelt hat und dass sie innerhalb des kontrollierten Bereichs liegen. Umgangssprachlich wird dies von Funkamateuren als *Selbsterklärung* bezeichnet.

Auf eine Selbsterklärung kann nur verzichtet werden, wenn die Äquivalente Isotrope Strahlungsleistung (EIRP) *kleiner* als $\qty{10}{\watt}$ EIRP ist - nicht $\qty{10}{\watt}$ Sendeleistung, auch nicht $\qty{10}{\watt}$ ERP!

Selbst ohne genaue Rechnung wird schnell deutlich, dass die Kombination aus $\qty{6}{\watt}$ Sendeleistung und einem Antennengewinn von $\qty{13}{\dBd}$ (Faktor 20) in der folgenden Frage den Grenzwert von $\qty{10}{\watt}$ EIRP deutlich überschreitet.

<indepth>
Zur Übung kann man das trotzdem Rechenen: Wir nutzen erneut die Formel aus der Formelsammlung: 

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a+\qty{2,15}{\dB}}{\qty{10}{\dB}}} = \qty{6}{\watt} \cdot 10^{\frac{\qty{13}{dBd}+\qty{2,15}{\dB}}{\qty{10}{\dB}}} \approx \qty{197}{\watt}$

Auch diese Rechnung lässt sich wieder leicht im Kopf durchführen, indem man den Gesamtgewinn in einzelne sinvolle Anteile zerlegt:
  
$\qty{13}{\dBd} + \qty{2,15}{\dB} = \qty{10}{\dBd} + \qty{3}{\dB} + \qty{2,15}{\dB}$

So ergibt sich:

$P_\text{EIRP} = \qty{6}{\watt} \cdot 10 \cdot 2 \cdot 1,64 \approx \qty{197}{\watt}$
</indepth>

[question:EK104]
  
In der [Anleitung zur Durchführung der Anzeige ortsfester Amateurfunkanlagen nach §9 der BEMFV](https://50ohm.de/abemfv) ist genau festgelegt, was unter dem Sicherheitsabstand zu verstehen ist. Der standortbezogene Sicherheitsabstand beschreibt den erforderlichen Abstand zwischen der Bezugsantenne und dem Bereich, in dem die geltenden Grenzwerte eingehalten werden müssen. Dabei sind auch die relevanten Feldstärken umliegender ortsfester Funkanlagen zu berücksichtigen.

Wichtig ist dabei: Der Sicherheitsabstand bezieht sich nicht auf einen einzelnen Punkt der Antenne, sondern auf die gesamte Antennenstruktur. Mit anderen Worten, für jeden Punkt der Antenne muss sichergestellt sein, dass außerhalb des berechneten Sicherheitsabstands die Grenzwerte eingehalten werden.

[question:EK107]
