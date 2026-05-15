In jedem Funkgerät sind eine oder mehrere Spannungsstabilisierungen vorhanden, da die Eingangsspannung,  vor allem bei mit Akku betriebenen Geräten, schwanken kann und dann empfindliche Baugruppen, wie z.B. Oszillatoren, ihre Frequenz ändern würden.

Spannungsstabilisierungen gibt es in 3 Varianten:
1. Die *Schaltung mit Z-Diode* stellt eine sehr einfache Schaltung zur Stabilisierung der Ausgangsspannung dar, da die Z-Diode die Ausgangsspannung in Grenzen stabil halten kann.

<margin>
Zur Erinnerung:
[picture:862:n_diode_kennlinie_uz:Kennline einer Z-Diode]
Die Z-Diode wird immer mit einem Vorwiderstand und in Sperrrichtung ($-U_\text{Z}$) betrieben. Z-Dioden mit Durchbruchspannungen $U_\text{Z}$ ab $\qty{5}{\volt}$, zeigen einen sehr steilen Verlauf der Kennlinie und eignen sich deshalb sehr gut zur Spannungsstabilisierung.
(siehe auch Klasse E: Abschnitt Diode 1)
</margin>

[picture:323:a_Stabilisierung mit Z-Diode:Spannungsstabilisierung mit Z-Diode]

---
[question:AD321]

Der Wirkungsgrad der Schaltung ist sehr niedrig, da die Verluste im Vorwiderstand $R_\text{V}$ und in der Z-Diode berücksichtigt werden müssen. Die Berechnung ist sehr aufwändig.

<tip>
Lösungsweg:
Spannung am Lastwiderstand: $U_\text{L} = I_\text{L} \cdot R_\text{L} = \qty{10}{\milli\ampere} \cdot \qty{470}{\ohm} = \qty{4700}{\milli\volt} = \qty{4,7}{\volt}$
Leistung im Lastwiderstand: $P_{\mathrm{out}} = \qty{4,7}{\volt} \cdot \qty{10}{\milli\ampere} = \qty{47}{\milli\watt}$
Verlustleistung in der Z-Diode: $P_{VZ} = \qty{4,7}{\volt} \cdot \qty{15}{\milli\ampere} = \qty{70,5}{\milli\watt}$
Eingangsstrom: $I_g = \qty{10}{\milli\ampere} + \qty{15}{\milli\ampere} = \qty{25}{\milli\ampere}$
Eingangsleistung: $P_{\mathrm{in}} = \qty{13,8}{\volt} \cdot \qty{25}{\milli\ampere} = \qty{345}{\milli\watt}$
Wirkungsgrad: $\eta = \frac{P_{out}}{P_{in}} = \frac{\qty{47}{\milli\watt}}{\qty{345}{\milli\watt}} = \num{0,1}$
  
</tip>


---
2. *Lineare Spannungsregler* stabilisieren die Ausgangsspannung dadurch, indem ein Leistungstransistor als veränderlicher Widerstand betrieben wird und zusammen mit dem Lastwiderstand einen Spannungsteiler bildet.
[picture:490:a_diskret aufgebaute Spannungsstabilisierung:diskret aufgebaute Spannungsstabilisierung]
In der folgenden Frage ist eine diskrete Spannungsstabilisierung mit Längstransistor dargestellt. Über eine Z-Diode wird eine Referenzspannung von $\qty{5,6}{\volt}$ an der Basis des Transistors erzeugt. Das Emitterpotential ist im Betriebszustand eines Siliziumtransistor um etwa $\qty{0,6}{\volt}$ niedriger als das Basispotential. Die geregelte Ausgangsspannung liegt dann bei etwa $\qty{5}{\volt}$.
%todo nur Schaltung aus Bild 490 darstellen
Der Laststrom fließt auch durch den Transistor und dadurch wird er bei hohem Laststrom sehr warm. Die sogenannten Längstransistoren befinden sich deshalb bei linear geregelten Spannungsstabilisierungen immer auf einem Kühlkörper. 

<margin>
 [photo:246:a_Längstransistor 2N3055 auf Kühlkörper:Der Längstransistor in einem linear geregelten Netzteil muss große Verlustleistungen aushalten und wird deshalb auf einen Kühlkörper montiert.]
</margin>

<margin>
[photo:307:a_linear geregeltes Netzteil:Innenansicht eines linear geregelten Netzteils für $\qty{13,8}{\volt}$ und $\qty{25}{\ampere}$; Gewicht $\qty{7}{\kilo\gram}$]
Der schwere Netztrafo bestimmt im Wesentlichen das Gesamtgewicht. 
Unter der Regelung befindet sich ein großer Kühlkörper mit den Längstransistoren, die durch den Lüfter gekühlt werden
</margin>


[question:AD315]
Die Verlustleistung $P_\text{V}$ ergibt sich aus der Differenz von  $P_{\mathrm{in}} - P_{\mathrm{out}}$.

------
[question:AD319]
Die Verlustleistung $P_\text{V}$ bestimmt auch den Wirkungsgrad eines Spannungsreglers. Bei linearen Spannungsreglern ist der Wirkungsgrad systembedingt oft sehr niedrig. Mit der folgenden Formel lässt sich der Wirkungsgrad berechnen:
Wirkungsgrad = abgegebene Leistung auf der Lastseite : gesamte Eingangsleistung
$\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}}$

