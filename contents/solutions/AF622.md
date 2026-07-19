Aliasing beschreibt das Auftreten von Mehrdeutigkeiten beim Abtasten eines analogen Signals mit einem A/D-Umsetzer. Die richtige Antwort betrifft daher den A/D-Umsetzer. Der D/A-Umsetzer generiert ein stufenweise analoges Signal und benötigt ein *Rekonstruktionsfilter*, um nach der D/A-Umsetzung den gewünschten Frequenzbereich herauszufiltern.

Um zu entscheiden, ob ein Hoch- oder Tiefpassfilter verwendet werden kann, betrachten wir das Abtasttheorem, das auch in den Hilfsmitteln zu finden ist:

$f_\text{abtast} > 2 \cdot f_{\mathrm{max}}$

Es besagt, dass die höchste Signalfrequenz immer kleiner als die Abtastrate sein muss. Dies ist mit einem Hochpassfilter nicht zu erfüllen, da dieses alle Frequenzen von seiner Grenzfrequenz $f_\mathrm{g}$ bis (zumindest theoretisch) unendlich passieren lässt. Ein Tiefpass dagegen lässt alle Frequenzen von $\qty{0}{\hertz}$ bis zu seiner Grenzfrequenz $f_\mathrm{g}$ passieren. Daher kann mit einem passend dimensionierten Tiefpass das Abtasttheorem eingehalten werden. Die Grenzfrequenz muss dafür deutlich kleiner als die halbe Abtastrate sein.