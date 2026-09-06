Wie wir bereits gelernt haben, kann ein Halbwellendipol auch an einem Ende gespeist werden. Der Speisewiderstand ist bei einer Drahtlänge von $\lambda / 2$ oder Vielfachen davon hochohmig (ca. $\qtyrange{2000}{2500}{\ohm}$).

Für die Anpassung einer solchen endgespeisten Antenne gibt es verschiedene Möglichkeiten. Im Folgenden betrachten wir drei typische Varianten:

* Fuchskreis
* Transformator zur Impedanzanpassung
* Zeppelinantenne

Eine Möglichkeit der Anpassung ist der bereits besprochene Fuchskreis (vgl. Abbildung [ref:a_fuchskreis]). Dabei handelt es sich um einen Parallelschwingkreis, der auf die Betriebsfrequenz abgestimmt wird. Er transformiert die niedrige Impedanz der Speiseleitung auf die hohe Speiseimpedanz der endgespeisten Halbwellenantenne und gleicht zugleich vorhandene Blindanteile aus.

<margin>
[picture:310:a_fuchskreis:Fuchskreis zur Anpassung einer endgespeisten Halbwellenantenne]
</margin>

[question:AG419]

---

Eine andere Möglichkeit ist ein Transformator (vgl. Abbildung [ref:a_unun_1_49]) mit einem Übersetzungsverhältnis von $ü = 1:7$. Da sowohl Spannung als auch Strom um den Faktor $\num{7}$ multipliziert bzw. dividiert werden, ergibt sich für den Widerstand eine Transformation von $1:7^2 = 1:49$ entsprechend $(1 \cdot \qty{50}{\ohm}) : (49 \cdot \qty{50}{\ohm}) = \qty{50}{\ohm} : \qty{2450}{\ohm}$.

<margin>
[photo:332:a_unun_1_49:1 zu 49 Un-Un zur Anpassung einer endgespeisten Halbwellenantenne]
[picture:315:a_endspeisung_1:Endgespeister Halbwellendipol mit Pigtail]
[picture:260:a_endspeisung_2:Endgespeister Halbwellendipol mit Koaxialkabel als Gegengewicht]
</margin>

<attention>
Hinsichtlich der *Impedanztransformation* (Transformation des Widerstands) geht das Windungsverhältnis eines Transformators im Quadrat ein, d.h. ein Transformator mit einem Windungsverhältnis von 1:7 sorgt für eine 1:49-Impedanztransformation. Bei Baluns und Un-Uns ist oft nicht angegeben, ob es sich um das Windungs- oder das Impedanzverhältnis handelt. Es besteht also die Möglichkeit der Verwechselung. Üblich ist die Angabe des Impedanzverhältnisses. Bei einem Transformator mit einem Windungsverhältnis ($ü$) von 1:7 spricht man dann z. B. von einem 1:49-Un-Un.
</attention>

Als Gegengewicht wird oft ein kurzes Drahtende (mindestens ein zwanzigstel der Wellenlänge), vgl. Abbildung [ref:a_endspeisung_1] oder ein Teil der koaxialen Zuleitung (mindests $\qty{0.05}{\lambda}$) verwendet, vgl. Abbildung [ref:a_endspeisung_2]. Eine Mantelwellensperre (Abkürzung MWS) verhindert, dass das weitere Zuleitungskabel zum Teil der Antenne wird.

[question:AG123]
[question:AG124]

---

Anstelle eines Fuchskreises oder Transformators kann auch eine Zweidrahtleitung der Länge $\lambda / 4$ verwendet werden. Dann spricht man von einer *Zeppelinantenne* (vgl. Abbildung[ref:a_zeppelinantenn]). Wie eine Leitung eine Impedanz transformiert werden wir in einem späteren Abschnitt noch genauer betrachten.

Die Bezeichnung geht auf den Einsatz dieser Antennen an Luftschiffen zurück. Durch die $\lambda / 4$ lange Zweidrahtleitung tritt die hohe Spannung erst an ihrem Ende und damit weit entfernt vom gasgefüllten Luftschiff auf (vgl. Abbildung [ref:a_zeppelinantenne_foto]).

<margin>
[picture:314:a_zeppelinantenne:Aufbau einer Zeppelinantenne]
[photo:336:a_zeppelinantenne_foto:Zeppelinantenne (Symbolbild)]
</margin>

[question:AG120]

---

