Ein altes Funkersprichwort sagt, dass der beste Hochfrequenzverstärker die Antenne ist. In den ersten Jahren der Funktechnik war sie der einzige "Verstärker", verstärkende Elektronik gab es nicht. 1907 kam dann die Elektronenröhre - ein sehr erfolgreiches Bauelement, aber doch recht groß und wenig effizient. Bereits seit den zwanziger Jahren träumte die Wissenschaft von Bauelementen ähnlicher Funktion, bei der aber alles im Inneren eines Festkörpers (Halbleiters) abläuft, nicht im Vakuum. Das erste Bauelement, bei dem das auch praktisch gelang, war 1947/1948 der *Bipolartransistor*, der auch ganz überwiegend Gegenstand der Prüfungsfragen der Klasse-E-Prüfung ist.

[question:EC602]

<indepth>
Der *Bipolartransistor* wird im Englischen auch BJT: Bipolar Junction Transistor, dt. bipolarer Sperrschicht-Transistor genannt.
</indepth>

Die ideale Funktion aller Transistortypen, und auch der Elektronenröhre, ist die einer *spannungsgesteuerten Stromquelle*: mit einer möglichst kleinen Spannungsänderung am Eingang soll eine möglichst große Stromänderung am Ausgang bewirkt werden.

Der Bipolartransistor hat drei Anschlüsse, die Emitter, Basis und Kollektor genannt werden. Der Emitter sendet Ladungsträger in die Basis -- beim npn-Bipolartransistor sind das *Elektronen*, beim pnp-Bipolartransistor Defektelekronen, auch *Löcher* genannt. Die Physik hinter diesen Begriffen werden wir erst in der Ausbildung für die Klasse A besprechen. Diese Ladungsträger durchqueren die Basis und werden vom Kollektor wieder aufgesammelt. 

---

Die Abbildung [ref:e_npn_pnp_symbol] zeigt die Schaltzeichen von NPN- und PNP-Transistoren. Die Emitterelektrode erkennen wir an einem Pfeil, der beim pnp-Transistor zur Basis hin und beim npn-Transistor von der Basis weg zeigt. 

<margin>
[picture:864:e_npn_pnp_symbol:Symbole NPN und PNP Transistor]
</margin>

[question:EC605]
[question:EC606]
[question:EC607]
[question:EC608]
[question:EC609]

---

Bipolartransistoren sind aus zwei Dioden zusammengesetzt -- der Emitter-Basis- und Basis-Kollektor-Diode.
Im aktiven Betrieb ist die Emitter-Basis-Diode stets in Flussrichtung geschaltet. Beim NPN-Transistor muss dabei das Potential an der Basis positiver sein als das des Emitters, beim PNP-Transistor negativer. Die Basis-Kollektor-Diode ist in Sperrrichtung gepolt. Dazu ist das Kollektorpotential beim NPN-Transistor positiver als die Basis zu wählen, beim PNP-Transistor negativer.

<tip>
Die Transistorfunktion stellt sich aber nur ein, wenn die Basiszone zwischen Emitter und Kollektor maximal wenige Mikrometer breit ist. Also können wir keinen Transistor erzeugen, indem wir zwei separate Dioden aneinander löten.
</tip>

Die minimale Spannung am Emitter-Basis-Übergang hängt vom verwendeten Halbleiter ab. Bei einem Silizium-NPN-Transistor muss die Basis etwa $\qty{0,6}{\volt}$ positiver als der Emitter sein, beim Silizium-PNP-Transistor etwa $\qty{0,6}{\volt}$ negativer.

[question:EC610]
[question:EC612]
[question:EC613]
[question:EC614]
[question:EC615]

---

<margin>
[picture:863:e_npn_i_u:Ströme uns Spannungen an einem npn-Transistor]
</margin>

---

Die Ströme und Spannungen an einem npn-Transistor sind in der Abbildung [ref:e_npn_i_u] dargestellt. Die Basis-Emitter-Spannung $U_{BE}$ kennen wir bereits, ebenso die Kollektor-Basis-Spannung $U_{CB}$. Der Kollektorstrom $I_C$ hängt exponentiell von der Basis-Emitter-Spannung ab:

