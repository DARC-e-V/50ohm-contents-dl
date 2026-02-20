Wie wir bereits gelernt haben, kann ein Halbwellendipol auch an einem Ende gespeist werden. Der Speisewiderstand ist bei einer Drahtlänge von $\lambda / 2$ oder Vielfachen davon hochohmig (ca. $\qty{2000}{\ohm}$ bis $\qty{2500}{\ohm}$). Eine Möglichkeit der Anpassung ist der bereits besprochene Fuchskreis.

[question:AG419]

---

Eine andere Möglichkeit ist ein Transformator mit einem Übersetzungsverhältnis von $ü = 1:7$. Da sowohl Spannung als auch Strom um den Faktor $\num{7}$ multipliziert bzw. dividiert werden, ergibt sich für den Widerstand eine Transformation von $1:7^2 = 1:49$ entsprechend $(1 \cdot \qty{50}{\ohm}) : (49 \cdot \qty{50}{\ohm}) = \qty{50}{\ohm} : \qty{2450}{\ohm}$.

<attention>
Hinsichtlich der *Impedanztransformation* (Transformation des Widerstands) geht das Windungsverhältnis eines Transformators im Quadrat ein, d.h. ein Transformator mit einem Windungsverhältnis von 1:7 sorgt für eine 1:49-Impedanztransformation. Bei Baluns und Un-Uns ist oft ist nicht angegeben, ob es sich um das Windungs- oder das Impedanzverhältnis handelt. Es besteht also die Möglichkeit der Verwechselung. Üblich ist die Angabe des Impedanzverhältnisses. Bei einem Transformator mit einem Windungsverhältnis ($ü$) von 1:7 spricht man dann z. B. von einem 1:49-Un-Un.
</attention>

Als Gegengewicht wird oft ein kurzes Drahtende (mindestens ein zwanzigstel der Wellenlänge) oder ein Teil der koaxialen Zuleitung verwendet. Eine Mantelwellensperre (Abkürzung MWS) verhindert, dass das weitere Zuleitungskabel zum Teil der Antenne wird.

[question:AG123]
[question:AG124]

Anstelle eines Fuchskreises oder Transformators kann auch eine Zweidrahtleitung der Länge $\lambda / 4$ verwendet werden. Dann spricht man von einer *Zeppelinantenne*.

%TODO namensherkunft zeppelin

[question:AG120]

---

Ebenso wie bei einem endgespeisten Halbwellendipol kann auch bei anderen Antennenformen eine Speiseleitung mit abweichendem Wellenwiderstand zur Anpassung verwendet werden. Für die Klasse E haben wir bereits die Ganzwellen-Schleifen-Antennen kennengelernt; darunter auch die Delta-Loop und die Quad-Antenne. Eine Delta-Loop-Antenne hat bei gleichlangen Schenkeln eine Speiseimpedanz von etwa $\qty{100}{\ohm}$. Durch Einfügen einer $\lambda / 4$-Leitung mit einem Wellenwiderstand von $\qty{75}{\ohm}$ erfolgt eine Transformation auf die im Amateurfunk üblichen $\qty{50}{\ohm}$.

[question:AG117]

<indepth>
Der optimale Wert für den Wellenwiderstand einer $\lambda / 4$-Speiseleitung, die zur Anpassung verwendet wird, errechnet sich aus dem *geometrischen Mittel* der beiden Impedanzen (z. B. $\qty{50}{\ohm}$ und $\qty{100}{\ohm}$ entsprechend $\sqrt{\qty{50}{\ohm} \cdot \qty{100}{\ohm}} \approx \qty{70,7}{\ohm}$.
</indepth>

Führt man die Ganzwellenschleife als Quadrat aus, dann muss die Länge jeder Seite entsprechend ein Viertel der Wellenlänge betragen.

[question:AG119]

<attention>
Wie beim Dipol weicht die mechanische Länge einer Ganzwellen-Schleifenantenne von der elektrischen Länge ab. Im Gegensatz zum Verkürzungsfaktor bei Dipolen gibt es bei Ganzwellenschleifen hingegen überraschenderweise einen *Verlängerungsfaktor*, d.h. die Antenne muss wenige Prozent länger sein, als eine Wellenlänge im Freiraum wäre.
</attention>

---

Da Frequenzbänder unterschiedliche Ausbreitungsbedingungen zu unterschiedlichen Tages-, Jahres- und Sonnenzykluszeiten aufweisen, möchten Funkamateure gerne auf möglichst vielen Frequenzbändern Betrieb machen können. Zwei Beispiele für Multibandantennen sind die *G5RV-Antenne mit zwei gleichlangen Schenklen* und einer Zweidrahtleitung sowie die *asymmetrisch angeregte Windomantenne* bei denen sich durch geschickte Abmessungen viele Resonanzen und damit eine Nutzung auf möglichst vielen Amateurfunkbändern ergeben.

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