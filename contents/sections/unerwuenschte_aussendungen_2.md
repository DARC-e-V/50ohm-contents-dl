In der Klasse N haben wir bereits unerwünschte Aussendungen kennengelernt. Solche Aussendungen sollten unbedingt vermieden werden, was durch verschiedene technische Maßnahmen erreicht werden kann – auf diese gehen wir in dieser Lektion näher ein. Unerwünschte Aussendungen entstehen bei Funksendern häufig durch *Oberwellen*, also ganzzahlige Vielfache der Grundfrequenz, sowie durch sogenannte *Nebenaussendungen*, wie in der Abbildung [ref:e_unerwuenschte_aussendungen_uebersicht] gezeigt. Zunächst befassen wir uns mit den Oberwellen, da sie andere Funkdienste beeinträchtigen oder stören können. Von einer Störung spricht man, wenn eine Amateurfunkstation unerwünschte Frequenzanteile so stark abstrahlt, dass die zulässigen Grenzwerte überschritten werden. Ein typisches Beispiel ist die Aussendung einer Oberschwingung eines Transceivers im UKW-Rundfunkbereich, wie in Abbildung [ref:e_unerwuenschte_aussendungen_oberwelle] dargestellt. Hierbei führt die vierfache Frequenz ($\qty{145,9}{\mega\hertz}\cdot 4 = \qty{583,6}{\mega\hertz}$) der Grundfrequenz zu einer Störung. Die Nebenaussendungen betrachten wir am Ende dieser Lektion.

<margin>
[picture:1008:e_unerwuenschte_aussendungen_uebersicht:Unerwünschte Aussendungen: Oberwellen (OW) und Nebenaussendungen (NA)]
</margin>

<margin>
[picture:745:e_unerwuenschte_aussendungen_oberwelle:Störung des DVB-T2-Empfang eines Fernsehers durch die Oberwelle einer Amateurfunkaussendung]
</margin>

---

Die Messung unerwünschter Aussendungen eines Senders erfolgt – im Gegensatz zur PEP-Messung – immer am Senderausgang unter Einbeziehung des gegebenenfalls verwendeten SWR-Meters, zusätzlicher Anpassgeräte und eventuell eingesetzter Tiefpassfilter (vgl. Abbildung [ref:e_unerwuenschte_aussendungen_trx]).
Hierdurch wird sichergestellt, dass nur die unerwünschten Aussendungen gemessen werden, die auch die Antenne erreichen können. Als Messgerät eignet sich hierfür am besten ein Spektrumanalysator. Wie genau eine solche Überprüfung durchgeführt wird, wie das Frequenzspektrum von Oberwellen aussieht und welche gesetzlichen Vorgaben dabei gelten, werden wir erst in der Klasse A näher betrachten.

<margin>
[picture:917:e_unerwuenschte_aussendungen_trx:Messung von unerwünschten Aussendungen]
</margin>

[question:EJ209]

Ein ideales Sendesignal, welches nur auf einer gewünschten Frequenz aussendet sollte ein idealer Sinus sein. Dieser enthält ausser der Grundfrequenz keine weiteren Frequenzanteile.

[question:EJ201]

<indepth>
Signalformen, welche nicht sinusförmig sind und insbesondere scharfe "Ecken und Kanten" enthalten, bestehen aus vielen verschiedenen Sinus-Frequenzanteilen und enthalten viele Oberwellenanteile. Insbesondere wenn Sender übersteuert werden, werden zuvor sinusförmige Signale oft verzerrt bzw. in deren Amplitude beschnitten. Hierdurch entstehen auch massive Oberwellenanteile. Jede Abweichung von der idealen Sinus-Form ist daher bei idealen Sendesignalen zu vermeiden. Diese Thematik werden wir in der Klasse A noch genauer betrachten. Mit diesem Applet lässt sich der Sachverhalt jedoch bereits ausprobieren.
[include:fourier]
</indepth>

---

