Eine Speiseleitung lässt sich als Schaltung vieler kleiner Induktivitäten und Kapazitäten wie in Abbildung [ref:a_wellenwiderstand] darstellen. Aus diesen sogenannten Induktivitätsbelägen $L'$ in $\unit{\henry\per\meter}$ und Kapazitätsbelägen $C'$ in $\unit{\farad\per\meter}$ ergibt sich der Wellenwiderstand $Z$ der Leitung. Allgemein gilt:

$Z_0 = \sqrt{\frac{L'}{C'}}.$

<margin>
[picture:1108:a_wellenwiderstand:Wellenwiderstand einer Speiseleitung]

| X: Eigenschaft               | l: Wert                               |
| Impedanz                     | $\qty{50}{\ohm}$                      |
| Frequenzbereich              | $ < \qty{1}{\giga\hertz}$             |
| Kapazitätsbelag              | $\qty{100}{\pico\farad\per\meter}$    |
| Induktivitätsbelag           | $\qty{0,25}{\micro\henry\per\meter}$  |
| Ausbreitungsgeschwingkeit    | $\qty{0,66}{\percent}$                |
[table:a_rg58:Technische Daten aus einem Datenblatt eines RG-58-Koaxialkabels]
</margin>

Die Tabelle [ref:a_rg58] zeigt die technischen Daten eines RG-58-Koaxialkabels. Der Wellenwiderstand beträgt $\qty{50}{\ohm}$, der Kapazitätsbelag $\qty{100}{\pico\farad\per\meter}$ und der Induktivitätsbelag $\qty{0,25}{\micro\henry\per\meter}$. Aus diesen Werten lässt sich der Wellenwiderstand mit der obigen Formel berechnen:

$Z_0 = \sqrt{\frac{\qty{0,25}{\micro\henry\per\meter}}{\qty{100}{\pico\farad\per\meter}}} = \sqrt{2500} = \qty{50}{\ohm}$

Sind diese Kapazitäts- und Induktivitätsbeläge nicht bekannt, so gibt es Formeln in der Formelsammlung, die auf den geometrischen Abmessungen der Leitung und der relativen Dielektrizitätszahl des Dielektrikums basieren.

Der Wellenwiderstand $Z_0$ einer symmetrischen Zweidrahtleitung hängt z. B. vom Mittenabstand der Leiter ($a$) und deren Durchmesser ($d$), sowie der relativen Dielektrizitätszahl $\epsilon_\mathrm{r}$ des dazwischen befindlichen Dielektrikums, ab. Die in der Formelsammlung angegebene Gleichung gilt für $a/d > 2,5$:

$Z_0 = \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2\cdot a}{d}\right)}$

Hierbei ist $\ln$ der natürliche Logarithmus.

[question:AG305]

Der Wellenwiderstand $Z_0$ einer Koaxialleitung hängt vom Verhältnis des Innendurchmessers des Außenleiters ($D$) zum Durchmesser des Innenleiters ($d$) sowie des dazwischen befindlichen Dielektrikums ab. Der Formelsammlung entnehmen wir:

$Z_0 = \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}$

Hierbei ist $\ln$ der natürliche Logarithmus und $\epsilon_\mathrm{r}$ die relative Dielektrizitätszahl des Dielektrikums.

[question:AG306]
[question:AG307]

Wenn eine Leitung mit ihrem Wellenwiderstand abgeschlossen wird, wenn also an einem Ende ein Bauteil oder eine Antenne angeschlossen wird, die genau denselben Widerstand aufweist, wie der Wellenwiderstand der Leitung, dann spricht man von Anpassung. In diesem Falle werden Wellen an diesem Ende des Kabels nicht reflektiert.

[question:AG304]
