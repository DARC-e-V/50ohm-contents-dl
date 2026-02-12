<margin>
[picture:1019:e_frequenzabhängiger_widerstand:Frequenzabhängikeit von Kondensator und Spule im Vergleich zu einem klassischen Widerstand]
[picture:1020:e_herleitung_tiefpass:Herleitung der Tiefpassschaltung ausgehend von einem Spannungsteiler]
</margin>

In den Kapiteln zu Kondensatoren und Spulen haben wir bereits gelernt, dass beide Bauelemente einen frequenzabhängigen Widerstand besitzen. Abbildung [ref:e_frequenzabhängiger_widerstand] zeigt qualitativ, dass der Widerstand eines ohmschen Widerstands unabhängig von der Frequenz ist, während der Widerstand eines Kondensators mit steigender Frequenz hyperbolisch abnimmt und der Widerstand einer Spule mit steigender Frequenz linear zunimmt.

Aus diesen Bauelementen lassen sich sogenannte passive Frequenzfilter aufbauen, die wir uns nun genauer ansehen. Im ersten Teil dieses Kapitels beschäftigen wir uns mit einfachen Filtern, nämlich Hoch- und Tiefpässen. Mit diesen Filtern lassen sich unerwünschte Frequenzbereiche ober- oder unterhalb einer Grenzfrequenz unterdrücken. Im zweiten Teil widmen wir uns anschließend komplexeren Filtern, wie zum Beispiel Bandpässen.

Wir beginnen mit der Herleitung eines Tiefpasses als sogennantes *RC-Glied*. Ausgangspunkt ist im Schritt (1) die Schaltung eines Spannungsteilers, wie sie in Abbildung [ref:e_herleitung_tiefpass] dargestellt ist und die wir bereits kennengelernt haben. Wir erinnern uns daran, dass für einen Spannungsteiler folgendes gilt: 

$ \frac{U_1}{U_2} = \frac{R_1}{R_2} $.

Das bedeutet beispielsweise: Ist der Widerstand $R_2$ doppelt so groß wie der Widerstand $R_1$, dann ist auch die Spannung $U_2$ doppelt so groß wie die Spannung $U_1$.

In Schritt (2) ersetzen wir den Widerstand $R_2$ durch den Kondensator $C_1$. Anschließend zeichnen wir die Schaltung in Schritt (3) noch etwas um, sodass wir die übliche Darstellung eines Tiefpasses erhalten.

---

Wir halten fest: Ein Tiefpass ist zunächst nichts anderes als ein Spannungsteiler. Deshalb können wir ihn im Folgenden auch genau so betrachten. In Abbildung [ref:e_wiederstaende_tiefpass] sind die Widerstandsverläufe in Abhängigkeit von der Frequenz nochmals dargestellt. Betrachten wir zunächst tiefe Frequenzen: In diesem Fall ist der Widerstand des Kondensators groß, sodass am Ausgang eine hohe Spannung anliegt. Steigt die Frequenz, wird der Widerstand des Kondensators zunehmend kleiner, und gemäß dem Prinzip des Spannungsteilers nimmt auch die Ausgangsspannung ab.

Auf diese Weise ergibt sich der Spannungsverlauf, wie er in Abbildung [ref:e_tiefpass_frequenzgang] gezeigt ist. Damit ist auch die Kernidee des Tiefpasses erklärt: Hohe Frequenzen werden stark gedämpft, während tiefe Frequenzen das Filter weitgehend ungehindert passieren. Ein Anwendungsbeispiel für einen Tiefpass ist die Verwendung hinter Sendeverstärkern, um die durch Verzerrungen auftretenden Oberwellen herauszufiltern. 

<margin>
[picture:1021:e_wiederstaende_tiefpass:Qualitatives Widerstandsverhalten im Tiefpass-Spannungsteiler]
[picture:1024:e_tiefpass_frequenzgang:Qualitativer Spannungsverlauf $U_A$ am Tiefpass]
</margin>

[question:ED208]
[question:ED201]

<indepth>
Die *Grenzfrequenz* ($f_g$) eines Tiefpasses ist die Frequenz, bei der das Ausgangssignal gerade beginnt, merklich abgeschwächt zu werden. Sie markiert also den Übergang zwischen dem Frequenzbereich, der vom Filter weitgehend ungehindert durchgelassen wird, und dem Bereich, in dem die Dämpfung deutlich zunimmt. Formal ist die Grenzfrequenz so definiert, dass bei ihr die Ausgangsleistung auf die Hälfte der Eingangsleistung abgefallen ist (-3 dB). Da die Leistung proportional zum Quadrat der Spannung ist, entspricht dies einer Abnahme der Ausgangsspannung auf etwa 70 % ihres ursprünglichen Wertes ($\frac{1}{\sqrt{2}}$). In der Praxis erkennt man die Grenzfrequenz daher oft an dem Punkt, an dem die Ausgangsspannung deutlich kleiner wird und der Frequenzgang „abzuknicken“ beginnt. Unterhalb der Grenzfrequenz werden tiefe Frequenzen nahezu unverändert übertragen, oberhalb der Grenzfrequenz werden höhere Frequenzen zunehmend gedämpft.
</indepth>

