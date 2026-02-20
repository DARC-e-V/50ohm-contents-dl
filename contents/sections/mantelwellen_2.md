Idealerweise sind die Ströme durch den Innen- und Außenleiter eines Koaxialkabels genau gleich groß und in der Richtung entgegengesetzt. Deren Summe ist also Null und man spricht dann von einem reinen *Gegentaktsignal*. Genau dann treten keine Mantelwellen auf.

Ist die Summe des Signals hingegen ungleich Null, dann ist ein sogenanntes *Gleichtaktsignal* vorhanden. Der Gleichtaktanteil eines Stroms im Koaxialkabel fließt stets auf der Außenseite des Außenleiters und ist damit ein Mantelstrom mit zugehöriger Mantelwelle um das Koaxialkabel herum.

[question:AG425]

Dass ein um einen Ferritkern gewickeltes Koaxialkabel zur Unterdrückung von Mantelwellen geeignet sind, haben wir bereits gelernt. Dies ist eine Form der sogenannten *stromkompensierten Drossel*.

Eine Drossel ist eine Spule, die hochfrequente Ströme blockieren soll. Die stromkompensierte Drossel ist eine Bauform der Drosselspule, bei der zwei getrennte Wicklungen auf den selben Magnetkern gewickelt werden. Hierbei wird die stromkompensierte Drossel so beschaltet, dass Gegentaktsignale, d. h. Signale bei denen der Strom in der einen Wicklung genau entgegengesetzt der anderen Wicklung sind und ansonsten die gleiche Größe aufweisen, kein Magnetfeld in den Kern induzieren. Die stromkompensierte Drossel lässt also Gegentaktsignale ungehindert hindurch. Gleichtaktanteile jedoch, also z. B. Ströme die nur auf dem Außenleiter und damit nur in einer Wicklung fließen, werden durch die Induktivität blockiert.

[question:AG426]

---

Eine Alternative zur stromkompensierten Drossel stellt ein HF-Trenntrafo dar. Da die Primär- und die Sekundärwicklung nicht miteinander verbunden sind, muss ein Strom der an einem Pol in den Trenntrafo hineinfließt (zumindest näherungsweise) auch in gleicher Größe aus dem anderen Pol wieder hinausfließen. Ein Gleichtaktanteil ist damit ausgeschlossen.

<indepth>
Da zwischen den Windungen der Spule eines Trenntrafos eine Kapazität entsteht und die Spule auch eine Kapazität gegenüber der anderen Spule ausbildet, unterdrückt auch ein Trenntrafo den Gleichtaktanteil eines Signals nicht vollständig.
</indepth>

[question:AJ115]

Wenn ein Koaxialkabel frei von HF-Gleichtaktsignalen ist, dann weist der Außenleiter keine hochfrequente Spannung gegenüber der Erde auf. Dies liegt daran, dass sich bei einem Gegentaktsignal, also entgegengesetzten Strömen im Innen- und Außenleiter, ein elektrisches Feld ausschließlich zwischen Innen- und Außenleiter ausbildet. Von außen betrachtet heben sich die Wirkungen der beiden Ströme auf, da sie in der Summe Null ergeben. Das Vorhandensein von Mantelwellen hängt also unmittelbar mit dem Vorhandensein von HF-Spannungen auf dem Außenleiter zusammen.

Genau solche Spannungen am Außenleiter entstehen z. B., wenn wir eine symmetrische Antenne an das Kabel anschließen, denn am Speisepunkt weist jeder Dipolschenkel eine Spannung gegenüber Erde auf. Verbinden wir die Schenkel jeweils mit einem Leiter des Koaxialkabels, so wird auch der Außenleiter eine Spannung gegenüber Erde aufweisen.

Gut geerdete Antennen hingegen, z. B. eine Groundplane Antenne mit vielen gut abgestimmten oder vergrabenen Radialen, weisen am Speisepunkt der Radiale eine Spannung von nahezu Null gegenüber der Erde auf. Schlecht geerdete Groundplane-Antennen hingegen können anfällig für Mantelwellen sein.

Eine weitere Möglichkeit, wie Mantelwellen entstehen können, ist durch kontaktlose Einkopplung in den Koax-Schirm. Führt man beispielsweise ein Speisekabel parallel zu einem Dipolschenkel, so entsteht eine Kopplung über das elektromagnetische Nahfeld der Antenne.

[question:AG427]

Bei vollständig symmetrischen Antennen kann ein sogenannter Spannungsbalun eingesetzt werden, um die Ströme im Koaxkabel zu symmetrieren. Eine beliebte Bauform ist ein Spartransformator, bei dem das Koaxialkabel in der Mitte und am Ende einer Spule angeschlossen wird, und die Antenne mit den beiden Enden der Spule verbunden wird.

% TODO: Bild Spannungsbalun / Spartransformator

Bei dieser Bauform kommt es neben der gewünschten Symmetrierung zusätzlich zu einer Verdoppelung der Spannung ($ü = 2$) sowie einer entsprechenden Halbierung des Stroms, was einer 1:4 Impedanztransformation entspricht, d. h. an ein $\qty{50}{\ohm}$ Koaxialkabel ist eine Antenne mit einem Speisewiderstand von möglichst $\qty{200}{\ohm}$ anzuschließen.

[question:AG421]
[question:AG422]

Diese Bauform ist jedoch nur geeignet Mantelwellen zu unterdrücken, wenn sich die angeschlossene Antenne tatsächlich symmetrisch verhält und sie nicht aufgrund von Umgebungseinflüssen asymmetrisch belastet wird.

Allen Bauteilen, die der Unterdrückung von Mantelwellen dienen, ist gemein, dass dennoch eine "kontaktlose" Einkopplung über die elektromagnetischen Nahfelder der Antennen direkt auf den Koaxschirm, also hinter der Mantelwellensperre, erfolgen kann. Hier kann z. B. eine weitere, zusätzliche Mantelwellensperre mit etwas Entfernung zur Antenne helfen.

[question:AG428]
[question:AG429]