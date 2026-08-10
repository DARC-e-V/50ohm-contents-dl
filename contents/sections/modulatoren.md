Dioden haben wir bereits in verschiedenen Schaltungen kennengelernt. Nun betrachten wir, wie ihre nichtlineare Kennlinie genutzt werden kann, um ein hochfrequentes Trägersignal mit einem niederfrequenten Nutzsignal zu modulieren.

Werden ein HF-Signal und ein NF-Signal gemeinsam, wie in Abbildung [ref:a_am_modulator] gezeigt, einer Diode zugeführt, beeinflusst die NF-Spannung die Leitfähigkeit der Diode. Dadurch wird das HF-Signal abhängig vom momentanen Wert der NF unterschiedlich stark übertragen. Seine Amplitude verändert sich somit im Takt des NF-Signals.

Am Ausgang entstehen dadurch neben dem ursprünglichen HF-Träger zwei Seitenbänder oberhalb und unterhalb der Trägerfrequenz. Ein auf die Trägerfrequenz abgestimmter Schwingkreis unterdrückt unerwünschte weitere Frequenzanteile. Am Ausgang erhält man damit ein amplitudenmoduliertes Signal (AM).

<margin>
[picture:772:a_am_modulator:Simpler AM-Modulator mit Diode und Schwingkreis]
</margin>

<webonly>
Die folgende Simulation zeigt die Funktionsweise des AM-Modulators, die Werte wurden so gewählt, dass die HF und NF gut zu erkennen sind. Die NF liegt bei $\qty{500}{\hertz}$, die HF bei $\qty{10}{\kilo\hertz}$. Die Amplitude des HF-Signals wird im Takt der NF verändert. Der Schwingkreis ist auf die Trägerfrequenz abgestimmt und unterdrückt unerwünschte Frequenzanteile. Wenn man den Schwingkreis entfernt, sieht man eine Vielzahl von Mischprodukten. Auch kann man mal die NF-Frequenz auf $\qty{1}{\kilo\hertz}$ umstellen, um zu sehen, wie sich die Seitenbänder verschieben.

[include:applet_am_modulator]
</webonly>

<indepth>
Ein AM-Signal lässt sich auch mathematisch beschreiben. Dazu betrachten wir zunächst ein normiertes sinusförmiges NF-Signal

$m(t)=\cos(\omega t)$

mit der Kreisfrequenz $\omega=2\pi f_\mathrm{m}$. Mit seiner Amplitude $\hat U_\mathrm{m}$ und einem zusätzlichen Gleichanteil $U_\mathrm{G}$ ergibt sich

$U_\mathrm{m}(t)=U_\mathrm{G}+\hat U_\mathrm{m}\cdot\cos(\omega t)$

Dieses Signal wird nun mit dem hochfrequenten Trägersignal

$U_\mathrm{T}(t)=\cos(\Omega t)$

mit $\Omega=2\pi f_\mathrm{T}$ multipliziert. Für das AM-Signal folgt damit:

$U_\mathrm{AM}(t)=\left(U_\mathrm{G}+\hat U_\mathrm{m}\cdot\cos(\omega t)\right)\cdot\cos(\Omega t)$

Ausmultipliziert ergibt sich:

$U_\mathrm{AM}(t)=U_\mathrm{G}\cdot\cos(\Omega t)+\hat U_\mathrm{m}\cdot\cos(\omega t)\cdot\cos(\Omega t)$

Mit der Beziehung

$\cos(a)\cdot\cos(b)=\frac{1}{2}\left(\cos(a+b)+\cos(a-b)\right)$

kann der zweite Term weiter zerlegt werden:

$U_\mathrm{AM}(t)=U_\mathrm{G}\cdot\cos(\Omega t)+\frac{\hat U_\mathrm{m}}{2}\left(\cos((\Omega+\omega)t)+\cos((\Omega-\omega)t)\right)$

Damit erkennt man unmittelbar die drei Bestandteile eines AM-Signals: Der erste Term beschreibt den *Träger* bei der Frequenz $\Omega$. Die beiden anderen Terme bilden das *obere und untere Seitenband* bei den Frequenzen $\Omega+\omega$ und $\Omega-\omega$.

Der Gleichanteil $U_\mathrm{G}$ ist dabei dafür verantwortlich, dass der Träger erhalten bleibt. Selbst wenn das Nutzsignal momentan null ist, wird weiterhin ein Trägersignal erzeugt.

[picture:1127:a_am_modulation:Spektrum eines AM-Signals mit Träger und zwei Seitenbändern]

</indepth>

