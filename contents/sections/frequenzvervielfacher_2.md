In der Klasse E haben wir bereits Frequenzvervielfacher auf Blockebene kennen gelernt. In der Klasse A wollen wir verstehen, wie sie funktionieren

Dioden und Transistoren besitzen eine nichtlineare Kennlinie. Werden sie mit einem sinusförmigen Signal angesteuert, wird dieses dadurch verzerrt. Wie wir bereits gelernt haben, entstehen bei solchen nichtlinearen Vorgängen Oberwellen. Bei einem Frequenzvervielfacher wird dieser Effekt gezielt genutzt: Das Eingangssignal wird zunächst nichtlinear verzerrt, sodass zahlreiche Oberwellen entstehen. Anschließend wird die gewünschte Oberwelle mit einem abgestimmten Schwingkreis oder Filter ausgewählt und als Ausgangssignal verwendet.

Technisch wird ein Frequenzvervielfacher so realisiert, dass das Eingangssignal zunächst einer nichtlinearen Verzerrerstufe zugeführt wird. Dies kann z.B. ein Klasse-C-Verstärker sein, welche wir im laufe des Kapitels noch besprechen werden. Anschließend wird aus dem Signalgemisch mittels Filtern die gewünschte Oberschwingung des Signals selektiert und an die nächste Stufe weitergeführt. Da die Frequenzvervielfachung auf Oberschwingungen/Harmonischen basiert, sind nur ganzzahlige Vielfache der Grundfrequenz möglich. In der Praxis wird (bis auf wenige Ausnahmen) nur die 2. Harmonische oder 3. Harmonische der Grundfrequenz verwendet (Verdoppelung, Verdreifachung).
Um höhere Frequenzvervielfachungen zu erreichen, werden daher Stufen mit Verdoppelung oder Verdreifachung hintereinandergeschaltet, so dass sich deren Faktoren anschließend multiplizieren.

[question:AF311]

Durch Frequenzvervielfachung und ggf. deren Hintereinanderschaltung werden Frequenzprodukte erzeugt, die oft zu Störungen führen können. Daher müssen Stufen der Frequenzvervielfachung sehr gut abgeschirmt sein, um unerwünschte Abstrahlungen maximal zu reduzieren.

[question:AF313]

Eine typische Vervielfacher-Schaltung (siehe Abbildung [ref:a_frequenzvervielfacher_schaltung]) enthält eine Verstärkerstufe, welche bewusst mit fehlender Basis-Vorspannung betrieben wird. Hierdurch entsteht ein Verstärker im Klasse-C Betrieb, der das Eingangssignal stark verzerrt und an dessen Ausgang das Signal mittels Filtern entnommen wird. Hierbei kommen für die Filter entsprechende Schwingkreise zum Einsatz, die auf der gewünschten Frequenz in Resonanz sind und meist abstimmbar sind.

<margin>
[picture:489:a_frequenzvervielfacher_schaltung:Beispiel für eine Schaltung eines Frequenzvervielfachers mit Klasse-C-Verstärker ohne Basis-Vorspannung]
</margin>

[question:AF312]

Wenn mehrere Vervielfacher-Stufen innerhalb eines Gerätes hintereinandergeschaltet sind, kann es zu Störungen auf Frequenzen kommen, die sich zwischen den einzelnen Vervielfacher-Stufen bilden. Um diese Frequenzen zu ermitteln, muss man den Weg des Signals durch die einzelnen Stufen und dessen danach vorhandene Frequenzen berechnen. Daher ist die Reihenfolge der entsprechenden Vervielfacher-Stufen von entscheidender Bedeutung bei der Ermittlung von Störfrequenzen, denn nur gewisse Frequenzen sind mathematisch möglich.

[question:AF314]
