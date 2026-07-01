In der Klasse E haben wir bereits die Grundlagen des Transformators kennengelernt. Er besteht aus zwei Spulen, die über einen Eisen- oder Ferritkern magnetisch gekoppelt sind. Damit die Seiten auseinandergehalten werden können, spricht man von Primärseite mit der Windungszahl $N_P$ und der Sekundärseite mit der Windungszahl $N_S$.

Das Transformatorprinzip beruht auf einem grundlegenden physikalischen Effekt: der elektromagnetischen Induktion. Ändert sich das Magnetfeld in einer Spule – wie es beim Anlegen einer Wechselspannung der Fall ist – so wird in einer benachbarten, magnetisch gekoppelten Spule eine elektrische Spannung induziert. Diese ist gemäß dem Induktionsgesetz so gerichtet, dass sie der Ursache ihrer Entstehung entgegenwirkt. Man spricht daher auch von *Gegeninduktion*.

[question:AC301]

In der Klasse E haben wir bereits die Formel für das Übersetzungsverhältnis $ü$ kennengelernt:

$ü = \frac{N_P}{N_S} = \frac{U_P}{U_S}$

Für die Ströme gilt entsprechend umgekehrt:

$ü = \frac{N_P}{N_S} = \frac{I_S}{I_P} = \frac{U_P}{U_S}$

Mit dieser Formel, die auch in der Formelsammlung zu finden ist, kann die nächste Frage gelöst werden:

[question:AC302]

---

Da stromführende Leitungen nicht übermäßig erwärmt werden dürfen, um Schäden an der Isolation oder sogar ein Glühen des Leiters zu vermeiden, darf eine bestimmte maximale Stromstärke in Abhängigkeit vom Leiterquerschnitt nicht überschritten werden. Setzt man die Stromstärke in Bezug zum Leiterquerschnitt in $\unit{\milli\meter\squared}$, so erhält man die sogenannte Stromdichte $S$. Für Transformatoren gilt nach den relevanten Normen, dass eine maximale Stromdichte von etwa $\qty{2,5}{\ampere\per\milli\meter\squared}$ nicht überschritten werden sollte.

Die Berechnungsformel lautet (siehe Formelsammlung -  Stichwort: Belastbarkeit von Wicklungen):

$I = S \cdot A_\mathrm{Dr}$

<unit>
Stromdichte $S = \frac{I}{A} $ in  $\unit{\ampere\per\milli\meter\squared}$
</unit>

<indepth>
Nach VDE ist für frei verlegte Leiter aus Kupfer die maximal zulässige Stromstärke mit $\qty{12}{\ampere}$ bei einer Querschnittsfläche von $\qty{0,75}{\milli\meter\squared}$ festgelegt. Bei Schmelzsicherungen kann die Stromdichte bis zu $\qty{3000}{\ampere\per\milli\meter\squared}$ erreichen.
</indepth>

Versuche nun die folgende Frage zu beantworten. Dafür brauchst du die Formel für die Querschnittsfläche eines Leiters und die Formel für die Belastbarkeit von Wicklungen. Achte darauf, dass die Einheiten korrekt umgerechnet werden.

[question:AC307]

---

Eines der wichtigsten Anwendungsgebiete von Transformatoren in der Hochfrequenztechnik ist die **Impedanzanpassung**. Hierbei werden Transformatoren als sogenannte Anpassungsübertrager eingesetzt.

Im Gegensatz zu Netztransformatoren besteht der Kern solcher Übertrager meist nicht aus massivem Eisen, sondern aus gepresstem Eisenpulver oder Ferrit. Diese Materialien sind für hohe Frequenzen besser geeignet und reduzieren Verluste.

<indepth>
Unter *Anpassung* versteht man, dass die Impedanz einer Quelle (z. B. eines Senders) möglichst genau an die Impedanz der Last (z. B. einer Antenne) angepasst wird. Nur bei guter Anpassung kann die Leistung optimal übertragen werden, ohne dass ein Teil der Energie reflektiert wird.
</indepth>

Ein Anpassungsübertrager hat daher die Aufgabe, eine gegebene Impedanz in eine andere umzuwandeln, sodass Quelle und Last möglichst gut zueinander passen.