---

Bei einem Hochpass hingegen werden die tiefen Frequenzen stark gedämpft, während die hohen Frequenzen dieses Filter kaum gedämpft passieren. Dies erreicht man, in dem man Kondensator und Widerstand tauscht wie in Abbildung [ref:e_wiederstaende_hochpass] dargestellt. Der Frequenzgang eines Hochpasses ist qualitativ in [ref:e_hochpass_frequenzgang] gezeigt. Ein Anwendungsbeispiel für einen Hochpass ist die Verwendung in einer Antennenweiche, um z.B. den Kurzwellenbereich vor einem UKW-Empfänger wegzufiltern, um Störungen durch Kurzwellenbetrieb zu vermeiden.

<margin>
[picture:1025:e_wiederstaende_hochpass:Qualitatives Widerstandsverhalten im Hochpass-Spannungsteiler]
[picture:1022:e_hochpass_frequenzgang:Qualitativer Spannungsverlauf $U_A$ am Hochpass]
</margin>

[question:ED211]
[question:ED202]

---

Einfache RC-Glieder haben den Nachteil, dass ihre Flanken im Grenzbereich eher flach verlaufen. Dazu wird die kleinste Impedanz eines RC-Tiefpasses durch den Widerstand $R$ bestimmt. Der Widerstand $R$ lässt sich jedoch durch eine Spule ersetzen, die sich im Frequenzverhalten einem Kondensator entgegengesetzt verhält. Es liegt daher nahe, Spulen und Kondensatoren zu Hoch- und Tiefpässen zu kombinieren. 
Bei *hohen Frequenzen ist der Spulenwiderstand hoch*, der Kondensatorwiderstand dagegen klein.
Bei *niedrigen Frequenzen ist der Spulenwiderstand niedrig*, der Kondensatorwiderstand dagegen groß. 
Je nachdem, über welches Bauteil die Ausgangsspannung gemessen wird, erhält man einen Hoch- oder einen Tiefpass. Merkt man sich, dass der Spulenwiderstand $X_L$ bei hoher Frequenz ebenfalls hoch ist, lässt sich eine Schaltung schnell als Hoch- oder Tiefpass identifizieren, wenn man sich anschaut, über welches Bauteil die Ausgangsspannung gemessen wird.

<tip>
Auch bei Schaltungen mit Kondensator und Spule gilt folgende einfache Regel: Handelt es sich im oberen Zweig des Spannungsteilers um ein aufrechtes *H* – wie in *H*ochpass, so liegt ein Hochpass vor. Befindet sich im oberen Zweig hingegen ein Widerstand oder eine Spule, handelt es sich um einen Tiefpass.
[picture:1023:e_hochpass_tipp:Tipp zum Merken]
</tip>

[question:ED209]
[question:ED212]

---

In den folgenden Fragen geht es um eine praktische Anwendung unserer Filter. Natürlich können auch mehrere frequenzabhängige Bauteile in einer Schaltung verwendet werden, so dass der Übergang im Bereich der Grenzfrequenz steilflankiger wird. Welche Schaltung in den Folgenden zwei Fragen verwendet werden, solltest Du mit dem genannten Tipp nun leicht erkennen. 

[question:ED210]
[question:ED213] 

Ein weiteres Praxisbeispiel für eine Verkettung von Spulen und Kondensatoren als Filter, ist der am Rand erklärte Diplexer. 

<indepth>
*Praxisbeispiel Diplexer:* Passive Hoch- und Tiefpässe werden auch in Frequenzweichen verwendet. Im untenstehenden Beispiel ist eine Schaltung für einen sog. Diplexer für 2m und 70cm zu sehen. Dieser kann verwendet werden, um z.B. ein 2m- und ein 70cm-Funkgerät an einer gemeinsamen Duoband-Antenne zu verwenden. Umgekehrt könnte man auch getrennte Antennen für 2m und 70cm an einem UKW-Duoband-Gerät verwenden, um z.B. für 2m-Direktfunk einen Rundstrahler und für 70cm-Relaisfunk eine Richtantenne zu verwenden. 
Vor dem 2m-Ausgang ist ein Tiefpass, vor dem 70cm-Ausgang ein Hochpass zu sehen - jeweils aus 5 frequenzabhängigen Bauteilen kombiniert. 
[picture:939:e_circuit_diplexer:Schaltbild 2m-/70cm-Diplexer]
[photo:171:e_example_diplexer:Aufbaubeispiel]
</indepth>