Zur Unterdrückung von Oberwellen werden im Kurzwellenbereich üblicherweise *Oberwellenfilter* eingesetzt. Ihre Charakteristik ist so ausgelegt, dass Frequenzen unterhalb einer bestimmten Grenzfrequenz das Filter nahezu ungedämpft passieren, während Frequenzen oberhalb dieser Grenze nicht oder nur stark abgeschwächt durchgelassen werden. Ein *Oberwellenfilter* ist somit ein *Tiefpassfilter*, wie wir es bereits im Kapitel Schwingkreise kennengelernt haben. Der Frequenzgang eines solchen Tiefpasses ist in Abbildung [ref:e_ua_tiefpass] dargestellt. Abbildung [ref:e_ua_tiefpass_selbstbau] zeigt ein selbstgebautes Tiefpassfilter bestehend aus Kondensatoren und Spulen welche auf Ringkerne gewickelt wurden. Schaltet man bei einem Mehrbandsender das Band um, wird dabei in der Regel auch ein passendes Oberwellenfilter ausgewählt. Oft ist dann das Klicken eines Relais zu hören, das diese Umschaltung vornimmt.

Dass dieses Thema sehr wichtig ist, zeigt sich an der großen Zahl von Prüfungsfragen dazu. Mit dem Wissen über Oberwellen und Tiefpässe lassen sich diese jedoch sehr leicht beantworten.

<margin>
[picture:591:e_ua_tiefpass:Frequenzgang eines Tiefpassfilters]
</margin>

<margin>
[photo:320:e_ua_tiefpass_selbstbau:Selbgebautes Tiefpassfilters]
</margin>

---

[question:EJ202]
[question:EJ204]
[question:EJ205]
[question:EJ206]
[question:EJ207]
[question:EJ208]
[question:EJ203]

<indepth>
[picture:593:bandpass:Frequenzgang eines Bandpassfilters]
  
Eine weitere Möglichkeit Oberwellen zu unterdrücken stellt der Einsatz eines Bandpassfilters dar. Bandpassfilter werden häufig bei Einbandsendern sowie bei Sendern für den VHF/UHF/SHF-Bereich verwendet. Hierbei müssen oft auch Signalanteile, welche innerhalb der Aufbereitung des Sendesignals entstehen, und sich auch unterhalb der Sendefrequenz befinden können, unterdrückt werden.
</indepth>

Wie schon zuvor erwähnt sind sinusförmige Signale für die Vermeidung von Oberwellenanteilen essentiell. Dies wird unter anderem dadurch erreicht, dass die Senderstufen, insbesondere die Leistungsendstufen eines Senders verzerrungsfrei arbeiten. Erfolgt eine Neueinstellung des Arbeitspunktes einer Sender-Endstufe ist im Anschluss auf jeden Fall auf deren Linearität und die Qualität der Aussendung auf Oberwellenarmut zu prüfen.

[question:EF404]

Unerwünschte Aussendungen können auch in unmittelbarer Nähe zum eigentlichen Sendesignal auftreten (vgl. Abbildung [ref:e_unerwuenschte_aussendungen_uebersicht]) und betreffen damit oft andere Funkamateure auf demselben Band. Solche Störungen lassen sich mit Filtern nur schwer oder gar nicht unterdrücken und sollten daher bereits am Anfang der Signalaufbereitung durch geeignete Maßnahmen vermieden werden. Häufig entstehen diese *Nebenaussendungen* – auch Nebenprodukte genannt und umgangssprachlich als „Splatter“ bezeichnet – durch eine zu hohe Einstellung des Mikrofonverstärkers im Sender, wodurch sich das Sendesignal ungewollt verbreitert.

[question:EJ213]
[question:EJ214]

Das Gleiche gilt auch für digitale Übertragungsverfahren, wie zum Beispiel Packet Radio. Um Nebenaussendungen und Überschreitungen der zulässigen Bandbreite zu vermeiden, kann insbesondere bei AFSK-modulierten FM-Sendern entweder der Hub begrenzt oder die NF-Aussteuerung reduziert werden.

[question:EJ212]

Auch die Stabilität des im Sender verwendeten Oszillators kann dazu führen, dass Aussendungen außerhalb der Bandgrenzen liegen oder benachbarte Stationen gestört werden. Besonders bei älteren Selbstbaugeräten ohne quarzstabilisierte Oszillatoren ist dies möglich. Moderne Kurzwellentransceiver, aber auch aktuelle Selbstbaugeräte und Bausätze, verfügen in der Regel über sehr stabile Referenzoszillatoren.

[question:EJ216]