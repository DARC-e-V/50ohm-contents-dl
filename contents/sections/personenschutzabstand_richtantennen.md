Bei der Berechnung von Sicherheitsabständen spielt die Winkeldämpfung bei Richtantennen eine wichtige Rolle. Die größte Strahlungsleistung wird in der Mitte der Strahlungskeule abgestrahlt. In den anderen Richtungen ist sie geringer. Ist die Antenne ausreichend hoch, stahlt die Antenne zum großen Teil über den <u>nicht</u> kontrollierbaren Bereich hinweg, also dem Bereich in dem die Grenzwerte unbedingt eingehalten werden müssen. 

Im kritischen Winkel von $\qty{40}{\degree}$ unterhalb der Antenne befindet sich ein nicht kontrollierbarer Bereich. Die Strahlungsleistung ist dort um $\qty{6}{\dB}$ niedriger als in der Mitte des Strahlungsdiagramms. Die direkte Folge ist, dass dort der Sicherheitsabstand entsprechend geringer sein kann.

$\qty{6}{\dB}$ entsprechen einem Faktor von $\num{0,25}$ oder $\dfrac{1}{4}$ (Formelsammlung).

$ E = \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_\textrm{EIRP}}}{d}$
Umstellen der Formel nach $d$ (Sicherheitsabstand).
$ d = \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_\textrm{EIRP}}}{E}$

Die Strahlungsleistung $P_\textrm{EIRP}$ ist nicht bekannt. Allerdings wissen wir, dass bei dieser Rechnung nur ein Viertel der Strahlungsleistung im Vergleich zur maximalen Strahlungleistung ansetzen müssen.

$\begin{split} d &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_\textrm{EIRP}\cdot \dfrac{1}{4}}}{E}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_\textrm{EIRP}}}{E}\cdot \sqrt{\dfrac{1}{4}}\\ d &= \dfrac{\sqrt{\qty{30}{\ohm}\cdot P_\textrm{EIRP}}}{E}\cdot \mathbf{\dfrac{1}{2}}\end{split}$

Wird die Strahlungsleistung auf $\dfrac{1}{4}$ reduziert halbiert sich der Sicherheitsabstand von $\qty{20}{\meter}$ auf die Hälfte. Er verringert sich auf $\qty{10}{\meter}$.

[question:AK105]

<margin>
[picture:950:a_richtantenne_personenschutz:In einem Winkel von 40° unterhalb der Achse der Hauptstrahlungskeule ist die Strahlungsleistung 6 dB geringer als bei dem Winkel 0°.]
</margin>