<indepth>
[photo:320:e_tiefpass_selbstbau:Selbstgebautes Tiefpassfilter]
Die oben genannten Filter lassen sich natürlich wunderbar für alle Frequenzbereiche selbst berechnen und bauen. In der Formelsammlung finden sich die benötigten Formeln, wobei es natürlich auch viele Bauvorschläge und Berechnungsprogramme gibt. Die benötigten Spulen lassen sich dazu oft leicht selbst herstellen. Hierfür reicht bei kleinen Spulenwerten ein kleiner Vorrat an 0.8mm-Kupferlackdraht für stabile Luftspulen aus. Bei großen Spulenwerten z.B. für die Kurzwellenbereiche kommt man mit 0.2mm-Kupferlackdraht und Kernmaterial mit entsprechenden AL-Werten aus, um sich jederzeit die richtigen Werte selbst herstellen zu können. Die benötigten Größen, Wicklungen usw. bekommt man über Formelsammlung, Bauvorschläge oder Berechnungsprogramme ebenfalls meist leicht heraus.
</indepth>  

---

Nun haben wir einfache RC- und LC-Glieder als Hoch- und Tiefpassfilter kennengelernt. Aus Kondensatoren und Spulen lassen sich jedoch noch weitere Filtertypen realisieren, die über reine Hoch- und Tiefpässe hinausgehen. Diese wollen wir uns nun im zweiten Teil genauer ansehen, nämlich die sogenannten *Schwingkreise*.

<margin>
[picture:1026:e_rp_schwinkreis:(a) Reihen- (b) Parallelschwinkreis]
</margin>

Mithilfe von Schwingkreisen lassen sich Spule und Kondensator – je nach gewünschter Filterwirkung – so anordnen, dass bei einer bestimmten Frequenz ein besonders hoher oder besonders niedriger Widerstand auftritt. Dadurch werden Frequenzen oberhalb oder unterhalb dieser Frequenz gezielt gedämpft oder durchgelassen.

Die Anordnung von Spule und Kondensator kann dabei entweder in Serie oder parallel erfolgen. Man unterscheidet entsprechend Reihenschwingkreise (a) und Parallelschwingkreise (b), wie in Abbildung [ref:e_rp_schwinkreis] dargestellt. 

---

Schaltet man Spule und Kondensator parallel und gibt zum Beispiel einen Rechteckimpuls auf diese Anordnung, gerät diese in Schwingung. Der aufgeladene Kondensator hat nun Energie im elektrischen Feld gespeichert, welches sich jedoch über die Spule abbaut. Durch den Stromfluss durch die Spule baut sich ein magnetisches Feld in ihr auf, was dem Stromfluss erst noch einen Widerstand entgegensetzt. Sobald das Magnetfeld jedoch aufgebaut ist, entlädt sich der Kondensator vollständig. Die Energie ist nun im Magnetfeld der Spule gespeichert. Da der Kondensator sich aber nicht weiter entladen und keinen Stromfluss aufrechterhalten kann, kann das Magnetfeld nicht aufrechterhalten werden. Das Magnetfeld der Spule entlädt sich und erzeugt eine Spannung in umgekehrter Richtung. Diese Spannung lädt den Kondensator nun in umgehrter Richtung auf, bis das Magnetfeld in der Spule abgebaut ist und dem elektrischen Feld im Kondensator keinen Widerstand mehr entgegensetzen kann. Der Vorgang beginnt anschließend erneut. 

<margin>
[include:applet_schwingkreis]
</margin>

---

Aus diesem Grund spricht man von einem Schwingkreis. Die Frequenz, mit der dieser Schwingkreis schwingt, bezeichnet man als Resonanzfrequenz ($f_o$). Sie ist vergleichbar mit der Resonanzfrequenz einer Stimmgabel, die durch einen Stoß in Schwingung versetzt wird. Im Resonanzfall sind die Widerstände von Spule $X_L$ und Kondensator $X_C$ gleich groß. Solche Schwingkreise lassen sich zum einen zur Erzeugung von Schwingungen verwenden, was wir im Kapitel Oszillatoren noch genauer betrachten werden. Zum anderen können sie auch als Filter eingesetzt werden – und genau das ist das Thema dieses Kapitels.

