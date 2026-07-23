Ein bereits seit Jahrzehnten bekanntes Verfahren findet seit einiger Zeit verstärkt Anwendung im Amateurfunk: die *Polarmodulation*. Abbildung [ref:polar_modulator] zeigt das Blochschaltbild des Verfahrens. Dabei werden die beiden Signalkomponenten $I(t)$ und $Q(t)$, wie im vorherigen Kapitel beschrieben, in die momentane Amplitude $A(t)$ und die Phase $\varphi(t)$ umgerechnet:

$A(t)=\sqrt{I^2(t)+Q^2(t)}$

$\varphi(t)=\operatorname{atan2}\left(Q(t),I(t)\right)$

Die Phaseninformation $\varphi(t)$ moduliert anschließend einen HF-Träger mit konstanter Amplitude. Das entstehende Signal enthält damit bereits die vollständige Phaseninformation, besitzt jedoch weiterhin eine konstante Hüllkurve. Deshalb muss es nicht mit einer linearen Endstufe verstärkt werden. Stattdessen kann eine besonders effiziente Schaltendstufe, beispielsweise ein Klasse-E-Verstärker, eingesetzt werden. Solche Endstufen erreichen in der Praxis häufig Wirkungsgrade von mehr als $\qtyrange{80}{90}{\percent}$.

Die Amplitudeninformation $A(t)$ wird über einen schnellen Hüllkurvenverstärker auf die Versorgungsspannung der Endstufe aufgeprägt. Dadurch verändert sich die Ausgangsamplitude entsprechend der gewünschten Hüllkurve. Am Ausgang entsteht wieder das vollständige amplituden- und phasenmodulierte Signal:

$s(t)=A(t)\cos\left(\omega_\mathrm{T}t+\varphi(t)\right)$

Damit das Signal möglichst unverzerrt bleibt, müssen der Amplituden- und der Phasenpfad zeitlich sehr genau aufeinander abgestimmt sein.

Durch den hohen Wirkungsgrad der Endstufe wird weniger elektrische Leistung in Wärme umgesetzt. Das spart Strom, verringert den Kühlbedarf und ermöglicht kleinere und leichtere Funkgeräte ohne große Metallkühlkörper. Polarmodulation eignet sich daher besonders für batteriebetriebene QRP-Funkgeräte, wird inzwischen aber auch in leistungsfähigeren kommerziellen Transceivern eingesetzt. Zu diesem Thema gibt es keine direkte Prüfungsfrage aber ist ein spannendes Verfahren was in Zukunft immer stärker in Amateurfunkgeräten eingesetzt werden wird.

<margin>
[picture:1117:polar_modulator:Polar Modulator]
</margin>