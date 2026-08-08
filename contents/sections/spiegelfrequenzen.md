Konzeptbedingt entstehen bei einem Überlagerungsempfänger durch den hierbei stattfindenden Mischprozess (vgl. Abbildung [ref:spiegelfrequenzen_mischen1]) mit der Oszillatorfrequenz des Empfängers immer zwei mögliche Empfangsfrequenzen:

$f_\text{ZF} = \left|f_\text{e} \pm f_\text{o}\right|$

Da wir im Überlagerungsempfänger auf eine niedrigere Zwischenfrequenz heruntermischen wollen, ist hier insbesondere die Differenzfrequenz interessant:

$f_\text{ZF} = \left|f_\text{e} - f_\text{o}\right|$

Der Betrag ist dabei entscheidend: Für eine feste Oszillatorfrequenz $f_\text{o}$ und Zwischenfrequenz $f_\text{ZF}$ gibt es zwei mögliche Empfangsfrequenzen, die beide dieselbe Zwischenfrequenz erzeugen. Eine davon ist die gewünschte Empfangsfrequenz, die andere wird als *Spiegelfrequenz* bezeichnet.

<margin>
[picture:807:spiegelfrequenzen_mischen1:Mischvorgang mit Empfangsfrequenz $f_\text{e}$, Oszillatorfrequenz $f_\text{o}$ und der Zwischenfrequenz $f_\text{ZF}$]
</margin>

---

<margin>
[picture:806:spiegelfrequenzen_fe1_fe2:Empfangsfrequenzen, die beide zur selben $f_\text{ZF}$ führen]
</margin>

Beispiel: Nehmen wir an, unser Oszillator schwingt, wie in Abbildung [ref:spiegelfrequenzen_fe1_fe2] gezeigt, auf der Frequenz $f_\text{o}=\qty{3,955}{\mega\hertz}$. Die Zwischenfrequenz $f_\text{ZF}$ soll $\qty{0,455}{\mega\hertz}$ betragen. Durch den Betrag in unserer Formel gibt es nun zwei Möglichkeiten, welche Empfangsfrequenzen man hören kann, nämlich $f_\text{e1} = \qty{3,500}{\mega\hertz}$ und $f_\text{e2} = \qty{4,410}{\mega\hertz}$. Für beide Werte ergibt die Formel die Zwischenfrequenz $f_\text{ZF}$.

Wenn $f_\text{e1}$ die gewünschte Empfangsfrequenz ist, so wird $f_\text{e2}$ die Spiegelfrequenz von $f_\text{e1}$ genannt. Ist $f_\text{e2}$ die gewünschte Empfangsfrequenz, so wird $f_\text{e1}$ die Spiegelfrequenz von $f_\text{e2}$ genannt.

Der Abstand zwischen gewünschter Empfangsfrequenz und Spiegelfrequenz beträgt hierbei immer das Doppelte der Zwischenfrequenz (ZF), wie man in der Abbildung [ref:spiegelfrequenzen_fe1_fe2] leicht sehen kann. 

Schwingt der Oszillator *oberhalb* der Empfangsfrequenz ($f_\mathrm{E} < f_\mathrm{OSZ}$) so befindet sich auch die Spiegelfrequenz um das doppelte der ZF *oberhalb* der Empfangsfrequenz ($f_\mathrm{S} = f_\mathrm{E} + 2\cdot f_\mathrm{ZF}$).

Befindet sich der Oszillator hingegen *unterhalb* der Empfangsfrequenz ($f_\mathrm{E} > f_\mathrm{OSZ}$) so befindet sich auch die Spiegelfrequenz um das doppelte der ZF *unterhalb* der Empfangsfrequenz ($f_\mathrm{S} = f_\mathrm{E} - 2\cdot f_\mathrm{ZF}$). Diesen Zusammenhang findet man auch in der Formelsammlung. 

Versuche nun mit diesem Wissen die folgenden Fragen zu lösen.

[question:AF106]
[question:AF201]
[question:AF202]
[question:AF203]
[question:AF107]
[question:AF108]

---
<margin>
[picture:808:spiegelfrequenzen_mischen2:Zusätzlicher Bandpassfilter zur Spiegelfrequenzunterdrückung]
</margin>

Die Spiegelfrequenz kann bei unzureichender Unterdrückung zu Empfangsstörungen führen, da Signale auf der Spiegelfrequenz ebenfalls auf die gleiche Zwischenfrequenz umgesetzt werden und dadurch im Empfänger hörbar werden können. Um dies zu vermeiden, wird die gewünschte Empfangsfrequenz, wie in Abbildung [ref:spiegelfrequenzen_mischen2] gezeigt, bereits vor dem Mischer mit einem Bandpassfilter selektiert. Die Spiegelfrequenz soll dabei möglichst stark unterdrückt werden.

Für eine wirksame Spiegelfrequenzunterdrückung ist ein möglichst großer Abstand zwischen gewünschter Empfangsfrequenz und Spiegelfrequenz vorteilhaft. Dieser Abstand wird größer, wenn eine höhere Zwischenfrequenz gewählt wird.

Dies lässt sich auch anhand von Abbildung [ref:spiegelfrequenzen_fe1_fe2] erkennen: Mit zunehmender ZF liegen die beiden möglichen Empfangsfrequenzen $f_\text{e1}$ und $f_\text{e2}$ weiter auseinander.

Je größer dieser Frequenzabstand ist, desto leichter kann der vorgeschaltete Bandpass die gewünschte Empfangsfrequenz passieren lassen und die Spiegelfrequenz gleichzeitig stark dämpfen. Bei einem sehr kleinen Abstand müsste das Filter dagegen wesentlich steilere Flanken beziehungsweise eine höhere Selektivität besitzen. Die Anforderungen an die Vorselektion des Empfängers wären dadurch deutlich höher.

[question:AF109]
[question:AF110]
[question:AF111]
[question:AF204]