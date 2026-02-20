## Wellenwiderstand einer Zweidrahtleitung

* Der Wellenwiderstand $Z$ hängt vom Verhältnis des doppelten Mittenabstand der Leiter ($a$) und dem Durchmesser der Leiter $d$ sowie vom Dielektrikum ab
* Formel aus der Formelsammlung mit $\epsilon_\mathrm{r}$ als relative Dielektrizitätszahl:

<fragment>
$Z = \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2 \cdot a}{d}\right)}$
</fragment>

---
[question:AG305]
---
#### Lösungsweg
* gegeben: $d = \qty{2}{\milli\meter}$
* gegeben: $a = \qty{20}{\centi\meter}$
* gegeben: $\epsilon_\mathrm{r} \approx 1$ für Luft
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{120}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{2 \cdot a}{d}\right)}\\ &= \dfrac{\qty{120}{\ohm}}{\sqrt{1}} \cdot \ln{\left(\dfrac{2 \cdot \qty{200}{\milli\meter}}{\qty{2}{\milli\meter}}\right)}\\ &\approx \qty{635}{\ohm}\end{split}$
</fragment>
---
## Wellenwiderstand einer Koaxialleitung

* Der Wellenwiderstand $Z$ hängt vom Verhältnis des Innendurchmessers des Außenleiters ($D$) zum Durchmesser des Innenleiters ($d$) sowie vom Dielektrikum ab
* Formel aus der Formelsammlung mit $\epsilon_\mathrm{r}$ als relative Dielektrizitätszahl

<fragment>
$Z = \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\dfrac{D}{d}}$
</fragment>

---
[question:AG306]
----
#### Lösungsweg
* gegeben: $D = \qty{5}{\milli\meter}$
* gegeben: $d = \qty{1}{\milli\meter}$
* gegeben: $\epsilon_\mathrm{r} \approx 1$ für Luft
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}\\ &= \dfrac{\qty{60}{\ohm}}{\sqrt{1}} \cdot \ln{\left(\dfrac{\qty{5}{\milli\meter}}{\qty{1}{\milli\meter}}\right)}\\ &\approx \qty{97}{\ohm}\end{split}$
</fragment>
---
[question:AG307]
---
#### Lösungsweg
* gegeben: $d = \qty{0,7}{\milli\meter}$
* gegeben: $D = \qty{4,4}{\milli\meter}$
* gegeben: $\epsilon_\mathrm{r} = 2,29$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{\qty{60}{\ohm}}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\left(\dfrac{D}{d}\right)}\\ &= \dfrac{\qty{60}{\ohm}}{\sqrt{2,29}} \cdot \ln{\left(\dfrac{\qty{4,4}{\milli\meter}}{\qty{0,7}{\milli\meter}}\right)}\\ &\approx \qty{75}{\ohm}\end{split}$
</fragment>
---
### Anpassung von Koaxialleitungen

* Wird ein Bauteil oder eine Antenne angeschlossen, die exakt den Wellenwiderstand der Leitung aufweist, spricht man von Anpassung
* Bei Anpassung werden Wellen am Abschluss nicht zurückreflektiert

---
[question:AG304]