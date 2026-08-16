Eine sogenannte *Lecherleitung* besteht aus zwei parallelen Leitern, auf denen sich durch die Überlagerung von hin- und rücklaufender Welle stehende HF-Wellen ausbilden. Sie kann am Ende entweder offen (vgl. Abbildung [ref:a_lecherleitung_offen]) oder kurzgeschlossen (vgl. Abbildung [ref:a_lecherleitung_kurzgeschlossen]) sein. In beiden Fällen entstehen charakteristische Strom- und Spannungsverteilungen, die beispielsweise zur Bestimmung der Wellenlänge genutzt werden können.

<margin>
[picture:1112:a_lecherleitung_offen:Lecherleitung mit offenem Ende]
</margin>

Bei einer am Ende *offenen* Lecherleitung kann am Leitungsende kein Strom fließen. Dort befindet sich daher ein Stromminimum und gleichzeitig ein Spannungsmaximum. Aus dem Ohmschen Gesetz

$R=\frac{U}{I}$

folgt, dass das Verhältnis von Spannung zu Strom an dieser Stelle idealisiert unendlich groß wird, also $R=\infty$. Strom und Spannung sind entlang der Leitung räumlich um $\frac{\lambda}{4}$ gegeneinander verschoben. Im Abstand von $\frac{\lambda}{4}$ vom offenen Leitungsende befindet sich daher ein Strommaximum und gleichzeitig ein Spannungsminimum. Da dort die Spannung idealisiert gegen null geht, ergibt sich nach dem Ohmschen Gesetz entsprechend $R=0$. Nach jeweils weiteren $\frac{\lambda}{4}$ wechseln sich Strommaximum und Spannungsmaximum ab. Nach einer Strecke von $\frac{\lambda}{2}$ liegt wieder die gleiche Strom- und Spannungsverteilung vor, wie in Abbildung [ref:a_lecherleitung_offen] dargestellt.

---

Bei einer am Ende *kurzgeschlossenen* Lecherleitung können die beiden Leiter am Leitungsende keine unterschiedliche Spannung besitzen. Dort gilt daher $U=0$. Es befindet sich dort ein Spannungsminimum und gleichzeitig ein Strommaximum. Mit $R=\frac{U}{I}$ folgt damit idealisiert $R=0$. Im Abstand von $\frac{\lambda}{4}$ vom Kurzschluss befindet sich dagegen ein Spannungsmaximum und gleichzeitig ein Stromminimum. Da der Strom dort idealisiert gegen null geht, wird das Verhältnis $\frac{U}{I}$ sehr groß und es gilt idealisiert $R=\infty$. Auch bei der kurzgeschlossenen Lecherleitung wechseln sich Strom- und Spannungsmaxima nach jeweils $\frac{\lambda}{4}$ ab. Nach einer Strecke von $\frac{\lambda}{2}$ liegt wieder die gleiche Strom- und Spannungsverteilung vor, wie in Abbildung [ref:a_lecherleitung_kurzgeschlossen] dargestellt.


<margin>
[picture:1111:a_lecherleitung_kurzgeschlossen:Lecherleitung mit kurzgeschlossenem Ende]
</margin>

Welche Frequenz sich auf einer Lecherleitung als Resonanz ausbildet, hängt im Wesentlichen von ihrer Länge ab. Ändert sich die Leitungslänge, ändert sich damit auch die Resonanzfrequenz.

[question:AG320]

Bei einer Leitungslänge von $\frac{\lambda}{2}$ wiederholt sich die Strom- und Spannungsverteilung vollständig. Eine Lastimpedanz am Leitungsende erscheint daher am Leitungseingang wieder mit demselben Wert.

Ein besonders wichtiger Spezialfall ergibt sich, wenn die Lecherleitung bei der betrachteten Frequenz eine elektrische Länge von genau $\frac{\lambda}{4}$ besitzt. Wie wir an den Strom- und Spannungsverteilungen gesehen haben, vertauschen sich über eine Strecke von $\frac{\lambda}{4}$ ein Strommaximum und ein Spannungsmaximum miteinander. Dadurch wird auch eine hohe Impedanz in eine niedrige Impedanz und umgekehrt transformiert.

Bei einer am Ende *offenen* $\frac{\lambda}{4}$-Leitung ist die Impedanz am Leitungsende idealisiert unendlich groß. Nach einer Strecke von $\frac{\lambda}{4}$ befindet sich am Leitungseingang dagegen ein Spannungsminimum und ein Strommaximum. Die Eingangsimpedanz ist daher nahezu null ($Z_\mathrm{in} \approx \qty{0}{\ohm}$). Ein offenes Leitungsende wird durch eine $\frac{\lambda}{4}$ lange Leitung also näherungsweise in einen Kurzschluss transformiert.

---

[question:AG411]

Umgekehrt besitzt eine am Ende *kurzgeschlossene* Leitung am Leitungsende die Impedanz $\qty{0}{\ohm}$. Nach einer Strecke von $\frac{\lambda}{4}$ liegt am Leitungseingang ein Spannungsmaximum und ein Stromminimum vor. Die Eingangsimpedanz wird dort daher sehr groß ($Z_\mathrm{in} \rightarrow \infty$). Ein Kurzschluss am Leitungsende wird durch eine $\frac{\lambda}{4}$ lange Leitung somit näherungsweise in einen Leerlauf transformiert.

<indepth>
Das Verhalten einer $\frac{\lambda}{4}$-Leitung lässt sich auch mit Schwingkreisen vergleichen. Eine offene $\frac{\lambda}{4}$-Leitung besitzt am Eingang eine sehr kleine Impedanz und verhält sich dort ähnlich wie ein *Reihenschwingkreis in Resonanz*. Eine kurzgeschlossene $\frac{\lambda}{4}$-Leitung besitzt am Eingang dagegen eine sehr große Impedanz und verhält sich ähnlich wie ein *Parallelschwingkreis in Resonanz*.
</indepth>

Im nächsten Abschnitt betrachten wir, wie sich mit Hilfe von $\frac{\lambda}{4}$-Leitungen gezielt Impedanztransformationen durchführen lassen.