In den Klassen N und E haben wir das SWR und die entsprechenden Formeln für die vorlaufende und rücklaufende Leistung kennen gelernt. In vielen Fällen kann man das Stehwellenverhältnis einfach angeben, wenn der Speisewiderstand einer Antenne bekannt ist. Sofern sich eine Antenne (oder Dummy-Load) weder induktiv noch kapazitiv verhält, sie also einen reinen Wirkwiderstand ($R_a$) darstellt, ergibt sich das Stehwellenverhältnis aus dem Verhältnis zwischen Lastwiderstand und Wellenwiderstand der Leitung, wobei Zähler und Nenner so zu wählen sind, dass sich ein SWR von größer gleich eins ergibt.

Die Abbildung [ref:a_swr] zeigt die Spannungsverteilung einer stehenden Welle auf einer Leitung. An bestimmten Stellen erreicht die Spannung ein Maximum $U_\mathrm{max}$, an anderen ein Minimum $U_\mathrm{min}$. Der Abstand zwischen zwei benachbarten Spannungsmaxima beziehungsweise zwei benachbarten Spannungsminima beträgt dabei jeweils $\frac{\lambda}{2}$. Aus dem Verhältnis von maximaler zu minimaler Spannung lässt sich auch das Stehwellenverhältnis bestimmen:

Mathematisch ausgedrückt bedeutet dies:

$s = \frac{U_\mathrm{max}}{U_\mathrm{min}} = \begin{cases} \dfrac{R_a}{Z}, & \text{für } R_a > Z, \\[6pt] 1, & \text{für } R_a = Z, \\[6pt] \dfrac{Z}{R_a}, & \text{für } R_a < Z. \end{cases}$

<margin>
[picture:978:a_swr:Stehende Welle]
</margin>

Eine Antenne mit einem Speisewiderstand von $\qty{100}{\ohm}$ verursacht bei Speisung mit einem $\qty{50}{\ohm}$ Kabel ein Stehwellenverhältnis von $\num{2}$, da der Speisewiderstand doppelt so groß ist. Eine Antenne mit einem Speisewiderstand von $\qty{10}{\ohm}$ hätte ein Stehwellenverhältnis von $\num{5}$, da der Wellenwiderstand der Leitung fünf mal so groß ist.

Zur Beantwortung der folgenden Frage müssen wir uns außerdem daran erinnern, dass der Widerstand eines Faltdipols knapp $\qtyrange{240}{300}{\ohm}$ beträgt.

[question:AG405]

Ein trügerischer Effekt ist die Auswirkung von Leitungsdämpfung auf das Stehwellenverhältnis. Je mehr Verluste eine Leitung aufweist, umso kleiner (also "besser") kann das Stehwellenverhältnis auf dieser Leitung ausfallen. Dies liegt daran, dass eine verlustbehaftete Leitung sowohl die vorlaufende als auch die rücklaufende Leistung reduziert. Selbst wenn am Ende einer Leitung keine Antenne angeschlossen ist (Leerlauf oder Kurzschluss), und dort $\qty{100}{\percent}$ der Energie reflektiert wird, also das Stehwellenverhältnis dort $\infty$ beträgt, so kann man am anderen Ende ein deutlich besseres Stehwellenverhältnis messen. Geht z. B. in Hin-Richtung die Hälfte der Leistung verloren und in Rück-Richtung erneut die Hälfte verloren, so reduziert sich die Energie auf ein Viertel ($\frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4}$). Entsprechend zeigt ein Stehwellenmessgerät an der Senderseite des Kabels ein Stehwellenverhältnis von $\num{3}$ an, was $\qty{25}{\percent}$ reflektierter Leistung entspricht, obwohl am Ende $\qty{100}{\percent}$ reflektiert werden – es kommen jedoch nur $\qty{25}{\percent}$ am Stehwellenmessgerät an.

[question:AG402]
[question:AG403]

Bei einer Leitungsdämpfung von $\qty{5}{\dB}$ und vollständiger Reflektion am Ende des Kabels, z. B. aufgrund einer abgeklemmten Antenne, messen wir gar ein überraschend gutes SWR, obwohl gar keine Antenne angeschlossen ist! Dies können wir wie folgt berechnen:

$s = \frac{\sqrt{P_\mathrm{v}}+\sqrt{P_\mathrm{r}}}{\sqrt{P_\mathrm{v}}-\sqrt{P_\mathrm{r}}}$

Damit lässt sich die folgende Frage berechnen, sofern wir beachten, dass die gemessene rücklaufende Welle nur ein Zehntel der Energie der vorlaufenden Welle ausmacht: $\qty{5}{\dB}$ Dämpfung in Hin-Richtung und $\qty{5}{\dB}$ Dämpfung in Rück-Richtung, entsprechend $\qty{10}{\dB}$ Dämpfung insgesamt. $P_\mathrm{r}$ ist also in diesem Falle nur ein Zehntel von $P_\mathrm{v}$.

[question:AG404]