Ebenso wie bei einem endgespeisten Halbwellendipol kann auch bei anderen Antennenformen eine Speiseleitung mit abweichendem Wellenwiderstand zur Anpassung verwendet werden. Für die Klasse E haben wir bereits die Ganzwellen-Schleifen-Antennen kennengelernt; darunter auch die Delta-Loop und die Quad-Antenne. Eine Delta-Loop-Antenne (vgl. Abbildung [ref:a_delta_loop]) hat bei gleichlangen Schenkeln eine Speiseimpedanz von etwa $\qty{100}{\ohm}$. Durch Einfügen einer $\lambda / 4$-Leitung mit einem Wellenwiderstand von $\qty{75}{\ohm}$ erfolgt eine Transformation auf die im Amateurfunk üblichen $\qty{50}{\ohm}$.

<margin>
[picture:311:a_delta_loop:Delta-Loop-Antenne]
</margin>

[question:AG117]

<indepth>
Der optimale Wert für den Wellenwiderstand einer $\lambda / 4$-Speiseleitung, die zur Anpassung verwendet wird, errechnet sich aus dem *geometrischen Mittel* der beiden Impedanzen, z. B. $\qty{50}{\ohm}$ und $\qty{100}{\ohm}$ entsprechend $\sqrt{\qty{50}{\ohm} \cdot \qty{100}{\ohm}} \approx \qty{70,7}{\ohm}$.
</indepth>

Führt man die Ganzwellenschleife als Quadrat aus, dann muss die Länge jeder Seite entsprechend ein Viertel der Wellenlänge betragen.

[question:AG119]

<attention>
Wie beim Dipol weicht die mechanische Länge einer Ganzwellen-Schleifenantenne von der elektrischen Länge ab. Im Gegensatz zum Verkürzungsfaktor bei Dipolen gibt es bei Ganzwellenschleifen hingegen überraschenderweise einen *Verlängerungsfaktor*, d.h. die Antenne muss wenige Prozent länger sein, als eine Wellenlänge im Freiraum wäre.
</attention>

---

Da Frequenzbänder unterschiedliche Ausbreitungsbedingungen zu unterschiedlichen Tages-, Jahres- und Sonnenzykluszeiten aufweisen, möchten Funkamateure gerne auf möglichst vielen Frequenzbändern Betrieb machen können. Zwei Beispiele für Multibandantennen sind die *G5RV-Antenne mit zwei gleichlangen Schenkeln* (vgl. Abbildung [ref:a_g5rv]) und einer Zweidrahtleitung sowie die *asymmetrisch angeregte Windomantenne* (vgl. Abbildung [ref:a_windom]), bei denen sich durch geschickte Abmessungen viele Resonanzen und damit eine Nutzung auf möglichst vielen Amateurfunkbändern ergeben.

<margin>
[picture:313:a_g5rv:G5RV-Antenne]
[picture:309:a_windom:Windomantenne]
</margin>

[question:AG121]
[question:AG122]

---

% TODO: Darstellung von $5/8 \lambda$ prüfen

Dass eine Antenne resonant ist, bedeutet noch nicht, dass sie auch eine gute Abstrahlcharakteristik aufweist. Oftmals ist es gewünscht, eine möglichst flache Abstrahlung zu erreichen. Bei gegenüber Erde erregten Vertikalantennen ergibt sich eine Länge von ca. $5/8 \lambda$ als Optimum.

<indepth>
Ein einfacher Draht mit Erde als Gegenpol ist bei einer Länge von $5/8 \lambda$ nicht resonant. Resonanzen ergeben sich nur bei $1/4$, $3/4$, $5/4$ usw. Daher ist eine Anpassung notig. Dies wird in der Regel durch Einfügen einer Spule erreicht, welche die elektrische Länge von $5/8$ auf $6/8$ (also $3/4$) verlängert. Solche Spulen sieht man oft bei Antennen für den KFZ-Bereich.
% TODO: Bild VHF oder CB-KFZ-Antenne
</indepth>

<attention>
Das Optimum von $5/8 \lambda$ gilt nur für gegenüber Erde erregte Antennen. Betrachtet man beispielsweise mittengespeiste Dipole, die sich entweder im Freiraum oder vertikal, knapp über dem Erdboden befinden, dann liegt das Optimum bei $5/4 \lambda$.
% TODO: Frage ist falsch, siehe 2. Review von DL9JBE.
</attention>

[question:AG223]