Dieses Prinzip wird in der folgenden Frage deutlich: Eine Diode wird mit einem NF-Signal und einem HF-Signal gleichzeitig beaufschlagt und das Ausgangs-Signal wird mit einem LC-Schwingkreis ausgefiltert.

[question:AD507]

---

Mit vier Dioden in einer Ringanordnung lässt sich ein Modulator so aufbauen, dass der Träger am Ausgang unterdrückt wird. Eine solche Schaltung haben wir bereits im Kapitel „Mischer II“ als *Balancemischer* kennengelernt. Dort wurde sie verwendet, um ein HF-Signal auf eine Zwischenfrequenz umzusetzen. Im Sender nutzen wir dasselbe Grundprinzip nun zur Erzeugung eines modulierten Signals.

<margin>
[picture:759:a_balancemodulator:Balancemodulator mit Diodenring]
</margin>

Man erkennt einen Balancemischer beziehungsweise Balancemodulator typischerweise an dem Diodenring, wie er in Abbildung [ref:a_balancemodulator] dargestellt ist. Der Diodenring wird vom Oszillatorsignal $f_\mathrm{OSZ}$ angesteuert. Je nach Polarität des Oszillatorsignals leitet jeweils eines der beiden gegenüberliegenden Diodenpaare.

Dadurch wird das NF-Signal abwechselnd mit gleicher oder umgekehrter Polarität zum Ausgang übertragen. Vereinfacht betrachtet wird das NF-Signal also mit dem Oszillatorsignal multipliziert.

Der entscheidende Vorteil der symmetrischen Schaltung ist die *Trägerunterdrückung*: Die Anteile des Oszillatorsignals heben sich am Ausgang idealerweise gegenseitig auf. Ohne NF-Signal entsteht deshalb kein Ausgangssignal. Wird ein NF-Signal angelegt, entstehen dagegen das obere und das untere Seitenband, während der Träger unterdrückt bleibt.

Das Ausgangssignal wird als *Doppelseitenband-Signal mit unterdrücktem Träger* (DSB) bezeichnet.

[question:AE206]
[question:AF302]
[question:AF308]
[question:AD510]

<indepth>
Die Trägerunterdrückung eines Balancemodulators lässt sich vereinfacht mit zwei symmetrischen Zweigen beschreiben:

$u_1(t)=\left(U_G+\hat U_\mathrm{m}\cos(\omega t)\right)\cos(\Omega t)$

$u_2(t)=\left(U_G-\hat U_\mathrm{m}\cos(\omega t)\right)\cos(\Omega t)$

Am Ausgang werden beide Signale voneinander abgezogen:

$u_\mathrm{out}(t)=u_1(t)-u_2(t)$

Damit ergibt sich:

$u_\mathrm{out}(t)=U_G\cos(\Omega t)+\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)-U_G\cos(\Omega t)+\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)$

Die beiden Trägeranteile $U_G\cos(\Omega t)$ heben sich auf. Übrig bleibt:

$u_\mathrm{out}(t)=2\hat U_\mathrm{m}\cos(\omega t)\cos(\Omega t)$

Mit $\cos(a)\cos(b)=\frac{1}{2}\left(\cos(a+b)+\cos(a-b)\right)$ folgt:

$u_\mathrm{out}(t)=\hat U_\mathrm{m}\left(\cos((\Omega+\omega)t)+\cos((\Omega-\omega)t)\right)$

Das Ausgangssignal enthält damit nur noch das obere und das untere Seitenband. Der Träger bei $\Omega$ ist unterdrückt.
</indepth>

---

Damit sich das Oszillatorsignal am Ausgang möglichst vollständig aufhebt, muss die Schaltung symmetrisch, also *ausbalanciert*, sein. Bereits kleine Unterschiede in Amplitude oder Phase zwischen den beiden Signalwegen führen dazu, dass ein Rest des Trägers am Ausgang verbleibt. Die Amplitudensymmetrie kann beispielsweise mit einem Potentiometer abgeglichen werden. Für den Phasenabgleich wird in manchen Schaltungen zusätzlich ein Trimmkondensator verwendet. Ziel des Abgleichs ist eine möglichst hohe Trägerunterdrückung, während die beiden Modulationsseitenbänder erhalten bleiben.

<webonly>
Das folgende Applet zeigt den Trägerabgleich. Wenn der Regler auf der rechten Seite verschoben wird, zeigt sich der Träger plötzlich im Spektrum. 

[include:applet_dsp]
</webonly>

[question:AF309]

---

