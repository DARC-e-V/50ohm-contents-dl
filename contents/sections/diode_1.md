Bereits aus der Klasse-N-Ausbildung ist die Grundfunktion der Diode bekannt: sie lässt Strom nur in einer Richtung fließen, nämlich wenn die an der Anode anliegende Spannung ($U_a$) größer ist als die Spannung an der Kathode ($U_k$), vgl. Abbildung [ref:e_diode_u_i].

<margin>
[picture:859:e_diode_u_i:Spannungen und Strom an einer Diode mit Vorwiderstand]
</margin>

Mathematisch können wir diese Forderung so schreiben:

$U_d = U_a - U_k > 0$

Ist allerdings $U_d$ nur ein ganz wenig größer als 0, fließt noch kein merkbarer Strom. Sobald $U_d$ eine Schwellspannung überschreitet, fließt ein großer Strom. Diese Schwellspannung ist von der Bauart der Diode abhängig und heißt auch Flussspannung, weil bei ihrem Überschreiten so richtig viel Strom fließt. Das liegt an der *exponentiellen Kennlinie* einer Diode.

<margin>
[picture:861:e_diode_kennlinie_iu:Kennlinie einer Diode]
</margin>

<indepth>
Der Diodenstrom ist durch eine exponentielle Gleichung gegeben. "Exponentiell" heißt sie, weil sich die unabhängige Variable $U_d$ im Exponenten, also der "Hochzahl" befindet.

$I_d = I_S \left(e^{\frac{U_d}{U_T}}-1\right)$

$e$ ist die sogenannte Euler'sche Zahl ($e\approx 2,718$), $U_T$ eine Konstante, die bei Raumtemperatur etwa $\qty{26}{\milli\volt}$ beträgt.

$I_S$ ist hier der *Sperrsättigungsstrom*, das ist der sehr kleine Strom, der bei negativen Spannungen durch die Diode fließt. Der Wert von $I_S$ hängt neben ein paar Parametern der Diode, wie der Diodenfläche, vor allem auch vom verwendeten Halbleitermaterial ab. Bei Materialien wie Germanium (Ge) mit einer geringen *Energiebandlücke* (darauf gehen wir in der Ausbildung zur Klasse A näher ein) ist $I_S$ größer, bei Materialien mit größerer Energiebandlücke ist $I_S$ kleiner.
</indepth>

[question:EC501]

Betrachten wir eine Diodenkennlinie in Abbildung [ref:e_diode_kennlinie_iu], so steigt der Diodenstrom bei positiven $U_d$ ab einer gewissen Spannung steil an. Diese Spannung wird auch als *Schwellspannung* $U_{th}$ bezeichnet, sie ist aber nur Ausdruck der unterschiedlichen $I_S$: je kleiner $I_S$, desto höher ist die Schwellspannung. 

Als Anhaltspunkte für die Schwellspannung von Dioden können wir für Germanium (Ge) etwa $\qtyrange{0,2}{0,3}{\volt}$ und für Silizium (Si) etwa $\qtyrange{0,6}{0,7}{\volt}$ angeben.

<attention>
Die Schwellspannung $U_{th}$ wird auch *Flussspannung* genannt, weil erst ab dieser Spannung der Strom markant zu fließen beginnt.
</attention>

*Leuchtdioden* (LEDs) sind spezielle Dioden, bei denen das Halbleitermaterial so beschaffen ist, dass es bei Polung der Diode in Flussrichtung Licht aussendet. Das geht nur mit bestimmten Materialien - mit Si und Ge nicht. Die Farbe des Lichts ist durch die Energiebandlücke gegeben. Je größer die Energiebandlücke, desto kurzwelliger das Licht, um so geringer der Sperrsättigungsstrom, und daher um so höher die Schwellspannung. Daher haben rote LEDs etwa $\qty{1,7}{\volt}$ Schwellspannung und grüne LEDs $\qty{2,5}{\volt}$. Die verschiedenen Kennlinien sind in der Abbildung [ref:e_diode_kennlinien] dargestellt.

