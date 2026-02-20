In der Klasse N aben wir bereits einige Antennenformen kennen gelernt. In der Klasse E wollen wir nun die Eigenschaften der verscheidenen Antennen genauer besprechen. Mittengespeiste Dipole sind *symmetrische Antennen*. Unter einer symmetrischen Antenne verstehen wir eine Antenne, die im Idealfall im Betrieb an beiden Polen (z. B. den Einspeisepunkten jedes Schenkels eines Dipols) bis auf das Vorzeichen die gleiche Spannung gegenüber Erde aufweist. Dies ist bei Dipolen einschließlich Faltdipol und auch den darauf basierenden Yagi-Uda-Antennen der Fall. Eine Groundplane-Antenne hingegen weist am Anschlusspunkt der Radiale idealerweise Erdpotential auf (also eine Spannung von Null gegenüber der Erde) und zählt damit nicht zu den symmetrischen Antennen.

<indepth>
Auch bei Kabeln zur Signalübertragung, z. B. der Speiseleitung einer Antenne, unterscheidet man zwischen *symmetrischen und asymmetrischen Kabeln*. Auch hier bezieht sich die Symmetrie auf die im Idealfall vorherrschenden elektrischen Spannungen gegenüber Erde. Bei einem Koaxialkabel sollten zwar die Ströme symmetrisch sein, jedoch nur der Innenleiter Spannung gegenüber Erde führen. Koaxialkabel gehören daher zu den asymmetrischen Speiseleitungen. Wie wir später lernen werden, sollten diese asymmetrischen Speiseleitungen nur mittels eines sogenannten Symmetrierglieds (Balun) an eine symmetrische Antenne angeschlossen werden.
</indepth>

[question:EG213]

---

Eine beliebte Antennenbauform ist ein insgesamt etwa eine Wellenlänge langer Draht in Form eines Kreises, eines Quadrates, eines Dreiecks oder einer ähnlichen Form. Man spricht dann von sogenannten Ganzwellen-*Schleifenantennen*. Aufgrund ihres einfachen Aufbaus sehr beliebt ist die sogenannte Delta-Loop-Antenne, welche, wie das große Delta (Δ) aus dem griechischen Alphabet, die Form eines Dreiecks hat.

<margin>
[picture:311:e_delta_loop:Beispiel für eine Delta-Loop-Antenne]
</margin>

[question:EG101]

<indepth>
Auf die genaue *Form* kommt es bei den Ganzwellen-Schleifenantennen nicht an, sofern die Drahtlänge etwa einer Wellenlänge entspricht. Je nach Form können sich jedoch andere Speisewiderstände oder geringfügig bessere oder schlechtere Antennengewinne ergeben.
</indepth>

---

Von den Ganzwellen-Schleifenantennen zu unterscheiden sind die sogenannten *magnetischen Ringantennen* (Magnetic-Loops), die in Bezug auf die Wellenlänge viel kleinere Abmessungen aufweisen und ein magnetisches Nahfeld erzeugen (vgl. Abbildung [ref:e_mag_loop]).

<margin>
[picture:977:e_mag_loop:Beispiel für eine Magnetic-Loop-Antenne]
</margin>

[question:EG105]

<indepth>
Obwohl solche magnetischen Ringantennen grundsätzlich auch für den Sendebetrieb geeignet sind, ist es schwierig, einen hohen *Wirkungsgrad* zu erzielen. Wirkungsgrade zwischen $\qty{1}{\percent}$ und $\qty{10}{\percent}$ sind bei Magnetantennen im Sendebetrieb üblich. Dennoch können diese Magnetic-Loops gegenüber anderen Antennen Vorteile bieten: Neben dem kompakten Aufbau stören sie sich oft weniger an im Nahfeld befindlichen elektrisch leitfähigen oder dämpfenden Gegenständen, z. B. Mauern oder Dachziegeln bei Montage im Innenraum oder unter einem Hausdach. 
</indepth>

---

