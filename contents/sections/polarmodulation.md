Ein bereits seit Jahrzehnten bekanntes Verfahren findet seit einiger Zeit verstärkt Anwendung im Amateurfunk: die *Polarmodulation*.

Zu diesem Thema gibt es keine Prüfungsfrage. Aber die Polarmodulation ist ein spannendes Verfahren, das in Zukunft immer stärker in Amateurfunkgeräten eingesetzt werden wird. Daher sei sie hier kurz vorgestellt:

Sie basiert auf der Beobachtung, was passiert, wenn ich in ein beliebiges Signal einigermaßen schmaler Bandbreite zeitlich hinein zoome: Der einzelne Wellenzug so aus wie eine Sinuswelle.

Diese Sinuswelle ist definiert durch wenige Zahlen: Frequenz, Phase und Amplitude.  Wobei Frequenz und Phase miteinander verkoppelt sind: Wer mit einer bestimmten Grundfrequenz anfängt, aber dann bei jedem Wellenzug immer wieder dieselbe Phasenänderung vornimmt, landet bei einer anderen, versetzten Frequenz.

Aus diesen Überlegungen ergibt sich das Verfahren der *Polarmodulation*.  Mit ihm können beliebige Signale einigermaßen schmaler Bandbreite erzeugt werden, zum Beispiel SSB-Signale. Dazu müssen nur, ausgehend von einer Grundfrequenz, Phase und Amplitude des Signals gleichzeitig kontrollierbar sein.

Abbildung [ref:polar_modulator] zeigt das Blochschaltbild des Verfahrens. Dabei werden die beiden Signalkomponenten $I(t)$ und $Q(t)$ (wie sie im vorherigen Kapitel beschrieben wurden) in die momentane Amplitude $A(t)$ und die momentane Phase $\varphi(t)$ umgerechnet:

$A(t)=\sqrt{I^2(t)+Q^2(t)}$

$\varphi(t)=\operatorname{atan2}\left(Q(t),I(t)\right)$

Die Phaseninformation $\varphi(t)$ moduliert anschließend einen HF-Träger mit zunächst konstanter Amplitude. Das entstehende Signal immer noch konstanter Amplitude enthält damit bereits die vollständige Phaseninformation. Es kann von einer besonders effiziente Schaltendstufe verstärkt werden, beispielsweise einem Klasse-E-Verstärker. Solche Endstufen erreichen in der Praxis häufig Wirkungsgrade von mehr als $\qtyrange{80}{90}{\percent}$.

Aber wie kommt die Amplitudenmodulation ins Bild? Dazu wird einfach die Versorgungsspannung der Endstufe entsprechend manipuliert. Ihr wird die Amplitudeninformation $A(t)$ über einen Hüllkurvenverstärker aufgeprägt. Dadurch verändert sich die Ausgangsamplitude entsprechend der gerade nötigen Amplitude, es ergibt sich die gewünschten Hüllkurve. Am Ausgang entsteht wieder das vollständige amplituden- und phasenmodulierte Signal:

$s(t)=A(t)\cos\left(\omega_\mathrm{T}t+\varphi(t)\right)$

Damit das Signal möglichst unverzerrt bleibt, müssen der Amplituden- und der Phasenpfad zeitlich genau aufeinander abgestimmt sein.

Für den Hüllkurvenverstärker genügt ein relativ langsamer NF-Verstärker. Welchen Frequenzbereich er abdecken muss, hängt von der Bandbreite des zu erzeugenden Signals ab. Um den Wirkungsgrad hoch zu halten, wird hier gewöhnlich Schaltnetzteil-Technologie eingesetzt ("Klasse D"-NF-Verstärker).

Durch den hohen Wirkungsgrad wird wenig elektrische Leistung in Wärme umgesetzt. Das spart Energie, verringert den Kühlbedarf und ermöglicht kleinere und leichtere Funkgeräte ohne große Metallkühlkörper und mit billigeren Endstufentransistoren. Polarmodulation eignet sich besonders für batteriebetriebene QRP-Funkgeräte, wird aber auch in leistungsfähigeren kommerziellen Transceivern eingesetzt.

Das Verfahren wurde in den 1970er Jahren unter dem Namen "HELAPS" erstmals beim Satelliten AO-7 eingesetzt. Damals wurde die nötige Extraktion von Phase und Amplitude mit analogen Mitteln bewerkstelligt. Inzwischen sind potente CPUs, die diese Aufgaben problemlos digital übernehmen können, billiger geworden als eine Pizza.

<margin>
[picture:1117:polar_modulator:Polar Modulator]
</margin>