<tip>
Eingangsleistung = Eingangsspannung x Laststrom
$P_{\mathrm{in}} = U_{\mathrm{in}} \cdot I_\text{L}$
$P_{\mathrm{in}} = \qty{13,8}{\volt} \cdot \qty{0,9}{\ampere} = \qty{12,42}{\watt}$
Ausgangsleistung =  Ausgangsspannung x Laststrom
$P_{\mathrm{out}} = U_{\mathrm{out}} \cdot I_\text{L}$
$P_{\mathrm{out}} = \qty{9}{\volt} \cdot \qty{0,9}{\ampere} = \qty{8,1}{\watt}$
</tip>
---
[question:AD320]

<tip>
Der Lösungsweg beginnt mit der Berechnung der Einzelleistungen. 
Eingangsleistung = Eingangsspannung x Laststrom
$P_{\mathrm{in}} = U_{\mathrm{in}} \cdot I_\text{L}$
$P_{\mathrm{in}} = \qty{13,8}{\volt} \cdot \qty{0,455}{\ampere} = \qty{6,28}{\watt}$
Ausgangsleistung = Ausgangsspannung x Laststrom
$P_{\mathrm{out}} = U_{\mathrm{out}} \cdot I_\text{L}$
$P_{\mathrm{out}} = \qty{5}{\volt} \cdot \qty{0,450}{\ampere} = \qty{2,25}{\watt}$
  
$\eta = \frac{P_{\mathrm{out}}}{P_{\mathrm{in}}} = \frac{\qty{2,25}{\watt}}{\qty{6,28}{\watt}} = \num{0,36}$
</tip>

3. *Festspannungsregler* in einer integrierten Schaltung
[picture:200:a_Festspannungsregler:Festspannungsregler]

Festspannungsregler arbeiten wie lineare Spannungsregler mit Längstransistor und  beinhalten eine sehr genaue Spannungsreferenzquelle zusammen mit einer optimalen elektronischen Regelung. Auch wenn die Eingangsspannung stark  schwankt (z.B. $\qty{\pm 2}{\volt}$) ist auf der Lastseite die Spannungsänderung nur im Millivoltbereich messbar. Die Kondensatoren auf beiden Seiten des Festspannungsreglers müssen nach Vorgaben des Herstellers gewählt werden, sonst kann es zu unerwünschten Schwingungen im Regelverhalten der Schaltung kommen.

---
[question:AD318]

<tip>
Der Lösungsweg beginnt mit der Berechnung des Laststromes: $I_\text{L} = \frac{\qty{5}{\volt}}{\qty{10}{\ohm}} = \qty{0,5}{\ampere}$
Eingangsleistung = Eingangsspannung x Laststrom
Hinweis: Der Strom in der Masseleitung des Festspannungsreglers ist vernachlässigbar klein und wird deshalb nicht berücksichtigt.
$P_{\mathrm{in}} = U_{\mathrm{in}} \cdot I_\text{L} = \qty{13,8}{\volt} \cdot \qty{0,5}{\ampere} = \qty{6,9}{\watt}$
  
Ausgangsleistung = Ausgangsspannung x Laststrom
$P_{\mathrm{out}} = U_{\mathrm{out}} \cdot I_\text{L} = \qty{5}{\volt} \cdot \qty{0,5}{\ampere} = \qty{2,5}{\watt}$
</tip>
Die Verlustleistung $P_\text{V}$ des Festspannungsreglers ergibt sich aus der Differenz von $P_{\mathrm{in}}$ und $P_{\mathrm{out}}$.

$P_\text{V} = P_{\mathrm{in}} - P_{\mathrm{out}} = \qty{6,9}{\watt} - \qty{2,5}{\watt} = \qty{4,4}{\watt}$

<margin>
[photo:245:a_Festspannungsregler:Festspannungsregler für $\qty{5}{\volt}$, $\qty{12}{\volt}$ und $\qty{9}{\volt}$ auf Kühlkörper]
</margin>
---
[question:AD317]

<tip>
Damit die interne Regelschaltung optimal funktioniert, muss die Eingangsspannung bei Standard-Festspannungsregler (z.B. Typ 7812) um ca. $\qty{3}{\volt}$ größer als die Ausgangsspannung sein. Es gibt Festspannungsregler, bei denen die Eingangsspannung nur um $\qty{1}{\volt}$ größer als die Ausgangsspannung sein muss. Diese Regler heißen Low-Drop-Spannungsregler.
</tip>
  
[question:AD316]

<margin>
Lösungshilfe
AD 315: $\qty{5}{\volt}$
AD 316: Die Eingangsspannung muss größer als die gewünschte Ausgangsspannung sein.
AD 317: Die Spannungsschwankung beträgt nahezu null Volt.
AD 318: $\qty{4,4}{\watt}$
AD 319: $\qty{12,42}{\watt} - \qty{8,1}{\watt} = \qty{4,32}{\watt}$
AD 320: $\num{0,36}$
AD 321: $\num{0,14}$
  
</margin>
  
