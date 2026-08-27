In der Klasse E haben wir bereits unerwünschte Aussendungen in Form von *Oberwellen* und *Nebenaussendungen* kennengelernt. Oberwellen bzw. Harmonische eines Signals entstehen immer, wenn sich Abweichungen von der idealen Sinus-Kurve bilden und sind immer ganzzahlige Vielfache der Grundfrequenz, wie in Abbildung [ref:a_harmonische] dargestellt.

Ein Beispiel zeigt die folgende Prüfungsfrage: Wird ein Verstärker übersteuert, werden die Spitzen der Amplitude des Sinussignals begrenzt – dadurch entstehen Oberwellen.

[question:AJ207]

<margin>
[picture:868:a_harmonische: Oberwellen (OW), Harmonische (Harm.) und Nebenaussendungen (NA)]
</margin>

---

Bei der Betrachtung von Vielfachen der Grundfrequenz eines Signals unterscheiden wir zwischen den Begriffen *Harmonische und Oberwellen* des Signals. Diese beiden Begriffe unterscheiden sich nur in deren Definition und Zählweise. Die 1. Harmonische eines Signals ist dessen Grundfrequenz selbst. Die 2. Harmonische entspricht der 1. Oberwelle eines Signals, die 3. Harmonische der 2. Oberwelle eines Signals und so weiter. Die nebenstehende Tabelle [ref:a_harmonische] zeigt den Zusammenhang. 

<margin>
| l: Vielfaches der Grundfrequenz | l: Harmonische | l: Oberwelle |
| $f_0$ | 1 | ~ |
| $2 \cdot f_0$ | 2 | 1 |
| $3 \cdot f_0$ | 3 | 2 |
| $4 \cdot f_0$ | 4 | 3 |
[table:a_harmonische:Harmonische und Oberwellen]
</margin>

---
  
[question:AJ203]
[question:AJ204]

<tip>
Der UKW-Rundfunk ist der "klassische" Rundfunk auf Ultrakurzwelle (UKW). Die Ausstrahlung von Radioprogrammen erfolgt im Frequenzbereich von $\qtyrange{87,6}{107,9}{\mega\hertz}$.
</tip>

Sollen bestimmte Oberwellen oder Harmonische eines Signals einzeln unterdrückt werden, so kann dies neben des klassischen Oberwellenfilters (Tiefpass) auch durch sog. *Sperrkreise* erfolgen. Ein Sperrkreis unterdrückt genau eine Frequenz maximal und lässt ansonsten alle anderen nahezu ungehindert passieren.

[question:AJ210]

---

