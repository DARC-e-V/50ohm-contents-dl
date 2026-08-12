---

### Symbol
* Ein *Symbol* ist ein unterscheidbarer Signalzustand.
* Symbole können sich z. B. durch Amplitude, Frequenz oder Phase unterscheiden.
* Mehr mögliche Symbole ermöglichen mehr Bits pro Symbol.

---

### Symbolrate
* Die *Symbolrate* gibt die Anzahl der übertragenen Symbole pro Sekunde an, die Einheit der Symbolrate ist *Baud*
* Datenrate und Symbolrate sind daher nicht immer identisch.
* Werden nur zwei Symbole verwendet und somit jedes Bit einzeln gesendet, entspricht die Symbolrate in Baud der Datenrate in $\unit{\bit\per\second}$.
* Werden jedoch mehr Symbole verwendet und somit mehrere Bits gleichzeitig übertragen, ist die Datenrate höher als die Symbolrate.

---

**Beispiele**

* 2 Symbole → 1 Bit/Symbol
* 4 Symbole → 2 Bit/Symbol
* 8 Symbole → 3 Bit/Symbol

---

* Die Formel $R_\mathrm{D} = R_\mathrm{S} \cdot N$ stellt den Zusammenhang dar:

<fragment>
* $R_\mathrm{D}$ → Datenübertragungsrate in $\unit{\bit\per\second}$
* $R_\mathrm{S}$ → Symbolrate in $\unit{\baud}$
* $N$ → Symbolgröße in $\unit{\bit\per\text{Symbol}}$
</fragment>

---

[question:AA104]

---

Beispiele:

<fragment>
*RTTY*: Umschaltung zwischen zwei Symbolfrequenzen, sodass pro Symbol ein Bit ($\num{0}$ oder $\num{1}$) übertragen werden kann.
→ Datenrate = Symbolrate
</fragment>

<fragment>
*FT4*: Umschaltung zwischen vier Symbolfrequenzen, so dass pro Symbol zwei Bit ($\num{00}$, $\num{01}$, $\num{10}$ oder $\num{11}$) übertragen werden können.
→ Datenrate = 2 $\cdot$ Symbolrate
</fragment>

---

[question:AE405]

---

#### Lösungsweg
* gegeben: $R_S = \qty{45,45}{\baud}$
* gegeben: $N=\qty{1}{\bit\per\text{Symbol}}$
* gesucht: $R_\mathrm{D}$

<fragment>
$R_\mathrm{D} = R_\mathrm{S} \cdot N = \qty{45,45}{\baud} \cdot \qty{1}{\bit\per\text{Symbol}} = \qty{45,45}{\bit\per\second}$
</fragment>

---

[question:AE406]

---

#### Lösungsweg
* gegeben: $R_S = \qty{23,4}{\baud}$
* gegeben: $N=\qty{2}{\bit\per\text{Symbol}}$
* gesucht: $R_\mathrm{D}$

<fragment>
$R_\mathrm{D} = R_\mathrm{S} \cdot N = \qty{23,4}{\baud} \cdot \qty{2}{\bit\per\text{Symbol}} = \qty{46,8}{\bit\per\second}$
</fragment>