*Endgespeiste Antennen* werden von einem Ende her gespeist. Meist beträgt ihre Länge eine halbe Wellenlänge. Man spricht dann auch von einem endgespeisten Halbwellendipol (englisch: end fed half wave, EFHW). Eine solche Antenne benötigt eine im Verhältnis zum Strom deutlich höhere Spannung, welche durch ein entsprechendes Anpassglied, z. B. einen Fuchskreis erzeugt werden kann. Endgespeiste Halbwellendipole, die mit einem Fuchskreis angepasst werden, bezeichnet man entsprechend als Fuchsantenne.

[question:EG104]
[question:EG103]

<margin>
[picture:310:e_fuchsantenne:Beispiel für eine Fuchs-Antenne]
</margin>

<person>
Der Fuchskreis bzw. die Fuchs-Antenne ist benannt nach *Dr. Josef Fuchs* (Amateurfunkrufzeichen OE1JF, UO1JF und EAAA), der diese im Jahre 1927 auch patentieren ließ.
</person>

<indepth>
Auch eine endgespeiste Antenne benötigt ein *Gegengewicht*, z. B. in Form eines $\lambda / 4$-Drahtes oder einer anderen Form der HF-Erdung. Allerdings sind die auftretenden Ströme bei EFHWs am Speisepunkt deutlich kleiner, weshalb auch eine weniger gute Erdung ausreichend sein kann, z. B. ein kurzes Drahtende von nur einem zehntel oder gar zwanzigstel der Wellenlänge. Manchmal dienen sogar nur der Schirm der Speiseleitung oder andere (eigentlich anderen Zwecken dienende) Metellelemente als Erdung.
  
Nicht zu Verwechseln mit den endgespeisten Halbwellendipolen sind die endgepeisten *Langdrahtantennen*, bei denen die Länge deutlich über einer Wellenlänge liegt. Die Verwechselung rührt daher, dass endgespeiste Halbwellendipole oft auch auf höheren Frequenzen betrieben werden, wodurch sie für diese Frequenzen dann de-facto eine Langdrahtantenne darstellen.
</indepth>

---

Die Richtwirkung einer Antenne kann man in einem sogenannten Strahlungsdiagramm darstellen. Hierbei wird für eine Ebene in jede Richtung der Gewinn bzw. die Feldstärke oder Strahlungsleistung aufgetragen. Je weiter der Graphenverlauf vom Mittelpunkt entfernt ist, umso größer der Gewinn bzw. umso höher die Feldstärke und Strahlungsleistung im Fernfeld. Falls keine Skala mit Winkeln verwendet wird, stellt man auch oft die mechanische Anordnung der Antenne im selben Diagramm dar, um zu verdeutlichen, welche Richtung im Diagramm welcher Richtung in Bezug auf die Antennenanordnung entspricht.

Ein Dipol strahlt nicht, wie man irrigerweise vermuten könnte, in Richtung des Drahtes, sondern rechtwinklig davon ab. In einer Ebene betrachtet und aufgetragen als Strahlungsdiagramm ergeben sich entsprechende Keulen (z. B. links und rechts) neben dem Dipol (vgl. Abbildung [ref:e_dipol_strahlungsdiagramm]). Ein vertikal aufgehanger Dipol strahlt also z. B. nach links und rechts sowie nach vorne und hinten ab. Da das Strahlungsdiagramm nur eine Ebene betrachtet, sieht man z. B. nur eine Keule für die Abstrahlung nach links und eine Keule für die Abstrahlung nach rechts. Je nach Skala können diese Keulen kreisförmig aussehen.

<margin>
[picture:1045:e_dipol_strahlungsdiagramm:Beispiel für die Abstrahlung des Dipols]
</margin>

<indepth>
Eine im Querschnitt *kreisförmige Keule* ergibt sich bei einer Skala, die linear zur Feldstärke ist, dann wenn ein stark verkürzter Dipol (hertzscher Dipol) betrachtet wird. Ein Halbwellendipol hat eigentlich einen etwas höheren Gewinn entsprechend einer etwas schmaleren Keule. Dennoch finden wir in den Prüfungsfragen eine kreisförmige Darstellung, die so nur näherungsweise stimmt. Bei einer Skala, die linear zur Strahlungsleistung in der jeweiligen Richtung wäre, müsste die Keule sogar noch schmaler ausfallen.
% TODO: ggf. Fragenbild korrigieren
</indepth>

