<left>
[photo:299:StepUpDownWandler: Abwärts- (Buck) Aufwärts- (Boost) Wandler]
</left>
<right>
* Wandelt Gleichspannungen um &rarr; DC/DC-Wandler
* z.B. von 13,8 V auf 5 V &rarr; Step-DOWN (Tiefsetzsteller)
* z.B. von 12 V auf 19 V &rarr; Step-UP (Hochsetzsteller)
</right>
<note>
Der Buck-Boost Converter im Bild kann von 0,5 V bis 25 V am Ausgang eingestellt werden. Die maximale Leistung beträgt 25 W.
</note>
---
### Wirkungsgrad

* Es entstehen Verluste durch die Bauteile in der Schaltung
* Wirkungsgrad $\eta$, meistens in $\%$ angegeben

<fragment>
$\eta = \frac{P_{\textrm{AB}}}{P_{\textrm{ZU}}}$
</fragment>

---
[question:AB213]
---
#### Lösungsweg
* gegeben: $U_{\textrm{ZU}} = 12V$
* gegeben: $U_{\textrm{AB}} = 5V$
* gegeben: $I_{\textrm{ZU}} = 2A$
* gegeben: $I_{\textrm{AB}} =3A$
* gesucht: $\eta$

<fragment>
$\begin{split} \eta &= \frac{P_{\textrm{AB}}}{P_{\textrm{ZU}}} = \frac{U_{\textrm{AB}} \cdot I_{\textrm{AB}}}{U_{\textrm{ZU}} \cdot I_{\textrm{ZU}}}\\ &= \frac{5V \cdot 3A}{12V \cdot 2A} = \frac{15W}{24W} = 0,625 = 62,5\% \end{split}$
</fragment>
---
[question:AB214]
---
* gegeben: $U_{\textrm{ZU}} = 5V$
* gegeben: $U_{\textrm{AB}} = 12V$
* gegeben: $I_{\textrm{ZU}} = 3A$
* gegeben: $I_{\textrm{AB}} =1A$
* gesucht: $\eta$

<fragment>
$\begin{split} \eta &= \frac{P_{\textrm{AB}}}{P_{\textrm{ZU}}} = \frac{U_{\textrm{AB}} \cdot I_{\textrm{AB}}}{U_{\textrm{ZU}} \cdot I_{\textrm{ZU}}}\\ &= \frac{12V \cdot 1A}{5V \cdot 3A} = \frac{12W}{15W} = 0,8 = 80\% \end{split}$
</fragment>