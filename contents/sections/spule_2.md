In der Funktechnik spricht man auch von einer Impedanz. Beispiele: Antennenimpedanz bei $\qty{3,6}{\mega\hertz}$, Eingangs- und Ausgangsimpedanz einer Verstärkerstufe, Impedanzwandler
<indepth>
[photo:269:a_Widerstandsdreieck R - L:Geometrische Addition von R und $X_L$ und Phasenverschiebung zwischen Z und R]
Da die Gesamtspannung an $Z$ anliegt und der Strom in Phase mit $R$ zu sehen ist, ergibt sich eine Phasenverschiebung von $\varphi = \qty{45}{\degree}$, wobei $I$ gegenüber $U$ nacheilend ist.

</indepth>

<indepth>
[photo:270:a_Pulvereisenringkern:Beispiel für einen Pulvereisenringkern]
[photo:271:a_Ferritringkern:Beispiel für einen Ferritkern]  
</indepth>

Bei einer Reihenschaltung von Blindwiderstand und Wirkwiderstand ergibt sich ein Scheinwiderstand $Z$, der nur im Betrieb an Wechselspannung auftritt und nicht mit einem Ohm-Meter gemessen werden kann. Er wird auch als Impedanz $Z$ bezeichnet und als Widerstand in Ohm angegeben.
Merke: Der Begriff Impedanz steht für einen Widerstand, der sich aus einem ohmschen Anteil ($R$) und einem kapazitiven  ($X_C$) und/oder induktiven Anteil ($X_L$) zusammensetzt.

Beispiel: Wirkwiderstand $\qty{100}{\ohm}$ und Blindwiderstand $\qty{100}{\ohm}$ in Reihenschaltung ergeben einen Scheinwiderstand (Impedanz) von $\qty{141}{\ohm}$.
Das Ergebnis entsteht durch geometrische Addition der beiden Widerstände über ein rechtwinliges Dreieck nach dem den Satz des Pythagoras.
$a^2$ +$b^2$ = $c^2$
Für die Widerstände bedeutet dies: $R^2$ +$X_L ^2$ = $Z^2$
$Z  = \sqrt{(\qty{100}{\ohm})^2 + (\qty{100}{\ohm})^2} = \qty{141}{\ohm}$
Bitte nachrechnen!
[question:AA101]

In der Funktechnik ist vor allem das Verhalten an Wechselspannung wichtig.
Die Spule zeigt, ähnlich wie ein Kondensator, einen "Wechselstromwiderstand ", dass heißt, obwohl der Spulendraht nur einen sehr kleinen ohmschen Widerstand (Leiterwiderstand) besitzt, fließt bei einem Betrieb an Wechselspannung kein Kurzschlussstrom, sondern ein Strom, der mit steigender Frequenz der Wechselspannung kleiner wird. 

% todo Bild Stromkreis mit XL

