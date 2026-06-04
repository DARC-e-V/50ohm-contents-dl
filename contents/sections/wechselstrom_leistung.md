Bei sinusförmigen Wechselstromsignalen wird die Leistung aus den Effektivwerten von Strom und Spannung berechnet. Es darf somit nicht einfach stattdessen die Spannung von Spitze zu Spitze $U_\text{SS}$, oder die Spitzenspannung $\hat{U}$ stattdessen eingesetzt werden.

<margin>
[picture:834:a_wechselstrom_leistung:Effektivwerte für die Leistungsberechnung]
</margin>

Somit ergibt sich für die Berechnung der Leistung
$P_\text{Wechselstrom} = U_\text{eff} \cdot I_\text{eff} = \dfrac{{U_\text{eff}}^2}{R} = I_\text{eff}^2 \cdot R$


Bei sinusförmigen Signalen gilt allerdings auch:

$U_\text{eff} = \dfrac {\hat{U}} {\sqrt{2}} = \dfrac {U_\text{SS}} {2 \cdot \sqrt{2}}$ 
$I_\text{eff} = \dfrac {\hat{I}} {\sqrt{2}} = \dfrac {I_\text{SS}} {2 \cdot \sqrt{2}}$ 

Entsprechend ergeben sich für sinusförmige Signale folgende Zusammenhänge, bei denen auch mit Spitzenwerten und Spitze-Spitze-Werten gerechnet werden können:

$\begin{split} P_\text{Wechselstrom} &=  U_\text{eff} \cdot I_\text{eff} \\ &= \frac{\hat{U}\cdot\hat{I}}{\sqrt{2}\cdot\sqrt{2}} = \frac{\hat{U} \cdot \hat{I}}{2} \\ &= \frac{U_\text{eff}^2}{R} = \left(\frac{\hat{U}}{\sqrt{2}}\right)^2 \cdot \frac{1}{R} = \frac{\hat{U}^2}{2 \cdot R} \\ &= I_\text{eff}^2 \cdot R = \left(\frac{\hat{I}}{\sqrt{2}}\right)^2 \cdot R = \frac{\hat{I}^2\cdot R}{2} \end{split}$

Die folgende Frage lässt sich mit diesen Überlegungen sehr leicht lösen ($I_\mathrm{max}$ ist dabei nur eine andere Bezeichnung für $\hat{I}$):

[question:AB301]

Im Amateurfunkbereich haben wir es mit Spannungen mit unterschiedlichen Frequenzen (z.B. Kilo- oder Gigahertz) und Wellenformen (Rechteckspannung, sinusförmige Spannung, Gleichspannung) zu tun. Diese können auch verzerrt sein und nicht als z.B. reine Sinusspannung vorliegen. Diese unterschiedlichen Spannungen erzeugen in einem Stromkreis unterschiedliche elektrische Ströme. Prinzipiell würde man nun verschiedene Geräte benötigen um diese Bandbreite an elektrischen Strömen mit einer vernüftigen Messgenauigkeit messen zu können. 

Im Amateurfunkbereich verwendet man deshalb oft einen sogenannten *Thermoumformer*.
Man nutzt hierbei aus, dass der Stromfluss den Leiterdraht erwärmt (vgl. Widerstand von Drähten). Je mehr Strom dabei fließt desto wärmer wird der Draht. Die Erwärmung ist also proportional zur Stromstärke. Der Thermoumformer misst diese Erwärmung und zeigt sie als Stromstärke an.  Zu beachten ist dabei, dass wir mit dieser Messmethode den *Effektivwert* der Stromstärke erhalten. Der Vorteil dabei ist nun, dass sich die Stromstärke nahezu *unabhängig* von der Wellenform oder Frequenz bestimmen lässt. Der Thermoumformer kann damit eine großen Bereich an Signalen abdecken. 

[question:AI105]
