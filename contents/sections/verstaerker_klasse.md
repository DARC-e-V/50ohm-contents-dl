Wie wir in den vorherigen Abschnitten gesehen haben, haben Transistoren eine Kennlinie, die den Zusammenhang zwischen Eingangssignal (Basis-Emitter- oder Gate-Source-Spannung) und Ausgangssignal (Kollektor-/Drainstrom) darstellt. Hierbei gibt es im Bereich der Kennlinie verschiedene Abschnitte, in denen der Transistor eine lineare oder auch nichtlineare Charakteristik hat. Gerade Bereiche der Kennlinie, in denen eine Änderung der Steuergröße eine proportionale Änderung der Ausgangsgröße bewirkt, werden als linear bezeichnet. Andere Bereiche der Kennlinie, in denen eine Änderung der Steuergröße **keine** proportionale Änderung der Ausgangsgröße bewirkt, werden als nichtlinear bezeichnet.

<margin>
[picture:1085:a_kennlinien_transistor_arbeitspunkt:Vereinfachte Eingangskennlinie eines Transistors mit verschiedenen Arbeitspunkten]  
</margin>

Die Vorspannung an der Basis beziehungsweise am Gate legt zunächst den Ruhearbeitspunkt des Transistors fest. Zusammen mit der Größe des Eingangssignals bestimmt dieser, über welchen Bereich der Kennlinie der Transistor ausgesteuert wird und während welchen Anteils einer Signalperiode Strom fließt. Daraus ergeben sich die Verstärkerklassen A, A/B, B und C mit unterschiedlichen Eigenschaften hinsichtlich Wirkungsgrad, Linearität, Stromflusswinkel und Oberwellenanteil. Abbildung [ref:a_kennlinien_transistor_arbeitspunkt] zeigt die typischen Ruhearbeitspunkte der verschiedenen Verstärkerklassen für den A-, B-, A/B- und C-Betrieb. Durch den Aufbau der gesamten Verstärkerschaltung können deren jeweilige Vor- und Nachteile gezielt genutzt oder teilweise ausgeglichen werden. Im Folgenden werden wir uns die verschiedenen Verstärkerklassen anschauen. 

[question:AD416]

---

% A-Betrieb des Verstärkers:

Beim *A-Betrieb* wird der Arbeitspunkt so gewählt, dass der Transistor während der gesamten Signalperiode leitend bleibt (Stromflusswinkel $\qty{360}{\degree}$). Für eine möglichst große und symmetrische Aussteuerung liegt der Ruhearbeitspunkt häufig ungefähr in der Mitte der Arbeitsgeraden, also zwischen Sperrung und Sättigung, sodass der Transistor vollständig im linearen Bereich arbeitet. Die Verstärkung des Eingangssignals (vgl. [ref:a_eingangsspannung]) erfolgt dann um den gewünschten Arbeitspunkt herum, der das Zentrum des Arbeitsbereiches definiert. Durch die Wahl des Arbeitspunktes ergibt sich ein entsprechender Ruhestrom ($I_\mathrm{A}$) des Transistors (vgl. [ref:a_ausgangsstrom_a]). Dieser fließt auch ohne vorhandenes Eingangssignal. Der Ruhestrom beeinflusst die Effizienz eines Verstärkers maßgeblich, da er dessen thermische Verlustleistung erhöht und damit dessen Wirkungsgrad reduziert. Im A-Betrieb erreicht man so üblicherweise einen Wirkungsgrad von ca. $\eta = \qty{40}{\percent}$, was für einen linearen Verstärker ein guter Wert ist. Der Oberwellenanteil ist im A-Betrieb sehr gering, da der Transistor vollständig im linearen Bereich arbeitet.

Alle Signale, deren Modulations-Information sich in deren Amplitude befindet, müssen in der Regel linear verstärkt werden, um die übertragene Information verzerrungsfrei zu übermitteln (SSB, AM etc.). Es gibt allerdings auch schaltungstechnische Tricks, durch die ein linearer A-Betrieb nicht unbedingt erforderlich ist. Signale, deren Modulations-Information sich nicht in der Amplitude sondern nur in der Frequenz befindet, können auch im nichtlinearen Bereich eines Verstärkers verstärkt werden (FM etc.) und anschließend gefiltert werden.

Zusammenfassung A-Betrieb:

- Wirkungsgrad ca. $\qty{40}{\percent}$
- sehr geringer Oberwellenanteil
- Eignet sich gut für AM und SSB
- Ein Ausgangsstrom fließt durch die gesamte Periode (Stromflusswinkel $\Theta =\qty{360}{\degree}$) des Eingangssignals

<margin>
[picture:1086:a_eingangsspannung:Beispiel für eine HF-Eingangsspannung $U_\mathrm{BE}$ eines Transistors]
[picture:1087:a_ausgangsstrom_a:Beispiel für einen HF-Ausgangsstrom $I_\mathrm{C}$ eines Transistors im A-Betrieb]
</margin>

[question:AD419]