Die Ursache ist der Anstieg des induktiven Blindwiderstandes $X_L$.
[question:AC203]
(siehe Formelsammlung Seite 236 oben links -  Stichwort: Induktiver Blindwiderstand)
$X_L$"  links oben.
$X_L = \omega \cdot L = 2\pi \cdot f \cdot L$
Beispielrechnung für die Frage AC 204:
$X_L = 2\pi \cdot \qty{100}{\mega\hertz} \cdot \qty{3}{\micro\henry}$
Jetzt werden die Vorsilben in Zehnerpotenzen umgewandelt, damit das Ergebnis in Ohm berechnet werden kann.
$X_L = 6,28 \cdot \qty{100e6}{\hertz} \cdot \qty{3e-6}{\henry}$
Die Zehnerpotenzen  $10^6 \cdot 10^{-6}$ ergeben $1$. Im letzten Schritt werden die verbliebenen Zahlen multipliziert.
$X_L = 6,28 \cdot \qty{(100 \cdot 3)}{\ohm} = \qty{1884}{\ohm}$
[question:AC204]
Mit einem vektoriellen Network Analyzer (VNA) läßt sich die Veränderung des induktiven Blindwiderstandes $X-L$ in Abhängigkeit von der Frequenz darstellen. Wir sprechen auch hier von einem Blindwiderstand, da eine verlustfreie Spule keine Wirkenergie aufnimmt. Sollte eine Spule bei Hochfrequenzanwendungen warm werden, dann besitz sie Verluste, die diese Erwärmung bewirken.
Die Verluste entstehen durch den ohmschen Widerstand des Drahtes und zusätzlich wirkt auch noch der Skin-Effekt, der den Drahtquerschnitt scheinbar verkleinert.
% todo BILD XL in Abhängigkeit der Frequenz
[photo:265:a_XL Verlauf V2:Veränderung des induktiven Blindwiderstandes $X_L$ einer Spule von $\qty{500}{\kilo\hertz}$ bis $\qty{10}{\mega\hertz}$]
Die rote Linie zeigt die Phasenlage des induktiven Blindwiderstandes $X_L$.
[question:AC202]

[picture:944:a_Blindleistung Spule:Das Produkt von $U \cdot I$ ergibt die grüne Leistungskurve]
Die Phasenverschiebung zwischen Spannung und Strom beträgt 90 Grad, wobei der Strom nacheilend ist.
Daraus ergibt sich eine Leistungskurve, die um die Nulllinie symmetrisch schwankt. Der Mittelwert ergibt Null, d.h. es wird keine Wirkleistung aufgenommen.
Wir sprechen deshalb auch bei einer verlustfreien Spule von Blindleistung und Blindwiderstand.
[question:AC201]


% entfernt [photo:266:a_Blindleistung einer Spule:Blindleistung in einer Spule]
Sollte eine Spule bei Hochfrequenzanwendungen warm werden, dann besitzt sie Verluste, die diese Erwärmung bewirken.
Die Verluste entstehen durch den ohmschen Widerstand des Drahtes und zusätzlich wirkt auch noch der Skin-Effekt, der den Drahtquerschnitt scheinbar verkleinert.
[question:AC209]

Grundsätzlich steigt die Induktivität wenn die Windungszahl erhöht wird, die Spulenlänge verkürzt wird, die Querschnittsfläche der Spule vergrößert wird und ein magnetisch leitfähigeres Material als Spulenkern verwendet wird.
Zur Erhöhung der Induktivität, ohne die Windungszahl drastisch zu steigern,  wird die Wicklung auf einen Ferritringkern gewickelt. Drosselspulen mit hoher Induktivität werden zur Verringerung hochfrequenter Ströme eingesetzt.

---

[question:AC211]
Eine wichtige Kenngöße einer Spule ist die Induktivität $L$. Sie gibt an, welche Selbstinduktionsspannung die Spule erzeugen kann und dadurch den fließenden Strom, im Einschalt- und Ausschaltmoment verzögert. Der Formelbuchstabe $L$ wurde zu Ehren des Professors Emil Lenz aus St. Petersburg (1804 - 1864, Verfasser der Lenzschen Regel) gewählt.

Bei Ringkernspulen wird zur Erleichterung der Induktivitätsberechnung ein sogenannter $A_L$-Wert des Kernmaterials angegeben.
Die Berechnung der Induktivität lautet dann:
L = $N^2$ * $A_L$
(siehe Formelsammlung Seite 236 oben rechts -  Stichwort: Induktivität einer Ringkernspule)
ACHTUNG: Die Benennung des $A_L$-Wertes ist in Nanohenry pro Windungen im Quadrat angegeben.
Berechnungsbeispiel für die Induktivität einer Ringkernspule Frage AC 205:
L = $N^2$ * $A_L$
$L = 14^2 \cdot \qty{1,5}{\nano\henry} = \qty{294}{\nano\henry} = \qty{0,294}{\micro\henry}$
Die letzte Umwandlung ist notwendig, da die Lösung mit dieser Vorsilbe angegeben ist.
[question:AC205]