Nach der Amateurfunkverordnung (AFuV) sind unerwünschte Aussendungen auf das geringstmögliche Maß zu beschränken. Für selbst gebaute Amateurfunkgeräte sowie für ursprünglich kommerziell vertriebene Geräte, die von einem Funkamateur verändert wurden, legt die [Verfügung 33/2007](https://50ohm.de/vfg33) der Bundesnetzagentur (BNetzA) konkrete Grenzwerte fest. Die Abbildung [ref:a_vfg33] zeigt einen Auszug aus dieser Verfügung mit den zulässigen Grenzwerten für unerwünschte Aussendungen. 

Die Grenzwerte sind üblicherweise in $\unit{\dBc}$ angegeben und beschreiben, um wie viele Dezibel eine unerwünschte Aussendung gegenüber dem Trägersignal beziehungsweise dem maximalen Sendesignalpegel des Senders (PEP) abgeschwächt sein muss. Alternativ zur relativen Angabe in $\unit{\dBc}$ kann für unerwünschte Aussendungen auch ein absoluter Grenzwert der Leistung, beispielsweise in $\unit{\dBm}$ oder $\unit{\micro\watt}$, gelten. Maßgeblich ist dabei jeweils der höhere der aus beiden Grenzwerten resultierenden zulässigen Leistungswerte.

Für Amateurfunkgeräte, die kommerziell in der Europäischen Union vertrieben werden, gelten ebenfalls Grenzwerte für unerwünschte Aussendungen. Diese sind EU-weit einheitlich geregelt. Im Unterschied zu den Grenzwerten der Verfügung 33/2007 hängen die zulässigen Werte hierbei teilweise von der Sendeleistung des Geräts ab. Die Abbildung [ref:a_etsi_vfg] stellt die Grenzwerte für kommerziell vertriebene Geräte den Vorgaben der Verfügung 33/2007 gegenüber.

Ein Beispiel verdeutlicht den Unterschied: Für ein kommerziell vertriebenes Handfunkgerät mit einer Sendeleistung von $\qty{5}{\watt}$ gilt im dargestellten Frequenzbereich ein Grenzwert von $\qty{-50}{\dBc}$. Wird dagegen ein entsprechendes $\qty{5}{\watt}$-Gerät für das 2-m- oder 70-cm-Band selbst gebaut, muss nach Verfügung 33/2007 ein Grenzwert von $\qty{-60}{\dBc}$ eingehalten werden.

Bei einer Sendeleistung von $\qty{750}{\watt}$ bleibt dieser Grenzwert für das selbst gebaute Gerät bei $\qty{-60}{\dBc}$. Für ein kommerziell vertriebenes Gerät mit derselben Leistung gilt dagegen ein strengerer Grenzwert von $\qty{-70}{\dBc}$.

Die folgenden Prüfungsfragen beziehen sich auf selbst gebaute oder modifizierte Amateurfunkgeräte und somit auf die Grenzwerte für unerwünschte Aussendungen, wie sie in der Verfügung 33/2007 der Bundesnetzagentur festgelegt sind.

<margin>
[photo:319:a_vfg33:Auszug aus der Verfügung 33 von 2007.]
[picture:1139:a_etsi_vfg:Vergleich der ETSI Norm EN 301783 mit der Verfügung 33 von 2007. Im Hintergrund sind die Amateurfunkbänder grau hinterlegt.]
</margin>

---

Für den VHF/UHF/SHF-Bereich von $\qtyrange{50}{1000}{\mega\hertz}$ gilt, dass Nebenaussendungen und Oberwellen mindestens $\qty{60}{\dB}$ gegenüber dem maximalen Sendesignalspitzenpegel des Senders (PEP) gedämpft werden müssen, so lange sich die Leistung der Signale oberhalb eines Pegels von $\qty{0,25}{\micro\watt}$ befindet (vgl. Abbildung [ref:a_uagw]). 

<margin>
[picture:918:a_uagw:Oberwellendämpfung VHF/UHF/SHF-Bereich]
</margin>

[question:AJ225]

---

Für den Kurzwellenbereich von $\qtyrange{1,7}{35}{\mega\hertz}$ gilt, dass Nebenaussendungen und Oberwellen mindestens $\qty{40}{\dB}$ gegenüber dem maximalen Sendesignalspitzenpegel des Senders (PEP) gedämpft werden müssen, so lange sich die Leistung der Signale oberhalb eines Pegels von $\qty{0,25}{\micro\watt}$ befindet (vgl. Abbildung [ref:a_uagw2]).

<margin>
[picture:1140:a_uagw2:Oberwellendämpfung KW-Bereich]
</margin>

[question:AJ224]

%TODO BILD VON DL1COM EINBAUEN
Mit einem Spektrumanalysator lässt sich im Modus *Spurious Emissions* eine Messung der Oberwellen bzw. Harmonischen (engl. harmonics) durchführen, wie in Abbildung [ref:a_uagw] dargestellt. Der Spektrumanalysator erfasst dabei automatisch den Pegel des Trägers sowie die Unterdrückung der Harmonischen und zeigt diese zusätzlich auf dem Bildschirm an. Wenn man ein Gerät selbst baut, ist es entscheidend, durch Messungen sicherzustellen, dass die vorgeschriebenen Grenzwerte eingehalten werden. Ein kommerzieller Funkgerätehersteller bestätigt mit der CE-Erklärung zwar die Einhaltung dieser Grenzwerte, dennoch kommt es vor, dass einzelne Geräte die Vorgaben nicht erfüllen – in solchen Fällen kann die Bundesnetzagentur deren Betrieb und Verkauf verbieten.

Unerwünschte Aussendungen entstehen nicht nur durch Oberwellen, sondern können auch in der Frequenzaufbereitung von Sendern auftreten – etwa durch unerwünschte Mischprodukte, durch Schwankungen in der Versorgungsspannung oder durch eine Übersteuerung des NF-Signals. Das wollen wir uns im Folgenden noch etwas genauer anschauen. 

Zur Unterdrückung von unerwünschten Mischprodukten – aber auch der Oberwellen – wird nach Mischern häufig ein Bandpassfilter eingesetzt. Besonders bei Einbandsendern sowie bei Geräten für den VHF-, UHF- und SHF-Bereich kommen statt klassischer Oberwellen-Tiefpässe nämlich Bandpässe zum Einsatz. Bei diesen Funkgeräten müssen oft auch Signalanteile unterdrückt werden, die bereits innerhalb der Aufbereitung des Sendesignals entstehen und sich sogar unterhalb der eigentlichen Sendefrequenz befinden können.

[question:AJ211]
[question:AJ209]
[question:AJ208]

Unerwünschte Aussendungen können auch in unmittelbarer Nähe zum Sendesignal vorliegen. Diese sind durch den Einsatz von Filtern nur schwer oder gar nicht zu unterdrücken und sollten daher bereits zu Beginn der Signalaufbereitung durch entsprechende Maßnahmen wirksam unterdrückt werden. Häufig entstehen solche *Nebenaussendung*, oder auch *Nebenprodukte* genannt (umgangssprachlich auch als "Splatter" bezeichnet), welche das Sendesignal ungewollt verbreitern, durch eine zu hohe Einstellung des Mikrofonverstärkers eines Senders. Hierdurch wird das NF-Signal verzerrt, was unerwünschte Nebenaussendungen zur Folge hat. Abbildung [ref:a_harmonische] zeigt die Nebenaussendungen. 

[question:AJ219]

Auch durch eine nicht ausreichend stabilierte Versorgungsspannung von Senderendstufen können unerwünschte Aussendungen entstehen. Hierbei kann beispielsweise ein schlecht gefiltertes oder stabilisiertes Netzteil (mit Brummspannung behaftet) auf der Versorgungsspannungsseite zu AM-Aussendungen der Endstufe führen. Auch Einstreuungen von NF-Signalen auf der Netzversorgungsseite eines Senders können zu entsprechenden AM-Aussendungen führen. Dies ist oft bei CW-Aussendungen als "verbrummter" Träger/Ton wahrzunehmen, insbesondere bei älteren Sendern.

[question:AJ222]
[question:AJ223]