<margin>
[picture:1037:e_rsk_frequenzgang:Qualitativer Frequenzgang eines Reihenschwinkreises]
</margin>

---

Bei einem *Serienschwingkreis* bzw. *Reihenschwingkreis* wie in Abbildung [ref:e_rp_schwinkreis]a ist im Resonanzfall der Gesamtwiderstand am geringsten. Abbildung [ref:e_rsk_frequenzgang] zeigt den Frequenzgang. Bei Frequenzen über der Resonanzfrequenz wird der Spulenwiderstand größer, so dass auch der Gesamtwiderstand des Serienschwingkreises ansteigt. Das Gleiche passiert auch bei Frequenzen unterhalb der Resonanzfrequenz, wobei hier jedoch der Kondensatorwiderstand groß ist. Bei Serienschwingkreisen ist daher der Widerstand bei der Resonanzfrequenz am geringsten. Durch die Serienschaltung bestimmt bei Frequenzen abseits der Resonanzfrequenz das Bauteil mit dem größten Widerstand die Schwingkreisimpedanz.

<indepth>
Der Betragsfrequenzgang eines Serienschwinkreises aus einem Widerstand, einer Spule und einem Kondensator berechnet sich nach folgender Formel:
  
$Z = \sqrt{R^2+\left(X_L - X_C\right)^2}$
  
Im Resonanzfall wenn $X_C$ = $X_L$ gilt bleibt nur der Widerstand $R$ übrig. Im Idealen Fall, wenn der Widerstand $R=0$ ist ist der Widerstand sogar null. Wenn wir die Werte für $X_L$ und $X_C$ einsetzen erhalten wir:
  
$Z = \sqrt{R^2+\left(2\pi f \cdot L~-~\frac{1}{2\pi f \cdot C} \right)^2}$
  
In der Formel kann man den Frequenzgang aus Abbildung [ref:e_rsk_frequenzgang] sehr schön sehen: Wenn man die Frequenz gegen 0 gehen lässt, dann fällt der Anteil der Spule weg und nur der Kondensator wirkt. Lässt man die Frequenz hingegen gegen unendlich gehen, dann wirkt nur die Spule und der Anteil des Kondensators verschwindet.
  
Man kann die Resonanzfrequenz sogar berechnen. Wenn $X_L$ = $X_C$ gilt kann man die Formel nach $f$ auflösen:
  
$2\pi f \cdot L = \frac{1}{2\pi f \cdot C}$
  
So ergibt sich die Formel: 
  
$ f_0 = \frac{1}{2\pi \sqrt{L\cdot C}} $
  
