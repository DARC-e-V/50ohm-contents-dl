Um den Sicherheitsabstand zu Berechnen gibt es eine Näherungsformel. Wir finden Sie in der Formelsammlung: 

$ E = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{d} $

Diese kann man schnell zum Sicherheitsabstand $d$ umstellen: 

$ d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{E} $

Die Formelsammlung hat noch einen Hinweis, dass die obige Formel erst für Berechnungen im Fernfeld (bzw. stahlendem Nahfeld) ab $ d > \frac{\lambda}{2\pi} $ gilt.

Das liegt daran, dass nur im Fernfeld das elektrische und das magnetische Feld eine feste, konstante Phasenbeziehung zueinander aufweisen. Im reaktiven Nahfeld kann es hingegen lokal zu starken Überhöhungen sowohl des elektrischen als auch des magnetischen Feldes kommen. Diese Effekte lassen sich mit den Näherungsformeln für das Fernfeld nicht zuverlässig erfassen. Für Berechnungen im reaktiven Nahfeld, also für Abstände $d \le \frac{\lambda}{2\pi}$, sind daher in der Regel numerische Simulationen erforderlich. Mit Einschränkungen (nicht bei magnetischen Antennen, nicht bei sehr kurzen Antennen) sind die Ergebnisse auch im strahlenden Nahfeld brauchbar.

<indepth>
Das Fernfeld einer Strahlungsquelle, ist der Bereich, in dem die Vektoren der elektrischen Feldstärke ($E$), der magnetischen Feldstärke ($H$) senkrecht aufeinander stehen und keine Phasendifferenzen aufweisen. 

