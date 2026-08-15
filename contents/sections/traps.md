Multibandantennen, die gezielt auf mehreren Bändern resonant sind, haben wir bereits kennengelernt, z. B. die endgespeiste Antenne mit 1:49-Transformator. Kommen wir wieder auf unser Beispiel aus dem Abschnitt "Strom- und Spannungsspeisung II" zurück: Ein mittengespeister Halbwellendipol kann neben seiner Grundfrequenz grundsätzlich auch auf ungeradzahligen Vielfachen dieser Frequenz resonant sein. So besitzt beispielsweise ein für das $\qty{80}{\meter}$-Band ausgelegter Dipol mit einer Grundfrequenz von $\qty{3,5}{\mega\hertz}$ weitere Resonanzen näherungsweise bei $\qty{10,5}{\mega\hertz}$ und $\qty{17,5}{\mega\hertz}$.

Bei geradzahligen Vielfachen der Grundfrequenz, beispielsweise bei $\qty{7}{\mega\hertz}$ oder $\qty{14}{\mega\hertz}$, liegt am mittigen Speisepunkt dagegen ein Stromminimum und damit eine hohe Impedanz. Diese Frequenzen sind bei einem einfachen mittengespeisten Dipol daher nicht ohne Weiteres nutzbar. Eine Möglichkeit, zusätzliche Resonanzen gezielt auf solchen Frequenzen zu erzeugen, ist der sogenannte *Sperrkreis-Dipol*, der auch als *Trap-Dipol* bezeichnet wird.

Bei einem Sperrkreis-Dipol befindet sich in jeder Dipolhälfte mindestens ein Parallelschwingkreis aus einer Spule und einem Kondensator. Einen solchen Schwingkreis bezeichnet man als *Trap* (englisch für „Falle“). Ein Parallelschwingkreis ist bei seiner Resonanzfrequenz hochohmig (vgl. Abbildung [ref:a_sperrkreis]). Er wirkt dann als *Sperrkreis* und verhindert weitgehend, dass Strom in den weiter außen liegenden Teil des Dipols fließt. Dadurch kann derselbe Dipol auf mehreren Frequenzbändern unterschiedliche elektrische Längen besitzen.

<margin>
[picture:1036:a_sperrkreis:Qualitativer Frequenzgang eines Parallelschwingkreises (Sperrkreis)]
</margin>

[question:AG109]
[question:AG110]

---

Wie sich ein Trap auf den Dipol auswirkt, hängt davon ab, wie die Betriebsfrequenz im Verhältnis zu seiner Resonanzfrequenz $f_\mathrm{res}$ liegt.

* Bei $f=f_\mathrm{res}$ ist der Parallelschwingkreis hochohmig und wirkt als Sperrkreis. Der äußere Teil des Dipols wird dadurch weitgehend vom inneren Teil getrennt.
* Bei $f<f_\mathrm{res}$ überwiegt die induktive Wirkung des Traps. Er wirkt ähnlich wie eine Verlängerungsspule und verlängert den Strahler elektrisch.
* Bei $f>f_\mathrm{res}$ überwiegt die kapazitive Wirkung des Traps. Dadurch wird der Strahler elektrisch etwas verkürzt.

<margin>
In diesem Applet kann man die Wirkung eines Traps auf einen Dipol für verschiedene Frequenzen untersuchen:

[include:applet_traps]
</margin>

Besonders anschaulich ist zunächst der Resonanzfall. Wird der Dipol bei der Resonanzfrequenz des Traps betrieben (z. B. $\qty{7.05}{\mega\hertz}$ in unserer Abbildung), ist der Parallelschwingkreis hochohmig. Es fließt daher nur wenig Strom in den äußeren Teil des Dipols. Der Dipol verhält sich näherungsweise so, als würde er an der Position des Traps enden.

[question:AG112]

Dieser Zusammenhang kann für den Entwurf eines Zweiband-Dipols genutzt werden. Für das höherfrequente Band bestimmt der Abstand zwischen den beiden Traps im Wesentlichen die wirksame Dipollänge. Die äußeren Drahtstücke werden bei dieser Frequenz durch die Sperrwirkung der Traps weitgehend abgetrennt, als wären sie nicht da und der Dipol verhält sich wie ein kürzerer Dipol.

[question:AG116]

---

Wird der Dipol dagegen mit einer Frequenz *unterhalb* der Resonanzfrequenz des Traps betrieben (z. B. $\qty{3.5}{\mega\hertz}$ in unserer Abbildung), ist der Schwingkreis nicht mehr hochohmig. Seine induktive Wirkung überwiegt. Der Trap wirkt dadurch ähnlich wie eine Verlängerungsspule und verlängert den Dipol elektrisch. Dadurch kann der gesamte Dipol einschließlich der äußeren Drahtstücke für ein niedrigeres Frequenzband genutzt werden.

[question:AG111]

---

Bei einer Frequenz *oberhalb* der Resonanzfrequenz überwiegt dagegen die kapazitive Wirkung des Traps. Der Trap wirkt dadurch elektrisch verkürzend und er kann sogar auf z. B. $\qty{14}{\mega\hertz}$ resonant sein. Auch dieser Effekt sollte bei der Dimensionierung eines Sperrkreis-Dipols berücksichtigt werden.

[question:AG113]

---

Durch mehrere Trap-Paare können Dipole für noch mehr Frequenzbänder aufgebaut werden. Dabei liegen die Traps für die höchsten Frequenzen am weitesten innen, weil hierfür die kürzeste wirksame Dipollänge benötigt wird.

Der innerste Trap wird daher auf die höchste vorgesehene Frequenz abgestimmt. Das nächste weiter außen liegende Trap-Paar wird auf die nächstniedrigere Frequenz abgestimmt und so weiter. Je niedriger die Betriebsfrequenz ist, desto größere Teile des Dipols werden wirksam.

[question:AG115]
[question:AG114]

Traps werden nicht nur in Dipolantennen eingesetzt. Auch bei Richtantennen wie Yagi-Antennen können Sperrkreise in den einzelnen Elementen verwendet werden, um die Antenne auf mehreren Frequenzbändern nutzbar zu machen.