Die Ausgangsleistung eines Verstärkers kann durch Kenntnis des Arbeitspunktes und damit dessen ungefähren Wirkungsgrads grob berechnet werden. Hierbei berechnet man zunächst die Gleichspannungsleistung aus dem Produkt von Spannung und Strom, die dem Verstärker zugeführt wird. Anschließend multipliziert man diese Leistung mit dem numerischen Faktor des Wirkungsgrads, wobei $\qty{100}{\percent}$ einem Wirkungsgrad von $1$ entsprechen. Beispielsweise entspricht ein Wirkungsgrad von $\qty{40}{\percent}$ dann einem Faktor von $0,4$. Versuche nun die folgenden Aufgaben zu lösen:

[question:AD424]

% B-Betrieb des Verstärkers:

Wird der Arbeitspunkt für den *B-Betrieb* gewählt, liegt der Transistor idealerweise gerade am Sperrpunkt. Ohne Eingangssignal fließt daher praktisch kein Ruhestrom. Bei einer sinusförmigen Ansteuerung, wie in Abbildung [ref:a_eingangsspannung] dargestellt, beginnt der Transistor erst ab einer bestimmten Eingangsspannung zu leiten. Ein einzelner Transistor ist deshalb nur während einer Halbwelle beziehungsweise über einen Stromflusswinkel von $\qty{180}{\degree}$ aktiv.
Da im Ruhezustand nahezu keine Leistung aufgenommen wird, kann der theoretische Wirkungsgrad eines idealen B-Verstärkers bis zu rund $\qty{80}{\percent}$ betragen. Der Stromverlauf eines einzelnen Transistors ist jedoch nicht mehr sinusförmig und enthält daher einen hohen Oberwellenanteil. 

Um Oberwellen zu verringern beziehungsweise zu unterdrücken, gibt es in der Praxis verschiedene Lösungsmöglichkeiten:

- Eine Möglichkeit ist eine Gegentaktschaltung, im Englischen *push-pull amplifier*, mit zwei Transistoren, wie in Abbildung [ref:a_gegentakt] dargestellt. Dabei verstärkt jeder Transistor jeweils eine Halbwelle, sodass beide Halbwellen wieder zu einem vollständigen Sinussignal zusammengesetzt werden und der Oberwellenanteil deutlich reduziert wird.
- Neben einer Gegentaktstufe kann bei schmalbandigen HF-Verstärkern ein abgestimmter Schwingkreis verwendet werden. Der Transistor liefert dabei nur während einer Halbwelle Stromimpulse. Der Schwingkreis speichert Energie und schwingt zwischen den Stromimpulsen weiter, sodass am Ausgang wieder ein nahezu sinusförmiges Signal über die vollständige Periode entsteht. Oder anders ausgedrückt: Der Schwingkreis wirkt wie ein Filter, das die Oberwellenanteile unterdrückt. Diese Lösung ist jedoch nur für schmalbandige HF-Verstärker geeignet, da ein Schwingkreis nur in einem engen Frequenzbereich resonant ist.

<margin>
[picture:1089:a_ausgangsstrom_b:Beispiel für einen HF-Ausgangsstrom $I_\mathrm{C}$ eines Transistors im B-Betrieb]
[picture:1091:a_gegentakt:Gegentaktstufe mit zwei Transistoren, die jeweils eine Halbwelle verstärken]
</margin>

Zusammenfassung B-Betrieb:
- Geringe Vorspannung bis zum Einsetzen des Kollektorstroms
- Ruhestrom fast null
- Wirkungsgrad ca. bis zu $\qty{80}{\percent}$
- Geringer Oberwellenanteil mit Gegentaktstufe oder Schwingkreis
- Stromflusswinkel von $\Theta = \qty{180}{\degree}$, d.h. nur eine Halbwelle wird verstärkt

[question:AD420]
[question:AD417]

---

% A/B-Betrieb des Verstärkers:

Eine weitere Möglichkeit, einen Verstärker zu realisieren, ist der A/B-Betrieb, bei dem der Arbeitspunkt zwischen A- und B-Betrieb liegt. Der Ruhestrom ($I_\mathrm{A/B}$) ist dabei größer als im B-Betrieb, jedoch deutlich geringer als im A-Betrieb, wie in Abbildung [ref:a_ausgangsstrom_ab] dargestellt. Der Wirkungsgrad liegt zwischen $\qty{50}{\percent}$ und $\qty{80}{\percent}$ und der Oberwellenanteil ist mit entsprechender Schaltungstechnik ebenfalls gering.

Zusammenfassung A/B-Betrieb des Verstärkers
- Höhere Vorspannung als im B-Betrieb, jedoch geringer als im A-Betrieb
- Ruhestrom größer als im B-Betrieb, aber deutlich geringer als im A-Betrieb
- Wirkungsgrad zwischen $\qty{50}{\percent}$ und $\qty{80}{\percent}$
- Geringer Oberwellenanteil
- Stromflusswinkel: $\qty{180}{\degree} < \Theta < \qty{360}{\degree}$

