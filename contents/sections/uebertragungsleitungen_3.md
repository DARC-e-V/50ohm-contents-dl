In der Klasse E haben wir bereits die Paralleldraht-Speiseleitung, auch Hühnerleiter genannt, kennengelernt (vgl. Abbildung [ref:a_huenerleiter]). Diese besteht aus zwei parallel verlaufenden Leitern. Zweidrahtleitungen verhalten sich, sofern sie symmetrisch gespeist und belastet werden, auch hinsichtlich ihrer Strom- und Spannungsverteilung symmetrisch. Das bedeutet, dass Strom und Spannung an einer bestimmten Stelle auf beiden Leitern jeweils den gleichen Betrag, aber entgegengesetzte Vorzeichen besitzen, wie in Abbildung [ref:a_zweidrahtleitung] dargestellt.

<margin>
[photo:324:a_huenerleiter:Hühnerleiter, auch als Zweidrahtleitung bezeichnet]
</margin>

Die Ströme auf den beiden Leitern fließen damit zu jedem Zeitpunkt in entgegengesetzte Richtungen. Man spricht von *Gegentaktströmen*. Die von den beiden Leitern erzeugten elektromagnetischen Felder wirken dadurch in größerer Entfernung weitgehend gegeneinander und heben sich zum großen Teil auf. Eine symmetrisch betriebene Zweidrahtleitung strahlt daher nur wenig ab.

<margin>
[picture:1107:a_zweidrahtleitung:Strom- und Spannungsverteilung an einer Zweidrahtleitung]
</margin>

Ist die Speiseleitung dagegen nicht vollständig symmetrisch, können zusätzlich *Gleichtaktströme* auftreten. Dabei fließt ein Teil des Stroms auf beiden Leitern in die gleiche Richtung. Die von diesen Strömen erzeugten Felder heben sich nicht gegenseitig auf. Die Speiseleitung kann dann selbst wie eine Antenne wirken und Hochfrequenzenergie abstrahlen. Solche Gleichtaktanteile können beispielsweise entstehen, wenn ein Dipol nicht exakt symmetrisch aufgebaut ist, eine unsymmetrische Antenne oder Last angeschlossen wird oder der Übergang zwischen einer symmetrischen Antenne und einer unsymmetrischen Speiseleitung nicht durch einen geeigneten Balun beziehungsweise eine Mantelwellensperre entkoppelt wird.

[question:AG312]

Besonders im Nahfeld anderer Leitungen oder elektrischer Geräte kann zudem eine stärkere elektromagnetische Kopplung auftreten. Deshalb werden Speiseleitungen innerhalb von Gebäuden üblicherweise geschirmt ausgeführt, beispielsweise als Koaxialkabel. Bei einem Koaxialkabel befinden sich die elektromagnetischen Felder des Gegentakts weitgehend zwischen Innenleiter und Schirm. Dadurch werden sowohl die Abstrahlung der Speiseleitung als auch die Einkopplung äußerer Störungen reduziert.

[question:AG301]

Als geschirmtes Kabel bietet sich das Koaxialkabel an, welches wir auch in der Klasse E bereits kennengelernt haben. Koaxialkabel gibt es in verschiedensten Ausführungen. In der folgenden Frage werden die *Hochfrequenzeigenschaften* von Koaxialkabeln, also deren elektrischen Eigenschaften hinsichtlich hoher Frequenzen betrachtet. Dies sind im Wesentlichen:

* der Wellenwiderstand,
* die Kabeldämpfung und der
* Verkürzungsfaktor,

den wir gleich näher betrachten. Der Biegeradius hingegen ist eine mechanische Eigenschaft, die angibt, wie eng das Kabel in einer Kurve verlegt werden darf. Die Rückflussdämpfung gibt an, wieviele Reflexionen vorhanden sind, was von der an einer Leitung angeschlossenen Last abhängt und somit keine Kabeleigenschaft ist.

[question:AG303]

Der Verkürzungsfaktor ergibt sich durch das zwischen Innen- und Außenleiter befindliche Dielektrikum. In diesem befindet sich der Großteil der elektromagnetischen Welle, die durch das Kabel geleitet wird. Die Wahl des Dielektrikums bestimmt, wie schnell sich eine Welle durch das Kabel fortpflanzen kann. Die Ausbreitungsgeschwindigkeit im Koaxialkabel liegt unter der Lichtgeschwindigkeit im Freiraum. Übliche Materialien für das Dielektrikum sind Polyethylen (PE) und Teflon (PTFE). Durch Aufschäumung entsteht gewissermaßen eine Mischung mit Luft, bei der die Kabeldämpfung geringer ausfällt.

[question:AG314]
[question:AG302]

Die durch das Dielektrikum reduzierte Ausbreitungsgeschwindigkeit schlägt sich im Verkürzungsfaktor nieder, der angibt, auf welche Länge ein Kabel mechanisch gekürzt werden muss, damit es elektrisch eine bestimmte Länge aufweist (also z. B. eine viertel Wellenlänge lang ist). Für den Verkürzungsfaktor finden wir in der Formelsammlung folgenden Zusammenhang:

$k_\mathrm{v} = \frac{L_\mathrm{G}}{L_\mathrm{E}} = \frac{1}{\sqrt{\epsilon_\mathrm{r}}}$

Hierbei ist $k_\mathrm{v}$ der Verkürzungsfaktor, $L_\mathrm{G}$ die geometrische ("mechanische") Länge, und $L_\mathrm{E}$ die elektrische Länge. Die relative Dielektrizitätszahl $\epsilon_\mathrm{r}$ ist abhängig vom eingesetzten Dielektrikum. Für nicht-geschäumtes Polyethylen (PE) können wir der Formelsammlung eine Dielektrizitätszahl von $\num{2,29}$ entnehmen.

[question:AG317]