[question:EG215]
[question:EG214]

---

Aufgrund der zum Dipol senkrechten Abstrahlcharakteristik kann ein vertikal montierter Halbwellendipol entsprechend eine flache Abstrahlung ermöglichen, die z. B. im DX-Betrieb aber auch bei Kontakten über Direkt- oder Bodenwelle erwünscht sein kann.

[question:EG219]

<margin>
[photo:316:e_vertikaldipol:Vertikaler $\frac{\lambda}{2}$-Dipol]
</margin>

---

Einen Spezialfall einer Vertikalantenne stellt die gegen Erde (oder einer Fahrzeugkarosserie) erregte $5/8 \lambda$-Antenne dar (vgl. Abbildung [ref:e_fuenf_achtel]). Hier ist die Länge gerade so gewählt, dass sich ein optimaler Gewinn ergibt.

[question:EG108]

<margin>
[picture:650:e_fuenf_achtel:$5/8 \lambda$-Antenne]
</margin>

---

Auch eine Groundplane-Antenne strahlt rechtwinklig zum Strahler (nicht zu den Radialen) ab. Da das Strahlungsdiagramm die Groundplane-Antenne oft von oben betrachtet, ergibt sich nahezu ein Rundstrahler, der in alle Himmelsrichtungen nahezu den gleichen Gewinn aufweist (vgl. Abbildung [ref:e_ground_plane_abstrahlung]). Die Radiale haben nur geringen Einfluss und können das Strahlungsdiagramm leicht "verbeulen", was einem geringfügig abweichenden Gewinn in bestimmten Richtungen entspricht.

<margin>
[picture:1046:e_ground_plane_abstrahlung:Abstrahlung Groundplane-Antenne]
</margin>

[question:EG216]

<indepth>
Auch wenn das Strahlungsdiagramm einer Groundplane-Antenne mit Radialen leicht *"verbeult"* ist, ist diese Abweichung in der Theorie viel kleiner als oftmals dargestellt. Daher ist eine Groundplane-Antenne tatsächlich ein beinahe idealer Rundstrahler in der Ebene.
</indepth>

---

Richtantennen (z.B. die Yagi-Uda-Antenne) zeichnen sich dadurch aus, dass der Gewinn in einer Richtung deutlich höher ist, als in anderen Richtungen, wie in Abbildung [ref:e_richtantenne_abstrahlung] dargestellt.

[question:EG217]

<margin>
[picture:1047:e_richtantenne_abstrahlung:Abstrahlung Richtantenne]
</margin>

---

Bei höheren Frequenzen z. B. im UHF-Bereich oder darüber hinaus kommen auch Hornstrahler oder Parabolantennen (vgl. [ref:e_parabolantenne]) zum Einsatz. Ebenso finden sich auf Leiterplatten kleinerer Geräte Patchantennen. All diese Antennenbauformen sind für den Kurzwellenbereich unüblich, da sie unhandliche Größen erreichen würden. Deshalb bleiben für die folgenden Fragen nur noch Langdraht-Antenne, Yagi-Uda-Antenne, Dipol-Antenne, Windom-Antenne, Delta-Loop-Antenne übrig.

[question:EG106]

<margin>
[picture:850:e_parabolantenne:Parabolantenne]
</margin>

Die Sperrtopfantenne besteht aus einem $\lambda / 4$-langen Topf, der als Symmetrierglied bzw. Mantelwellensperre wirkt. Mit diesem Wissen lässt sich die folgende Frage beantworten, denn sowohl ein Sperrtopf als auch eine Kreuz-Yagi-Uda wären ebenso wie Parabolspiegel im $\qty{80}{\meter}$-Band unhandlich groß.

[question:EG107]