Die Grenze zwischen Fernfeld und Nahfeld ist in erster Linie abhängig von der Wellenlänge. Das Fernfeld bildet sich, laut den [Erläuterungen zur BEMFV](https://www.bundesnetzagentur.de/SharedDocs/Downloads/DE/Sachgebiete/Telekommunikation/Verbraucher/ElektromagnetischeFelder/Anzeige_Afu/Erlaeuterung_der_Bewertungsverfahren_nach_BEMFV.pdf?__blob=publicationFile&v=1), in einem Abstand von etwa $4\cdot\lambda$ aus. 

Das Nahfeld unterteilt sich in das *reaktive* und das *strahlende Nahfeld*. Praktisch ist, dass im strahlenden Nahfeld trotzdem die Formel für das Fernfeld verwendet werden kann. Das liegt daran, dass die Näherungsformel hier sehr konservative Abschätzungen liefert, das heißt die tatsächlichen Feldstärken sind geringer als die errechneten. Man ist auf der sicheren Seite. 
  
Mit der Formel $ d > \frac{\lambda}{2\pi} $ stellen wir also sicher, dass wir außerhalb des *reaktiven Nahfelds* sind.
</indepth>

%TODO Applet basteln: https://www.leifiphysik.de/elektrizitaetslehre/elektromagnetische-wellen/versuche/dipolstrahlung-animation

Auf diesen Sachverhalt zielt die folgende Frage ab:

[question:EK105]

Für 3,5 MHz beginnt das Fernfeld (strahlendes Nahfeld) erst bei 13,64 m.

 $ d > \frac{\lambda}{2 \cdot \pi} $
 
 $ d > \frac{\qty{85,7}{\meter}}{2 \cdot \pi} $
 
 $ d > \qty{13,64}{\meter} $ 
 
Der mit $\qty{3,65}{\meter}$ ermittelte Abstand liegt deutlich im reaktiven Nahfeld und ist deshalb ungültig. Statt der Näherungsformel für das Fernfeld muss eine andere Methode gewählt werden. In Frage kommen Messungen der E- und H-Feldanteile, Simulations- oder Nahfeldberechnungen.

Damit die folgende Frage beantwortet werden kann, muss berechnet werden wo das Fernfeld (strahlendes Nahfeld) für das 160 und 80-m-Band beginnt. 

[question:EK106]

Für $\qty{160}{\meter}$ gilt: $d > \frac{\qty{160}{\meter}}{2\pi} = \qty{25,5}{\meter}$
 
Für $\qty{80}{\meter}$ gilt: $d > \frac{\qty{80}{\meter}}{2\pi} = \qty{12,7}{\meter}$

Die Berechnung ist ungültig, wenn die Entfernung für $\qty{160}{\meter}$ kleiner als $\qty{25,5}{\meter}$ und für $\qty{80}{m}$ kleiner als $\qty{12,7}{\meter}$ ist.

%%%%

In der folgenden Frage muss nun erstmals ein richtiger Sicherheitsabstand berechnet werden. 

[question:EK108]

Zunächst müssen wir die Strahlungsleistung in $P_\textrm{EIRP}$ berechnen. Außerdem fällt uns auf, dass der Antennengewinn in $\unit{\dBd}$ angegeben ist. Hierzu nutzen wir wieder die Formel aus der Formelsammlung:

$P_\text{EIRP} = P_\text{Sender} \cdot 10^{\frac{g_i-a+\qty{2,15}{\dB}}{\qty{10}{\dB}}} = \qty{100}{W} \cdot 10^{\frac{\qty{7,5}{\dBd}-\qty{1,5}{\dB}+\qty{2,15}{\dB}}{\qty{10}{\dB}}} \approx \qty{653}{\watt}$

Die Summe der Gewinne und Dämpfungen des gesamten Antennensystems ist der Antennengewinn von 7,5 dBd, abzüglich der Kabeldämpfung von 1,5 dB und plus der Gewinn von 2,15 dBi für den isotropen Strahler (der Antennengewinn bezieht sich auf den Dipol).

Alternativ können wir, wie schon in den vorherigen Kapiteln, für die Gewinne und die Dämpfung die jeweiligen Faktoren ermittelt werden.
$\qty{7,5}{\dB} - \qty{1,5}{dB} = \qty{6}{\dB}$, das entspricht einem Faktor von $4$. Der Faktor für $\qty{2,15}{\dBi}$ ist $1,64$.

$P_\textrm{EIRP} = \qty{100}{\watt} \cdot 4 \cdot 1,64 = \qty{656}{\watt}$

---

Die Ergebnisse der beiden Rechenwegen sollten eigentlich gleich sein. Sie weichen aber etwas von ein ander ab. Das ist das Ergebnis von Rundungen bei den beiden Faktoren. Die vorhanden Leistung ist aber ausreichend genau um die Frage korrekt zu lösen. Wir setzen also diesen Wert in die Abstandsformel ein:

$ d = \frac{\sqrt{\qty{30}{\ohm}\cdot P_\text{EIRP}}}{E} = \frac{\sqrt{\qty{30}{\ohm}\cdot \qty{656}{\watt}}}{\qty{28}{\volt\per\meter}} \approx \qty{5}{\meter}  $

Den Sicherheitsabstand von 5 m wurde mit der Formel für das Fernfeld ermittelt. Deshalb ist er nur dann gültig, wenn der er auch im Fernfeld (bzw. strahlenden Nahfeld) liegt. Das wie oben schnell geprüft werden.

$d > \frac{\lambda}{2\pi}$

$d > \frac{\qty{10}{\meter}}{2\pi}$

$d > \qty{1,6}{\meter} $

Der berechnete Sicherheitsabstand von $\qty{5}{\meter}$ ist Größer als $\qty{1,6}{\meter}$ und liegt eindeutig im Fernfeld (bzw. strahlendem Nahfeld). Die Berechnung ist damit gültig. Die richtige Antwort ist $\qty{5}{\meter}$.

<indepth>
In der Tabelle steht für $\qty{6}{\dB}$ ein Faktor von $4$. Das ist ein gerundeter Wert und beträgt eigentlich $3,981071706$. Deshalb kommt es zum Rundungsfehler.
</indepth>