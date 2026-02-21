Gehen wir nun etwas genauer auf den Gegenspieler des A/D-Umsetzers - den D/A-Umsetzer - ein. Der D/A-Umsetzer erzeugt aus einem in digitalen Daten vorliegenden Datenstrom (Samples) wiederum ein analoges Signal. Hierbei kann der D/A-Umsetzer natürlich ebenso wie der A/D-Umsetzer nicht beliebig genaue Amplituden-Werte erzeugen, sondern hat genau so wie der A/D-Umsetzer eine maximale Auflösung (in Bits). Hierdurch gibt es ebenfalls wieder eine endliche Anzahl von analogen Signalwerten, die der D/A-Umsetzer erzeugen kann. Die Anzahl der möglichen Stufen errechnet sich wie schon zuvor beschrieben beim A/D-Umsetzer.

[question:AF609]

Ein D/A-Umsetzer kann immer nur Spannungen in einem bestimmten Spannungsbereich (z. B. von $\qty{0}{\volt}$ bis $\qty{1}{\volt}$ oder von $\qty{-2}{\volt}$ bis $\qty{2}{\volt}$) generieren. Hierbei verteilt sich die Anzahl der vorbeschriebenen Stufen (Auflösung des D/A-Umsetzers) bei einem linear arbeitenden D/A-Umsetzer (linear bedeutet hier, dass der Abstand zwischen den einzelnen Stufen immer gleich ist) auf den Spannungsbereich. Hat der D/A-Umsetzer z. B. eine Auflösung von nur $\qty{4}{\bit}$, so haben wir $\num{16}$ mögliche Stufen. Diese verteilen sich dann z. B. auf einen Spannungsbereich (Wertebereich) von $\qty{0}{\volt}$ bis $\qty{1}{\volt}$. Um die Schrittweite zwischen zwei Stufen zu errechnen, muss man den Spannungsbereich nur durch die Anzahl der möglichen Stufen teilen. Dies ergibt z. B. bei unserem vorgenannten Beispiel einen Abstand (Schrittweite) von $\qty{6,25}{\milli\volt}$.

[question:AF611]
[question:AF610]