---

In der Formelsammlung finden wir die Formel für das Übersetzungsverhältnis $ü$:

$ü = \sqrt{\frac{Z_p}{Z_s}} = \frac{N_p}{N_s} = \frac{U_p}{U_s}$

Quadriert man die Seiten der Gleichung ergibt sich: 


$ü^2 = \frac {Z_p}{Z_s} = \left(\frac{N_p}{N_s}\right)^2 = \left(\frac{U_p}{U_s}\right)^2$

Daran erkennt man, dass das Impedanzverhältnis ist das Quadrat des Spannungsverhältnisses und damit auch das Quadrat des Windungszahlenverhältnisses. Oder anders herum gesagt, ein bestimmtes Windungsverhältnis führt zu einem quadratisch höheren Impedanzverhältnis.

<indepth>
Herleitung der Formel zur Impedanzübertragung:
$ P_p = P_s$
$U_p \cdot I_p = U_s \cdot I_s$
Für $U$ das Ohmsche Gesetz einsetzen: $U = I \cdot R$;
$R$ wird durch $Z$ ersetzt
$(I_p \cdot Z_p) \cdot I_p = (I_s \cdot Z_s) \cdot I_s$
Das Impedanzverhältnis auf einer Seite bilden:
$ \frac{Z_p}{Z_s} = \frac{{I_s}^2}{{I_p}^2} = ü^2$
Alternativ für $I$ das Ohmsche Gesetz einsetzen:
$I = \frac{U}{R}$
$R$ wird durch $Z$ ersetzt
$\frac{U_p}{Z_p} \cdot U_p  = \frac{U_s}{Z_s} \cdot U_s$
Das Impedanzverhältnis auf einer Seite bilden:
$ \frac{Z_p}{Z_s} = \frac{{U_p}^2}{{U_s}^2} = ü^2$
</indepth>

---

Als Beispiel betrachten wir eine endgespeiste Antenne, die wir in einem späteren Kapitel noch genauer untersuchen werden. Deren Eingangsimpedanz beträgt etwa $\qty{2450}{\ohm}$ und ist damit deutlich hochohmig. Sie soll an einen Sender mit einer Lastimpedanz von $\qty{50}{\ohm}$ angepasst werden.

<margin>
[picture:260:a_endgespeiste_antenne:Endgespeiste Antenne mit Impedanzanpassung durch einen Übertrager]
</margin>

Für die Impedanzübertragung von $\qty{50}{\ohm}$ auf $\qty{2450}{\ohm}$ ist das Verhältnis $Z_p:Z_s = \qty{50}{\ohm}:\qty{2450}{\ohm} = 1:49$. Das bedeutet $ü^2 = 1:49$ und damit $ü=\sqrt{1}:\sqrt{49}=1:7$. Das bedeutet, dass die Primärseite nur ein Siebtel der Windungen der Sekundärseite haben darf, damit die Impedanzanpassung gelingt, z.B. $N_p=1$ und $N_s=7$. In der Praxis wird üblicherweise ein Windungsverhältnis von $2:14$ verwendet (vgl. Abbildung [ref:a_unun]).

<margin>
[photo:332:a_unun:Beispiel für einen Unun-Übertrager mit einem Windungsverhältnis von 2 zu 14, wobei die Primärseite und Sekundärseite zusammen bifilar (verdrillt) gewickelt sind]
</margin>

Die folgende Aufgabe entspricht im Wesentlichen dem zuvor betrachteten Beispiel. Für einen endgespeisten Dipol wird hier eine Eingangsimpedanz von etwa $\qty{2,5}{\kilo\ohm}$ angegeben. In der Praxis schwankt dieser Wert jedoch, abhängig von Umgebung und Aufbau, typischerweise im Bereich von etwa $\qty{2}{\kilo\ohm}$ bis $\qty{3}{\kilo\ohm}$. 
Mit einem Windungsverhältnis von etwa $1:7$ lässt sich dennoch in der Regel eine ausreichend gute Anpassung an $\qty{50}{\ohm}$ erreichen.

[question:AC306]

Versuche nun, die folgenden Fragen selbständig mit deinem Wissen zu lösen.

[question:AC305]
[question:AC303]
[question:AC304]
