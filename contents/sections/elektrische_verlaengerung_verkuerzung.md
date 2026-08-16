Bei Antennen müssen wir zwischen der *mechanischen* und der *elektrischen Länge* unterscheiden. Die mechanische Länge ist einfach die tatsächlich messbare Länge des Antennendrahtes oder Strahlers. Die elektrische Länge beschreibt dagegen, wie lang die Antenne bei der betrachteten Frequenz elektrisch wirkt. Sie kann unter anderem durch Spulen und Kondensatoren verändert werden, ohne dass die mechanische Länge des Strahlers geändert werden muss.

Betrachten wir zunächst Antennen in der Nähe ihrer Grundresonanz. Ein Halbwellendipol ist ungefähr bei einer Gesamtlänge von $\lambda/2$ resonant, eine Groundplane mit einem einzelnen vertikalen Strahler ungefähr bei einer Strahlerlänge von $\lambda/4$. Ist eine solche Antenne für die gewünschte Frequenz zu kurz, besitzt ihre Speiseimpedanz einen *kapazitiven* Blindanteil. Eine Spule kann diesen kapazitiven Blindanteil kompensieren. Man spricht dann von einer *elektrischen Verlängerung* der Antenne. Ist die Antenne dagegen für die gewünschte Frequenz zu lang, besitzt ihre Speiseimpedanz einen *induktiven* Blindanteil. Dieser kann mit einem Kondensator kompensiert werden. Man spricht dann von einer *elektrischen Verkürzung*. Eine Spule verlängert eine Antenne also elektrisch, ein Kondensator verkürzt sie elektrisch. Die mechanische Länge des Strahlers bleibt dabei unverändert.

<margin>
[picture:1134:a_5_8_lambda_strahlung:Strahlungsmuster und Stromverteilung von Vertikalantennen bei idealer Erde]
</margin>

---

Ein interessantes Beispiel ist die $\frac{5}{8}\lambda$-Vertikalantenne mit einer Länge von umgerechnet $\qty{0.625}{\lambda}$ (vgl. Abbildung [ref:a_5_8_lambda]). Der Strahler ist damit mechanisch etwa 2,5-mal so lang wie der einer normalen $\frac{\lambda}{4}$-Groundplane ($\qty{0.25}{\lambda}$). Die größere Strahlerlänge verändert das vertikale Strahlungsdiagramm vorteilhaft, wie in Abbildung [ref:a_5_8_lambda_strahlung] dargestellt: Mehr von der abgestrahlten Leistung wird in Richtung Horizont gebündelt, weniger wird nach oben oder unten abgestrahlt. Das ergibt bei terrestrischen Verbindungen bei gleicher Leistung in der Regel eine höhere Reichweite. Eine Strahlerlänge von etwa $\frac{5}{8} \lambda$ ist für diesen Effekt optimal: Wird der Strahler weiter verlängert, geht wieder mehr Leistung nach oben und unten verloren.

Allerdings ist diese Antenne bei der Strahlerlänge von $\frac{5}{8}\lambda=\qty{0.625}{\lambda}$ nicht resonant. Für Resonanz müsste die Strahlerlänge auf $\frac{\lambda}{2}=\qty{0.5}{\lambda}$ verkürzt oder auf $\frac{3}{4}\lambda=\qty{0.75}{\lambda}$ verlängert werden. Beides würde zu weniger Leistung am Horizont führen. Es empfiehlt sich, wegen der besseren Bündelung die Strahlerlänge bei $\frac{5}{8}\lambda$ zu lassen und die Resonanz elektrisch herzustellen, die Antenne also elektrisch zu verlängern. Eine von mehreren Möglichkeit dazu ist eine Fusspunktspule. Die Spule liefert einen induktiven Blindanteil, der den kapazitiven Blindanteil des $\frac{5}{8}\lambda$-Strahlers kompensiert. Die damit erreichte Impedanz ist sehr ähnlich der Impedanz einer Antenne mit Strahlerlänge $\frac{3}{4}\lambda=\qty{0.75}{\lambda}$. 

<margin>
[picture:650:a_5_8_lambda:$\qty{5}{8}\lambda$-Vertikalantenne]
</margin>

[question:AG106]

---

Umgekehrt kann eine Antenne, die in der Nähe ihrer Grundresonanz mechanisch etwas zu lang ist, durch einen Kondensator elektrisch verkürzt werden (vgl. Abbildung [ref:a_verkuerzung]). Der Kondensator liefert einen kapazitiven Blindanteil und kompensiert damit den induktiven Blindanteil des zu langen Strahlers.

[question:AG107]

<margin>
[picture:563:a_verkuerzung:Vertikalantenne mit Verkürzungskondensator]
</margin>

---

Bei einem Dipol lässt sich ebenfalls zunächst anhand seiner mechanischen Länge abschätzen, ob für die gewünschte Grundresonanz eine elektrische Verlängerung oder Verkürzung erforderlich ist.

[question:AG108]