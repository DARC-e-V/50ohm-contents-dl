Durch den geringen Aufwand ist der Brückengleichrichter eine häufig verwendete Gleichrichterschaltung. Dazu benötigt man einen Trafo und 4 Dioden. In der Abbildung [ref:a_brueckenlgeichrichter] ist ein solcher Brückengleichrichter dargestellt.

<margin>
[picture:965:a_brueckenlgeichrichter:Brückengleichrichter]
</margin>

---

In dem nebenstehenden Applet kann man bei dargestellter Polarität der Trafospannung $U_\text{a}$ bzw. $U_\text{s}$ den Laststrom in seinem Stromverlauf verfolgen und erkennen, dass der dieser stets in gleicher Richtung durch den Lastwiderstand $R$ fließt. Der Spannungsabfall am Lastwiderstand $R_\text{L}$ ist eine pulsierende Gleichspannung (DC), die aus positiven sinusförmigen Halbwellen besteht. Diese Spannung hat eine Frequenz $f=\qty{100}{\hertz}$.

<margin>
[include:applet_gleichrichter_2]
</margin>

---

<margin>
[photo:296: Brückengleichrichter Bauformen: Bauformen von Brückengleichrichtern]
Die Beschriftung der Anschlüsse ist zu beachten.

  1. Hochstrom-Brückengleichrichter 26 MB 20 A ($\qty{200}{\volt}$, $\qty{25}{\ampere}$) im Metallgehäuse zur direkten Montage auf einem Kühlkörper
  2. B80 C 5000/3300 bedeutet: maximal $\qty{80}{\volt}$ Betriebsspannung, C kapazitive Last max. $\qty{2500}{\micro\farad}$ mit Schutzwiderstand $R = \qty{1}{\ohm}$, maximaler Dauerlaststrom: $\qty{5000}{\milli\ampere}$ mit Kühlkörper, $\qty{3300}{\milli\ampere}$ ohne Kühlkörper
  3. BY 225 Brückengleichrichter - besonderes Gehäuse
  4. runde Bauform eines Brückengleichrichters B 80 C 1000
  5. B40 C 1500 - die veränderte Anschlussfolge ist zu beachten
  6. FPU 4M ($\qty{1000}{\volt}$, $\qty{4}{\ampere}$)
  7. im Kunststoff eingeprägte Anschlussfolge
</margin>

[question:AD305]

---
% TODO Frage 1180 ggf. bei Restwelligkeit behandeln

Wenn man nach dem Brückengleichrichter einen Ladekondensator $C_\text{L}$ und ein LC-Siebglied (vgl. Abbildung [ref:a_netzteil_Ucs]) verbaut, erreicht man damit eine kleinere Amplitude in der pulsierenden Ausgangsgleichspannung. Somit haben wir ein konventionelles Netzteil. 

% TODO Schaltungsbild einfügen
<margin>
[picture:66:a_netzteil_Ucs:Gleichrichterschaltung mit Siebung]
</margin>

Um jetzt die Spannung am Siebkondensator $C_\text{S}$ zu bestimmen, sollten wir wissen, dass die Kondensatoren sich auf die Spitzenspannung $\hat{U}$ der Sekundärspannung $U_{\mathrm{sek}}$ des Trafos aufladen.

$\hat{U}=U_{\mathrm{eff}}\cdot\sqrt{2}$

Weiterhin müssen wir beachten, ob der Trafo ein Übersetzungsverhältnis $ü$ aufweist. In unserem Beispiel hat der Trafo $ü = \frac{8}{1}$ und somit können wir mit der Formel $\frac{8}{1} = \frac{U_{\mathrm{prim}}}{U_{\mathrm{sek}}}$ nach $U_{\mathrm{sek}}$ umstellen. Wir kommen somit auf folgende Gleichung:
$U_{\mathrm{sek}} = \frac{U_{\mathrm{prim}}}{8} = \frac{U_{\mathrm{eff}} \cdot \sqrt{2}}{8} = \frac{\qty{230}{\volt} \cdot 1,414}{8} = \frac{\qty{325,22}{\volt}}{8} = \qty{40,65}{\volt}$

% Anmerkung DC4LW 2024-05-29: Muss die Diodenspannung nicht auch noch von $U_{\mathrm{sek}}$ abgezogen werden? Ergänzung: Habe erfahren, dass bei Leerlauf die Diodenspannung vernachlässigt werden kann.

[question:AD306]