$I_C = I_\text{S}\ e^{\frac{U_{BE}}{U_T}}$

$U_T$ ist bei Raumtemperatur etwa $\qty{26}{\milli\volt}$.

<indepth>
$I_\text{S}$ bezeichnet den sogenannten Sättigungs-Sperrstrom eines Bipolartransistors. Er ist ein charakteristischer Bauteilparameter und steht in engem Zusammenhang mit der Emitter-Basis-Diode. Dabei handelt es sich um einen sehr kleinen Leckstrom, der auch dann durch den Transistor fließt, wenn die Basis-Emitter-Strecke nicht leitend ist.
</indepth>

Der Basisstrom $I_B$ hat in weiten Betriebsbereichen die gleiche Spannungsabhängig wie der Kollektorstrom, sodass das Verhältnis von Kollektorstrom und Basisstrom konstant ist:

$\frac{I_C}{I_B} = B$

*B* ist die Stromverstärkung (genau genommen die Stromverstärkung in Emitterschaltung). Es ist oft praktischer, sich den Transistor als ein stromgesteuertes Bauelement vorzustellen, auch wenn das physikalisch nicht so ist. Die Stromverstärkung beträgt in praktischen Transistoren 50..350.

<tip>
Für die Stromsteuerung des Bipolartransistors gibt es eine uralte Analogie, bei der ein großer und ein kleiner Wasserkanal, ein Wehr im großen Kanal und eine Steuerklappe eine Rolle spielen. Die Älteren unter uns kennen das vielleicht noch aus dem "Kleinen Radiomann" des Kosmos-Verlags ...
  
[picture:835:e_transistor_wehr_geschlossen:Steuerkanal schließt Wehr komplett]
  
Zunächst fließt kein Wasser im kleinen Kanal. Das Wehr im großen Kanal ist geschlossen, daher fließt dort auch kein Wasser.
  
[picture:837:e_transistor_wehr_halb_offen:Steuerkanal öffnet Wehr halb]

Dann beginnt Wasser im kleinen Kanal zu fließen, dem Steuerkanal. Das Wasser hebt die Klappe an, die wiederum das Wehr betätigt -- auch im Hauptkanal beginnt, Wasser zu fließen.
  
[picture:836:e_transistor_wehr_geoeffnet:Steuerkanal öffnet Wehr komplett]

Jetzt fließt mehr Wasser im Steuerkanal, die Klappe wird weiter angehoben, das Wehr im Hauptkanal öffnet komplett.
</tip>

[question:EC603]

Der Emitterstrom $I_E$ ist die Summe aus Kollektorstrom und Basisstrom:

$I_E = I_C + I_B$

[question:EC611]

Der Spannungsarbeitspunkt von Transistoren wird meist über die Kollektor-Emitter-Spannung angegeben:

$U_{CE} = U_{CB} + U_{BE}$

Neben den hier überwiegend behandelten Bipolartransistoren gibt es vor allem auch *Feldeffekttransistoren*, die physikalisch anders funktionieren, aber nach außen die selbe Grundfunktion (spannungsgesteuerte Stromquelle) haben. In Form der MOSFETs beherrschen sie unsere Elektronik, denn sie sind millionen- bis milliardenfach in den integrierten Schaltkreisen der Digitalelektronik enthalten.

<indepth>
MOSFET steht für *metal-oxide-semiconductor field effect transistor*, dt. Metall-Oxid-Halbleiter-Feldeffekttransistor
</indepth>

[question:EC604]

Transistoren können nicht nur als Verstärker, sondern auch als (Strom-)Schalter (Strom an/aus) oder auch, bei kleinen Spannungen am Ausgang, als steuerbarer Widerstand eingesetzt werden. Die letzte Funktion wird vor allem mit Feldeffekttransistoren umgesetzt.

[question:EC601]