Der Balancemodulator bildet die erste Stufe eines SSB-Modulators und erzeugt ein DSB-Signal. Hinter dem Balancemodulator folgt als zweite Stufe ein schmalbandiges Bandpassfilter, wie in Abbildung [ref:a_ssb_modulation]. Es lässt nur eines der beiden Seitenbänder passieren und unterdrückt das jeweils andere. Am Ausgang entsteht dadurch ein Einseitenband-Signal (SSB).

<margin>
[picture:500:a_ssb_modulation:Blockschaltbild zur Modulation von SSB mit der Filtermethode]
</margin>

[question:AF306]
[question:AF304]
[question:AF303]
[question:AF305]

---

Eine gute Implementierung für ein Funkgerät, das sowohl USB als auch LSB erzeugen soll, besteht darin, das Bandpassfilter fest auf einen bestimmten Frequenzbereich auszulegen. Ob das obere oder das untere Seitenband ausgefiltert wird, wird nicht durch eine Änderung des Filters bestimmt, sondern durch die Frequenz des Oszillators im Balancemodulator. Dazu stehen zwei unterschiedliche Quarzoszillatoren zur Verfügung.

Wird beispielsweise für USB die Oszillatorfrequenz $\qty{8998,5}{\kilo\hertz}$ gewählt, entstehen durch die Modulation zwei Seitenbänder. Das obere Seitenband wird dabei genau in den Durchlassbereich konstanten Filters verschoben, während das untere Seitenband außerhalb des Durchlassbereichs liegt und unterdrückt wird.

Für LSB wird auf die andere Quarzfrequenz von $\qty{9001,5}{\kilo\hertz}$ umgeschaltet. Dadurch verschiebt sich das gesamte DSB-Spektrum so, dass nun das untere Seitenband in den Durchlassbereich desselben Filters fällt und das obere Seitenband unterdrückt wird.

Der entscheidende Trick besteht also darin, das Filter unverändert zu lassen und stattdessen durch unterschiedliche Oszillatorfrequenzen die Lage des DSB-Signals zu verschieben. Ähnlich wie bei der Zwischenfrequenz eines Empfängers kann dadurch ein fest abgestimmtes, hochwertiges Filter für unterschiedliche Frequenzlagen genutzt werden.

[question:AF307]

<margin>
<latexonly>
[picture:831:a_ssb_modulation_lsb:Frequenzen mit der Filtermethode bei LSB]
[picture:940:a_ssb_modulation_lsb:Spektrum mit der Filtermethode bei LSB]
[picture:832:a_ssb_modulation_usb:Frequenzen mit der Filtermethode bei USB]
[picture:941:a_ssb_modulation_usb:Spektrum mit der Filtermethode bei USB]
</latexonly>
<webonly>
[include:applet_dsp_filter]
</webonly>
</margin>

---

Für die Erzeugung eines frequenzmodulierten Signals (FM) kann eine *Kapazitätsdiode* verwendet werden. Sie ist in Schaltplänen an dem kleinen Kondensatorsymbol neben der Diode zu erkennen, wie in Abbildung [ref:a_fm_modulator].

Eine Kapazitätsdiode wird in Sperrrichtung betrieben. Ihre Kapazität hängt dabei von der anliegenden Sperrspannung ab. Wird sie als Teil des frequenzbestimmenden Schwingkreises eines Oszillators eingesetzt, verändert eine Änderung dieser Spannung die Resonanzfrequenz des Schwingkreises und damit die Frequenz des Oszillators.

Zur Frequenzmodulation wird der Gleichspannung an der Kapazitätsdiode das NF-Signal überlagert. Dadurch ändert sich ihre Kapazität im Takt des NF-Signals und die Oszillatorfrequenz wird entsprechend nach oben und unten verschoben. Auf diese Weise entsteht ein frequenzmoduliertes Signal.

<margin>
[picture:155:a_fm_modulator:FM-Modulator mit Kapazitäts-Diode]
</margin>

[question:AD508]
[question:AF310]

---

Mit großen NF-Spannungen kann man leicht viel größere Frequenzänderungen des Oszillators bewirken (FM-„Hub“) als zulässig. Daher ist eine „Hub“-Begrenzung durch eine Einstellung und Begrenzung der NF-Amplitude notwendig. Antiparallel geschaltete Dioden begrenzen die Spannung auf etwa die Dioden-Knickspannung. Ein Beispiel zeigen die Abbildungen [ref:a_fm_modulator_hub1] und [ref:a_fm_modulator_hub2].

<margin>
[picture:44:a_fm_modulator_hub1:Schaltung zur Hub-Begrenzung]
[picture:828:a_fm_modulator_hub2:Begrenzung des Signals]
</margin>

[question:AD509]