Bei Antennen müssen wir zwischen der *mechanischen* und der *elektrischen Länge* unterscheiden. Die mechanische Länge ist einfach die tatsächlich messbare Länge des Antennendrahtes oder Strahlers. Die elektrische Länge beschreibt dagegen, wie lang die Antenne bei der betrachteten Frequenz elektrisch wirkt. Sie kann unter anderem durch Spulen und Kondensatoren verändert werden, ohne dass die mechanische Länge des Strahlers geändert werden muss.

Betrachten wir zunächst Antennen in der Nähe ihrer Grundresonanz. Ein Halbwellendipol ist ungefähr bei einer Gesamtlänge von $\lambda/2$ resonant, eine Groundplane mit einem einzelnen vertikalen Strahler ungefähr bei einer Strahlerlänge von $\lambda/4$.

Ist eine solche Antenne für die gewünschte Frequenz zu kurz, besitzt ihre Speiseimpedanz einen *kapazitiven* Blindanteil. Eine Spule kann diesen kapazitiven Blindanteil kompensieren. Man spricht dann von einer *elektrischen Verlängerung* der Antenne.

Ist die Antenne dagegen für die gewünschte Frequenz zu lang, besitzt ihre Speiseimpedanz einen *induktiven* Blindanteil. Dieser kann mit einem Kondensator kompensiert werden. Man spricht dann von einer *elektrischen Verkürzung*.

Eine Spule verlängert eine Antenne also elektrisch, ein Kondensator verkürzt sie elektrisch. Die mechanische Länge des Strahlers bleibt dabei unverändert.

---

Ein interessantes Beispiel ist die $\frac{5}{8}\lambda$-Vertikalantenne. Bei einer normalen Groundplane ist der vertikale Strahler ungefähr $\frac{1}{4}\lambda=0{,}25\lambda$ lang. Bei einer $\frac{5}{8}\lambda$-Vertikalantenne beträgt die mechanische Länge des Strahlers dagegen $\frac{5}{8}\lambda=0{,}625\lambda$.

Der Strahler ist damit mechanisch etwa $\num{2,5}$-mal so lang wie bei einer normalen $\lambda/4$-Groundplane. Die größere Strahlerlänge verändert das vertikale Strahlungsdiagramm und bündelt die abgestrahlte Leistung stärker in Richtung Horizont (vgl. [ref:a_5_8_lambda_strahlung]). Dies kann beispielsweise für terrestrische Funkverbindungen von Vorteil sein.

Obwohl der $\frac{5}{8}\lambda$-Strahler mechanisch deutlich länger als ein $\lambda/4$-Strahler ist, ist er bei dieser Länge noch nicht resonant und besitzt am Speisepunkt einen kapazitiven Blindanteil. Die nächste geeignete Resonanz liegt bei ungefähr $\frac{3}{4}\lambda=0{,}75\lambda$. Zwischen $\frac{5}{8}\lambda$ und $\frac{3}{4}\lambda$ fehlt elektrisch noch $\frac{3}{4}\lambda-\frac{5}{8}\lambda =\frac{1}{8}\lambda$. Durch die Spule am Fußpunkt wird der Strahler deshalb *elektrisch verlängert*. Die Spule liefert einen induktiven Blindanteil, der den kapazitiven Blindanteil des $\frac{5}{8}\lambda$-Strahlers kompensiert.

<margin>
[picture:1134:a_5_8_lambda_strahlung:Strahlungsmuster und Stromverteilung von Vertikalantennen bei idealer Erde]
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