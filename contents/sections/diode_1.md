Bereits aus der Klasse-N-Ausbildung ist die Grundfunktion der Diode bekannt: sie lässt Strom nur in einer Richtung fließen, nämlich wenn die an der Anode anliegende Spannung ($U_\text{a}$) größer ist als die Spannung an der Kathode ($U_\text{k}$), vgl. Abbildung [ref:e_diode_u_i].

<margin>
[picture:859:e_diode_u_i:Spannungen und Strom an einer Diode mit Vorwiderstand]
</margin>

Mathematisch können wir diese Forderung so schreiben:

$U_\text{d} = U_\text{a} - U_\text{k} > 0$

Ist allerdings $U_\text{d}$ nur ein ganz wenig größer als $0$, fließt noch kein merkbarer Strom. Das liegt an der *exponentiellen Kennlinie* einer Diode. Der Diodenstrom ist nämlich:

$I_\text{d} = I_\text{S} \left(e^{\frac{U_\text{d}}{U_\text{T}}}-1\right)$

$e$ ist die sogenannte Euler'sche Zahl ($e\approx 2,718$), $U_\text{T}$ eine Konstante, die bei Raumtemperatur etwa $\qty{26}{\milli\volt}$ beträgt.

$I_\text{S}$ ist hier der *Sperrsättigungsstrom*, das ist der sehr kleine Strom, der bei negativen Spannungen durch die Diode fließt. Der Wert von $I_\text{S}$ hängt neben ein paar Parametern der Diode, wie der Diodenfläche, vor allem auch vom verwendeten Halbleitermaterial ab. Bei Materialien wie Germanium (Ge) mit einer geringen *Energiebandlücke* (darauf gehen wir in der Ausbildung zur Klasse A näher ein) ist $I_\text{S}$ größer, bei Materialien mit größerer Energiebandlücke ist $I_\text{S}$ kleiner. 

<margin>
[picture:861:e_diode_kennlinie_iu:Kennline einer Diode]
</margin>

[question:EC501]

Betrachten wir eine Diodenkennlinie in Abbildung [ref:e_diode_kennlinie_iu], so steigt der Diodenstrom bei positiven $U_\text{d}$ ab einer gewissen Spannung steil an. Diese Spannung wird auch als *Schwellspannung* $U_\text{th}$ bezeichnet, sie ist aber nur Ausdruck der unterschiedlichen $I_\text{S}$: je kleiner $I_\text{S}$, desto höher ist die Schwellspannung. 

Als Anhaltspunkte für die Schwellspannung von pn-Dioden können wir für Ge etwa $\qtyrange{0,2}{0,3}{\volt}$ und für Si etwa $\qtyrange{0,6}{0,7}{\volt}$ angeben.

*Leuchtdioden* (LEDs) sind ebenfalls pn-Dioden, bei denen das Halbleitermaterial so beschaffen ist, dass es bei Polung der Diode in Flussrichtung Licht aussendet. Das geht nur mit bestimmten Materialien - mit Si und Ge nicht. Die Farbe des Lichts ist durch die Energiebandlücke gegeben. Je größer die Energiebandlücke, desto kurzwelliger das Licht, um so geringer der Sperrsättigungsstrom, und daher um so höher die Schwellspannung. Daher haben rote LEDs etwa $\qty{1,7}{\volt}$ Schwellspannung und grüne LEDs $\qty{2,5}{\volt}$. Die verschienden Kennlinien sind in der Abbildung [ref:e_diode_kennlinien] dargestellt.

[question:EC513]
[question:EC510]
[question:EC509]
[question:EC511]
[question:EC512]

---

<margin>
[picture:858:e_diode_kennlinien:Kennlinen verschiedener Dioden]
</margin>


[question:EC503]
[question:EC506]
[question:EC507]
[question:EC508]

Da LEDs in Flussrichtung betrieben werden, ist es wichtig, einen Widerstand $R_\text{V}$ zwischen Spannungsquelle $U$ und LED zu schalten. $R_\text{V}$ stellt den erwünschten Strom $I$ ein. Dabei ist die Schwellspannung $U_\text{th}$ der LED zu berücksichtigen:

$ I=\frac{U-U_\text{th}}{R_\text{V}}$

[question:EC514]
[question:EC515]
[question:EC516]

---

In unserem einfachen Modell fließt für negative $U_\text{d}$ nur ein geringer Sperrstrom. Das stimmt aber nicht für sehr negative Spannungen. Irgendwann wird das elektrische Feld über der Verarmungszone zwischen n und p zu hoch und die Diode "bricht durch", der Strom in Rückwärtsrichtung steigt extrem stark an, wie in Abbildung [ref:n_diode_kennlinie_uz] gezeigt.

Dieser *Sperrdurchbruch* kann verschiedene physikalische Ursachen haben, die wir hier nicht im Detail behandeln können. Die Spannung, bei der dieser Durchbruch passiert, wird gemeinhin als *Zener-Spannung* $U_\text{z}$ bezeichnet, auch wenn der Zener-Effekt (ein quantenmechanischer Tunneleffekt) nur ein möglicher Durchbruchmechanismus ist. *Zenerdioden* werden zur Spannungsstabilisierung verwendet. Dabei ist es wichtig, den Durchbruchstrom durch einen Vorwiderstand zu begrenzen. 

<margin>
[picture:862:n_diode_kennlinie_uz:Kennline einer Z-Diode]
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

Die bisher behandelten Dioden waren alle *pn-Dioden*, die Diodeneigenschaft entsteht durch einen Halbleiterübergang. Bei der *Schottky-Diode* handelt es sich um eine Diode, deren Eigenschaften durch einen Metall-Halbleiter-Übergang entstehen. Die Schwellspannung ist etwa halb so groß wie die einer pn-Diode aus dem selben Material, oder kleiner, abhängig von der genauen Gestaltung des Metall-Halbleiter-Übergangs. Schottky-Dioden werden eingesetzt, wenn die Schwellspannung gering sein soll, oder aber als sehr schnelle Schaltdioden.  

[question:EC504]
[question:EC505]

<margin>
Metall-Halbleiter-Dioden sind die ältesten Gleichrichterbauelemente auf Halbleiterbasis. Ferdinand Braun entdeckte ihren Gleichrichtereffekt bereits 1874, ohne aber seine Beobachtung erklären zu können.
</margin>

Fassen wir zusammen:

Dioden lassen Strom nur einer Richtung fließen. Daher eignen sie sich zur Gleichrichtung von Wechselstrom.

Bei hohen Sperrspannungen allerdings ($U_\text{d} < U_\text{z}$), steigt der Strom in Rückwärtsrichtung stark an. Dieser Betriebspunkt kann sehr gut zur Spannungsstabilisierung genutzt werden (*Zenerdiode*).

Daneben lassen sie sich in Sperrrichtung auch als spannungsgesteuerte Kapazitäten verwenden, dies werden wir aber erst in der Ausbildung zur Klasse A behandeln. 

[question:EC502]
[question:EC518]
[question:EC519]