[question:AC206]

Beispielrechnung für die Frage AC 207:
Berechnungsbeispiel für die Windungszahl einer Ringkernspule:
$N = \sqrt \frac{L}{A_L}$
$N = \sqrt \frac{\qty{2}{\milli\henry}}{\qty{250}{\nano\henry}}$
Wichtig: Umwandlung von $\qty{2}{\milli\henry}$ in $\qty{2000000}{\nano\henry}$, damit sich gleiche Vorsilben kürzen lassen.
$N = \sqrt \frac{\qty{2000000}{\nano\henry}}{\qty{250}{\nano\henry}}$
$N = \sqrt {8000}$
$N = 89,4$
Man wird 90 Windungen aufbringen.
[question:AC207]

[question:AC208]

<indepth>
Wenn sich innerhalb der Spule ein magnetisch leitfähiges Material befindet (z.B. Eisen, Ferrit) dann wird das Magnetfeld verstärkt. Die dann wirksame magnetische Flussdichte B läßt sich mit folgender Formel berechnen:
$B = \mu_0 \cdot \mu_r \cdot H$
(siehe Formelsammlung Seite 236 oben rechts -  Stichwort: Magnetische Flussdichte)
Dabei enspricht $\mu_0$ der magnetischen Feldkonstante $\qty{1,2566e-6}{\volt\second\per\ampere\meter}$
$\mu_r$ steht für die relative Permeabilität des Kernmaterials in der Spule. Für Luft wird der Faktor 1 eingesetzt.
(siehe Formelsammlung Seite 243 unten rechts -  Stichwort: Magnetische Feldkonstante; relative Permeabilität )
</indepth>

<summary>
*Zusammenfassung (Version 1)*:
 Impedanz = besteht aus Wirkwiderstand und Blindwiderstand = Scheinwiderstand in Ohm
 
*MERKE: Induktivitäät, Strom zu späät!*
   
Formel Seite 236
$X_L =\omega \cdot L = 2\pi \cdot f \cdot L$
Umgestellt nach L:
$L =\frac{X_L}{2\pi \cdot f}$
  
$A_L$ - Wert in $\unit{\nano\henry}$ !!!
$L = N^2 \cdot A_L$
Umgestellt nach N:  
$N = \sqrt \frac{L}{A_L}$
Hohe Spulenverluste = niedrige Güte = großer tan "delta" = großer ESR  
</summary>

<margin>
|Zusammenfassung Spule                                                            |
|*Spule an Wechselspannung*|
|Impedanz = besteht aus Wirkwiderstand und Blindwiderstand = Scheinwiderstand in Ohm|
|*MERKE: Induktivitäät, Strom zu späät!*|  
|Formel Seite 236|
|$X_L =\omega \cdot L = 2\pi \cdot f \cdot L$|
Umgestellt nach L:|
$L =\frac{X_L}{2\pi \cdot f}$| 
|$A_L$ - Wert in $\unit{\nano\henry}$ !!!|
|$L = N^2 \cdot A_L$|
|Umgestellt nach N:|  
|$N = \sqrt \frac{L}{A_L}$|
|Hohe Spulenverluste = niedrige Güte = großer tan "delta" = großer ESR|    
[table:a_Spule Zusammenfassung:Zusammenfassung zur Spule in Klasse A]
</margin>


Hier geht es um die Abschirmung des elektrischen Feldes durch ein Alu-Gehäuse. 
[question:AC210]


Zur Abschirmung eines Magnetfeldes benötigt man ein magnetisch gut leitfähiges Material.

<margin>
Lösungshilfe:

*AC 206:* $\qty{112,5}{\milli\henry}$
*AC 208:* 20 Windungen
</margin>




