Bei der Amplitudenmodulation (AM) sowie bei SSB wird die zu übertragende Information durch eine Änderung der Amplitude des Hochfrequenzträgers übertragen. In der Klasse N haben wir bereits gelernt, dass bei der Frequenzmodulation (FM) die Amplitude des Trägers hingegen konstant bleibt - die Information wird hier durch eine Änderung der momentanen Frequenz des Trägers übertragen.

Abbildung [ref:e_frequenzmodulation_t] zeigt den zeitlichen Verlauf eines FM-Signals mit konstanter Amplitude. Ein FM-Signal ist daher daran zu erkennen, dass die Amplitude des Trägers (idealisiert) konstant bleibt, während sich seine momentane Frequenz in Abhängigkeit vom Modulationssignal fortlaufend ändert.

<margin>
[picture:906:e_frequenzmodulation_t:Zeitlicher Verlauf eines FM-Signals]
</margin>

[question:EE301]

---

Abbildung [ref:e_frequenzmodulation_frequenzhub] zeigt beispielhaft ein NF-Sinussignal, das eine entsprechende Frequenzabweichung (Frequenzhub) eines Hochfrequenzträgers im Spektrum verursacht. Das heißt bei einem FM-Signal wird die Lautstärkeinformation durch die *Trägerfrequenzauslenkung (Frequenzhub)* übertragen. Eine lauteres NF-Signal würde zu einer größeren Trägerfrequenzauslenkung und somit einer höheren Bandbreite des FM-Signals führen .

<margin>
[picture:827:e_frequenzmodulation_frequenzhub:Trägerauslenkung bei Frequenzmodulation]
</margin>

<indepth>
Die belegte Bandbreite einer FM-Aussendung wird durch den Hub und die maximale Modulationsfrequenz bestimmt. In erster Näherung kann für kleinen Hub und niedrige Modulationsfrequenz die *Carson-Formel* angewendet werden. Sie gibt an in welcher Bandbreite sich $\qty{99}{\percent}$ der Sendeleistung befinden.

$B\approx2 \cdot \left(\Delta f_{\textrm{T}} + f_{\textrm{mod max}} \right)$
  
Dieses Thema wird genauer in der Klasse A besprochen. 
</indepth>

[question:EE306]
[question:EE304]

Um die gesetzlichen Vorgaben hinsichtlich der belegten Bandbreite eines FM-Signals einzuhalten, wird in FM-Sendern das Mikrofonsignal zunächst in der Amplitude begrenzt (durch einen Begrenzerverstärker) und anschließend auf den Träger mittels FM aufmoduliert. Hierbei ist der Frequenzhub des Modulators bei maximaler Lautstärkeaussteuerung entweder festgelegt oder mittels eines Hub-Reglers einstellbar.

[question:EE305]

FM-Signale sind dadurch, dass die aufmodulierte Information nicht in der Amplitude, sondern lediglich in der Frequenz enthalten ist, gegenüber Amplitudenstörungen (z.B. durch Blitze, Zündanlagen, Motoren) relativ unempfindlich im Vergleich zu AM oder SSB. Hierdurch ergeben sich insbesondere beim Betrieb in KFZ und in gestörten Umgebungen Vorteile hinsichtlich der Störanfälligkeit.

[question:EE302]
[question:EE303]