## Wellenwiderstand einer Zweidrahtleitung

* Der Wellenwiderstand $Z$ hängt vom Verhältnis des doppelten Mittenabstand der Leiter ($a$) und dem Durchmesser der Leiter $d$ sowie vom Dielektrikum ab
* Formel aus der Formelsammlung mit $\epsilon_\mathrm{r}$ als relative Dielektrizitätszahl:

<fragment>
$Z = \dfrac{120Ω}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{(\dfrac{2 \cdot a}{d})}$
</fragment>

---
[question:AG305]
---
#### Lösungsweg
* gegeben: $d = 2mm$
* gegeben: $a = 20cm$
* gegeben: $\epsilon_\mathrm{r} \approx 1$ für Luft
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{120Ω}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{(\dfrac{2 \cdot a}{d})}\\ &= \dfrac{120Ω}{\sqrt{1}} \cdot \ln{(\dfrac{2 \cdot 200mm}{2mm})}\\ &\approx 635Ω\end{split}$
</fragment>
---
## Wellenwiderstand einer Koaxialleitung

* Der Wellenwiderstand $Z$ hängt vom Verhältnis des Innendurchmessers des Außenleiters ($D$) zum Durchmesser des Innenleiters ($d$) sowie vom Dielektrikum ab
* Formel aus der Formelsammlung mit $\epsilon_\mathrm{r}$ als relative Dielektrizitätszahl

<fragment>
$Z = \dfrac{60Ω}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{\dfrac{D}{d}}$
</fragment>

---
[question:AG306]
----
#### Lösungsweg
* gegeben: $D = 5mm$
* gegeben: $d = 1mm$
* gegeben: $\epsilon_\mathrm{r} \approx 1$ für Luft
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{60Ω}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{(\dfrac{D}{d})}\\ &= \dfrac{60Ω}{\sqrt{1}} \cdot \ln{(\dfrac{5mm}{1mm})}\\ &\approx 97Ω\end{split}$
</fragment>
---
[question:AG307]
---
#### Lösungsweg
* gegeben: $d = 0,7mm$
* gegeben: $D = 4,4mm$
* gegeben: $\epsilon_\mathrm{r} = 2,29$
* gesucht: $Z$

<fragment>
$\begin{split}Z &= \dfrac{60Ω}{\sqrt{\epsilon_\mathrm{r}}} \cdot \ln{(\dfrac{D}{d})}\\ &= \dfrac{60Ω}{\sqrt{2,29}} \cdot \ln{(\dfrac{4,4mm}{0,7mm})}\\ &\approx 75Ω\end{split}$
</fragment>
---
### Anpassung von Koaxialleitungen

* Wird ein Bauteil oder eine Antenne angeschlossen, die exakt den Wellenwiderstand der Leitung aufweist, spricht man von Anpassung
* Bei Anpassung werden Wellen am Abschluss nicht zurückreflektiert

---
[question:AG304]