[question:EC513]
[question:EC510]
[question:EC509]
[question:EC511]
[question:EC512]

---

<margin>
[picture:858:e_diode_kennlinien:Kennlinien verschiedener Dioden]
</margin>


[question:EC503]
[question:EC506]
[question:EC507]
[question:EC508]

Da LEDs in Flussrichtung betrieben werden, ist es wichtig, einen Widerstand $R_V$ zwischen Spannungsquelle $U$ und LED zu schalten. $R_V$ stellt den erwünschten Strom $I$ ein. Dabei ist die Schwellspannung $U_{th}$ der LED zu berücksichtigen:

$ I=\frac{U-U_{th}}{R_V}$

[question:EC514]
[question:EC515]
[question:EC516]

---

In unserem einfachen Modell fließt für negative $U_d$ nur ein geringer Sperrstrom. Das stimmt aber nicht für sehr negative Spannungen. Irgendwann wird das elektrische Feld über der Sperrschicht zu hoch und die Diode "bricht durch", der Strom in Rückwärtsrichtung steigt extrem stark an, wie in Abbildung [ref:n_diode_kennlinie_uz] gezeigt.

Dieser *Sperrdurchbruch* kann verschiedene physikalische Ursachen haben, die wir hier nicht im Detail behandeln können. Die Spannung, bei der dieser Durchbruch passiert, wird gemeinhin als *Zener-Spannung* $U_z$ bezeichnet, auch wenn der Zener-Effekt (ein quantenmechanischer Tunneleffekt) nur ein möglicher Durchbruchmechanismus ist. *Zenerdioden* werden zur Spannungsstabilisierung verwendet. Dabei ist es wichtig, den Durchbruchstrom durch einen Vorwiderstand zu begrenzen. 

<margin>
[picture:862:n_diode_kennlinie_uz:Kennlinie einer Z-Diode]
</margin>

---

Das Schaltsymbol einer Zenerdiode (Abbildung [ref:e_zener_symbol]) ist das einer regulären Diode, bei der der Kathodenstrich eine zusätzliche Fortsetzung unter $\qty{90}{\degree}$ erhält. Dies soll an das "Abknicken" der Kennlinie im Durchbruch erinnern.

<margin>
[picture:860:e_zener_symbol:Schaltsymbol einer Zenerdiode]
</margin>



[question:EC517]
[question:EC520]
[question:EC521]
[question:EC522]

Die bisher behandelten Dioden waren Dioden, deren Diodeneigenschaft durch einen Halbleiterübergang entsteht, der erst in [sec:diode_2] behandelt wird. Bei der *Schottky-Diode* handelt es sich um eine Diode, deren Eigenschaften durch einen Metall-Halbleiter-Übergang entstehen. Die Schwellspannung ist etwa halb so groß wie die einer herkömmlichen Halbleiterdiode aus dem selben Material, oder kleiner, abhängig von der genauen Gestaltung des Metall-Halbleiter-Übergangs. Schottky-Dioden werden eingesetzt, wenn die Schwellspannung gering sein soll, oder aber als sehr schnelle Schaltdioden.

[question:EC504]
[question:EC505]

<margin>
Metall-Halbleiter-Dioden sind die ältesten Gleichrichterbauelemente auf Halbleiterbasis. Ferdinand Braun entdeckte ihren Gleichrichtereffekt bereits 1874, ohne aber seine Beobachtung erklären zu können.
</margin>

Fassen wir zusammen:

Dioden lassen Strom nur einer Richtung fließen. Daher eignen sie sich zur Gleichrichtung von Wechselstrom.

Bei hohen Sperrspannungen allerdings ($U_d < U_z$), steigt der Strom in Rückwärtsrichtung stark an. Dieser Betriebspunkt kann sehr gut zur Spannungsstabilisierung genutzt werden (*Zenerdiode*).

Daneben lassen sie sich in Sperrrichtung auch als spannungsgesteuerte Kapazitäten verwenden, dies werden wir aber erst in der Ausbildung zur Klasse A behandeln. 

[question:EC502]
[question:EC518]
[question:EC519]