Insbesondere beim A/B- oder B-Betrieb eines Verstärkers ist Übersteuerung zu vermeiden, da diese schnell zu Verzerrungen des Signals führen kann. Diese äußern sich bei SSB in Form von Splatter auf benachbarten Frequenzen.
[question:AD423]

<margin>
[picture:1088:a_ausgangsstrom_ab:Beispiel für einen HF-Ausgangsstrom $I_\mathrm{C}$ eines Transistors im A/B-Betrieb]
</margin>

---

% C-Betrieb des Verstärkers:

Der sogenannte *C-Betrieb* ist stark nichtlinear, weil der Transistor nur während eines kleinen Teils der Eingangsschwingung leitet (vgl. Abbildung [ref:a_ausgangsstrom_c]). Der Stromflusswinkel beträgt weniger als $\qty{180}{\degree}$ und ohne Eingangssignal fließt idealerweise kein Ruhestrom. Dadurch können hohe Wirkungsgrade von typischerweise etwa $\qtyrange{80}{87}{\percent}$ erreicht werden.

Da der Transistor nur kurze Stromimpulse erzeugt, enthält sein Ausgangssignal starke Oberwellenanteile. Ein abgestimmter Schwingkreis oder ein nachgeschaltetes Filter wählt die gewünschte Ausgangsfrequenz aus und unterdrückt die unerwünschten Oberwellen. Da diese Oberwellen innerhalb des Leistungsverstärkers und des Filters noch erhebliche Leistungen besitzen können, müssen die Schaltung und ihre Leitungen sorgfältig aufgebaut und abgeschirmt werden, damit keine unerwünschten Signale abgestrahlt werden.

Der C-Betrieb eignet sich besonders für Signale mit konstanter Hüllkurve, beispielsweise für FM und CW. Für AM und SSB ist er ohne zusätzliche Maßnahmen ungeeignet, da die Amplitudeninformation durch die nichtlineare Verstärkung verzerrt würde. Deshalb werden für AM- und SSB-Verstärker in der Regel A-, B- oder A/B-Betrieb verwendet. Mit besonderen Verfahren wie der Polarmodulation können jedoch auch amplitudenmodulierte Signale mithilfe hocheffizienter, nichtlinearer Verstärker erzeugt werden. Darauf gehen wir in einem späteren Abschnitt noch genauer ein.

Zusammenfassung: C-Betrieb des Verstärkers
- Ohne Vorspannung
- Ruhestrom null
- Wirkungsgrad ca. $\qtyrange{80}{87}{\percent}$
- Erzeugt von allen Verstärkerklassen den höchsten Oberwellenanteil
- Stromflusswinkel von $\Theta < \qty{180}{\degree}$, d.h. nur ein kleiner Teil der Sinuswelle wird verstärkt

<margin>
[picture:1090:a_ausgangsstrom_c:Beispiel für einen HF-Ausgangsstrom $I_\mathrm{C}$ eines Transistors im C-Betrieb]
</margin>

[question:AD418]
[question:AD425]
[question:AD421]
[question:AD422]
[question:AJ218]
[question:AF402]
[question:AF403]

Fassen wir die gelernten Verstärkerklassen noch einmal in einer Übersicht zusammen:

| l: Eigenschaft | X: A-Betrieb | X: B-Betrieb | X: A/B-Betrieb | X: C-Betrieb |
| Ruhestrom | $I_\mathrm{A}$ | 0 | $I_\mathrm{A/B}$ | 0 |
| Wirkungsgrad | $\qty{40}{\percent}$ | bis zu $\qty{80}{\percent}$ | $\qtyrange{50}{80}{\percent}$ | $\qtyrange{80}{87}{\percent}$ |
| Stromflusswinkel | $\Theta = \qty{360}{\degree}$ | $\Theta = \qty{180}{\degree}$ | $\qty{180}{\degree} < \Theta < \qty{360}{\degree}$ | $\Theta < \qty{180}{\degree}$ |
| Maßnahmen gegen Oberwellen | Filter | Gegentaktstufe oder Filter | Gegentaktstufe oder Filter | Filter |

Neben den klassischen Verstärkerklassen A, B, AB und C gibt es weitere hocheffiziente Verstärkerklassen wie die Klassen D, E und F. Bei Klasse-D- und Klasse-E-Verstärkern wird der Transistor gezielt als Schalter betrieben, sodass möglichst wenig Leistung im Transistor selbst verloren geht. Klasse-F-Verstärker nutzen zusätzlich abgestimmte Netzwerke für die Grundfrequenz und ausgewählte Oberwellen, um Strom- und Spannungsverläufe am Transistor günstig zu formen. Auf diese Weise können sehr hohe Wirkungsgrade erreicht werden. Solche Verstärker erfordern jedoch eine sorgfältige Schaltungsauslegung und sind im HF-Bereich häufig nur für einen begrenzten Frequenzbereich geeignet. Weitere Betriebsarten wie Klasse J oder Klasse S verfolgen ähnliche Ziele, sind für die Amateurfunkprüfung jedoch nicht relevant.