Die genaue Herleitung der Formeln kann man z. B. auf [Wikipedia](https://de.wikipedia.org/wiki/Schwingkreis) nachlesen. Es sollte an dieser Stelle erwähnt werden, dass alle Frequenzgänge qualitativ aufgezeichnet sind und in der Realität ggf. etwas anders aussehen.
</indepth>

[question:ED206] 
[question:ED207]

---

Setzt man Kondensator und Spule zu einem *Parallelschwingkreis*, wie in Abbildung [ref:e_rp_schwinkreis]b zusammen, verhält es sich dagegen genau andersherum: Der Widerstand *Z* ist bei der Resonanzfrequenz der sehr hoch, vgl. Abbildung [ref:e_psk_frequenzgang]. Bei Frequenzen über der Resonanzfrequenz hat der Kondensator jedoch einen niedrigen Widerstand, so dass der Widerstand dieses Schwingkreises abnimmt. Bei Frequenzen unter der Resonanzfrequenz hat dagegen die Spule einen niedrigen Widerstand, so dass auch bei niedrigeren Frequenzen der Widerstand des Schwingkreises abnimmt. 
Bei Parallelschwingkreisen ist daher der Widerstand bei der Resonanzfrequenz am höchsten. Bei Frequenzen abseits der Resonanzfrequenz bestimmt das Bauteil mit dem geringeren Widerstand die Impedanz des Parallelschwingkreises. 

<margin>
[picture:1036:e_psk_frequenzgang:Qualitativer Frequenzgang eines Parallelschingkreises]
</margin>

[question:ED205]

% TODO ////

Je nachdem, wie Parallel- und Serienschwingkreise im Signalweg eingesetzt werden, lassen sich nun Frequenzbereiche entweder bedämpfen oder herausfiltern. Hierzu wollen wir wieder unseren Spannungsteileransatz nutzen.

---

Beginnen wir zunächst mit den Schaltungen für *Bandsperren*. Dabei gibt es zwei Möglichkeiten, diese als Spannungsteiler aufzubauen: erstens den *Saugkreis* (vgl. Abbildung [ref:e_saugkreis]) und zweitens den *Sperrkreis* (vgl. Abbildung [ref:e_sperrkreis]). In den Abbildungen sind jeweils der frequenzabhängige Widerstand sowie die Ausgangsspannung dargestellt. Mithilfe unserer bekannten Regeln zum Spannungsteiler lassen sich diese Zusammenhänge ganz analog zu den zuvor behandelten RC-Gliedern herleiten und verstehen. Weil die Parallelschwingkreise in Resonanz einen hohen Widerstand haben, lassen sich diese gut als Sperrkreis seriell im Signalweg verwenden. Oder man verwendet den geringen Resonanzwiderstand eines Serienschwingkreises parallel zum Signalweg als Saugkreis. Oft wird aber auch hier beides in Kombination verwendet. 
[question:ED204]. Eine Anwendung für Bandsperren ist z.B. die Unterdrückung einzelner Bandbereiche, zum Beispiel wenn ein naheliegender UKW-Radiosender den Empfang stört.

[question:ED215]

<margin>
[picture:1038:e_saugkreis:Qualitative Frequenzgänge eines Saugkreises]
[picture:1040:e_sperrkreis:Qualitative Frequenzgänge eines Sperrkreises]
</margin>

---

Die zweite Kategorie an Schaltungen die man aus Schwinkreisen entwickeln kann sind *Bandpässe*. Hier gibt es auch wieder zwei Möglichkeiten diese als Spannungsteiler aufzubauen: erstens den *Leitkreis* (vgl. Abbildung [ref:e_leitkreis]) und zweitens den *Bandpass* (vgl. Abbildung [ref:e_bandpass]). Auch hier erfolgt die Herleitung wie gewohnt über das Verhalten eines Spannungsteilers. Für einen Bandpass setzt man Parallelschwingkreise parallel zum Signalweg, da diese für Frequenzen abseits der Resonanz einen geringen Widerstand haben und diese sozusagen "kurzschließen". Ein Serienschwingkreis seriell im Signalweg sorgt für eine zusätzliche Dämpfung abseits der Resonanz, während dieser bei der gewünschten Frequenz einen geringen Widerstand hat.

[question:ED214] 
[question:ED204]
[question:ED203]


<margin>
[picture:1039:e_leitkreis:Qualitative Frequenzgänge eines Leitkreises]
[picture:1042:e_bandpass:Qualitative Frequenzgänge eines Bandpasses]
</margin>

Ein naheliegendes Anwendungsbeispiel für Bandpässe ist ihr Einsatz in Empfängern, bei denen eine Vorfilterung bestimmter Frequenzbänder erforderlich ist. In diesem Fall wird ein Filter verwendet, das nur ein gewünschtes Frequenzband passieren lässt, während alle anderen Frequenzen gedämpft werden. Solche Bandpässe finden sich daher in nahezu jedem Empfänger, oft sogar separat für jedes einzelne Kurzwellenband. Für entsprechend hohe Leistungen ausgelegt, werden Bandpässe auch im Sendebetrieb eingesetzt, etwa bei gemeinsamen Contesten oder Fielddays, um gegenseitige Störungen zwischen benachbarten Stationen zu minimieren.

Um Bandpässe und Bandsperren zu bauen, können also sowohl Serien- als auch Parallelschwingkreise verwendet werden. Entscheidend ist, dabei zu beachten, wie sich die jeweiligen Schwingkreise im Resonanzfall verhalten. Entsprechend ihres Verhaltens können diese seriell im oder parallel am Signalweg angebracht sein - ggf. sogar mehrfach miteinander kombiniert. 

In Filtern lassen sich als Kondensatoren nur bestimmte, geeignete Typen verwenden.
Elektrolytkondensatoren eignen sich für HF-Schaltungen zum Beispiel nicht, da ihre Kapazität zum einen stark frequenzabhängig ist, zum anderen weil sie bei hohen Frequenzen einen hohen Innenwiderstand haben. Folienkondensatoren eignen sich dagegen nicht, weil diese durch ihre Wicklungen (Eigeninduktivität) besonders ab dem Kurzwellenbereich stark frequenzabhängig sind und eine schlechte Güte haben. 
Keramikkondensatoren haben dagegen nur kleine Verluste und die Kapazität ist nur wenig frequenz- und temperaturabhängig. Zudem sind diese auch für große Spannungen leicht zu beschaffen.
Geeignet sind auch Kondensatoren aus Platten und Luft als Isolator, die man am ehesten als Drehkondensatoren antrifft. Für hohe Spannungen werden Drehkondensatoren in Antennentunern ebenfalls eingesetzt.

[question:ED216]