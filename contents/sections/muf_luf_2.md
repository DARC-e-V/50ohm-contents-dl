Die *MUF* (*maximum usable frequency*), also die höchste Frequenz, die die Ionosphäre für die Distanz zwischen Sender und Empfänger noch zurückbrechen kann, haben wir bereits in der Klasse E kennengelernt. Dort wurde deutlich, dass die MUF von der Dichte der freien Elektronen in der brechenden Region abhängt. In der Klasse A werden wir dieses Thema nun insbesondere mit Blick auf den Abstrahlwinkel noch genauer betrachten.

[question:AH206]
[question:AH207]

Wie wir auch schon wissen, ist die Reichweite der Raumwellen vom Abstrahlwinkel abhängig. Je flacher die Welle auf die Ionosphäre auftrifft, desto leichter erfolgt die Berechnung. Dieser Zusammenhang gilt auch für die MUF: Die gerade noch zurückgebrochene Frequenz, die *MUF*, ist umso höher, je flacher unser Signal in die Ionosphäre einfällt. Die Abbildung [ref:e_muf_winkel2] zeigt eine Simulation der Sprungdistanz für einen Sommertag im Jahr 2024 für ein Amateurfunksignal um die $\qty{7}{\mega\hertz}$. Bei $\qty{45}{\degree}$ lag die MUF an diesem Tag bei $\qty{7,5}{\mega\hertz}$. Ändert man den Abstrahlwinkel, verändert sich auch die MUF: Strahlt man steiler ab (z. B. $\qty{60}{\degree}$), sinkt die MUF und die Funkwelle wird nicht mehr refraktiert. Strahlt man hingegen flacher ab (z. B. $\qty{30}{\degree}$), so erhöht sich die MUF. Im Folgenden werden wir diesen Zusammenhang genauer betrachten.

<margin>
[picture:998:e_muf_winkel2:Sprungdistanz bei 7 MHz im Sommer 2024]
</margin>

---

Von Ionosphärenmessstationen wird die so genannte kritische Frequenz $f_\text{c}$ (oder oft auch $f_\text{k}$, $f_\text{krit}$ oder $f_\text{oF2}$) gemessen. Das ist die höchste Frequenz, bei der die senkrecht in die Ionosphäre eintretende Raumwelle gerade noch reflektiert wird (Vgl. Abbildung [ref:e_muf_winkel]). Wenn wir senkrecht nach oben strahlen, unser Signal also unter einem Winkel von $\qty{90}{\degree}$ in die Ionosphäre einfällt, ist die MUF am kleinsten, denn unser Signal muss dann ja in der Ionosphäre komplett "umkehren", also eine 180° Wendung vollführen. Das bedeutet, bei $\qty{90}{\degree}$ gilt $f_\text{c} = MUF$. 

<indepth>
Als Formelzeichen verwendet man $f_o$ (kleiner tiefgestellter Buchstabe "O" für *ordinary wave*) gefolgt von der ionosphärischen Region, für die diese Frequenz gilt, also z.B. $f_\text{oF2}$ für die F2-Region. Allerdings wird auch oft $f_\text{c}$, $f_\text{k}$ oder $f_\text{krit}$ als Formelzeichen verwendet.
</indepth>

<margin>
[picture:870:e_muf_winkel:Die Winkel zur Berechnung der MUF]
</margin>

<indepth>
Die kritische Frequenz ist also die höchste Frequenz, die aus der Ionosphäre wieder zurückkommt, wenn man senkrecht nach oben strahlt. Eine Daumenregel besagt, dass die höchste Frequenz, die bei *flacher* Einstrahlung noch zurückgeworfen wird, etwa das Dreifache der kritischen Frequenz beträgt.
</indepth>

[question:AH204]
[question:AH205]

---

Die Abbildung [ref:e_muf_fof2] zeigt den zeitlichen Verlauf von MUF und $f_\text{c}$ am 08.09.2025, gemessen mit der Ionosonde in Juliusruh. MUF $\qty{3000}{\kilo\meter}$ bedeutet in diesem Fall, dass sehr flach abgestrahlt wird, um eine Sprungdistanz von $\qty{3000}{\kilo\meter}$ zu erreichen.

<margin>
[picture:999:e_muf_fof2:MUF und $f_\text{c}$ am 08.09.2025]
</margin>

Für andere Abstrahlwinkel lässt sich die MUF aus der $f_\text{c}$ mithilfe der folgenden Formel aus der Formelsammlung näherungsweise bestimmen (gilt für $\alpha > \qty{40}{\degree}$):

$MUF \approx \frac{f_\text{c}}{sin(\alpha)}$

wobei $\alpha$ den Abstrahlwinkel bezeichnet (vgl. Abbildung [ref:e_muf_winkel]). Schaut man sich die Formel genauer an, erkennt man, dass die MUF stets höher liegt als die kritische Frequenz – und zwar umso mehr, je flacher die Sendeantenne abstrahlt bzw. die Empfangsantenne aufnimmt.

[question:AH208]

---

Für die kommerzielle Frequenzplanung, wo es darauf ankommt, dass eine Funkverbindung mit hoher Wahrscheinlichkeit gelingt, gibt es zudem den Begriff der *FOT* (*frequency of optimal transmission*, optimale Sendefrequenz), oder auch $f_\text{opt}$. Das ist die Frequenz, die auf einem bestimmten Signalweg statistisch an 90% aller Tage eine Funkverbindung erlaubt; sie liegt üblcherweise 15% unter dem monatlichen Mittel der MUF. In der Formelsammllung finden wir diesen Zusammenhang als 

$f_\text{OPT} = MUF \cdot 0,85$

Mit diesen Informationen können wir nun die folgende Aufgabe lösen; ein Taschenrechner ist dabei hilfreich.

[question:AH209]

<indepth>
Für DX Verbindungen im Amateurfunk spielt die $f_\text{opt}$ keine Rolle, denn dort wählt man in der Regel das höchste Frequenzband, das noch eine Verbindung erlaubt (also am nächsten an der MUF), da dort der geringste Rauschflur und damit das beste Signal zu erwarten ist (höchster Signal-/Rauschabstand SNR).
</indepth>

In der Klasse E haben wir bereits die LUF (Lowest Usable Frequency) kennengelernt. Sie wird von der D-Region bestimmt und bezeichnet die niedrigste nutzbare Frequenz, unterhalb derer die Dämpfung zu stark ist. Die D-Region *dämpft* ja unser Funksignal und pro Sprung muss dieses Signal auch noch *zwei* Mal durch diese D-Region hindurch. Gleichzeitig ist diese Dämpfung umso höher, je niedriger die Frequenz ist (der Zusammenhang ist quadratisch: halbiert man die Frequenz, vervierfacht sich die Dämpfung). Daher wird man, wenn man die Frequenz fortwährend verringert, ebenfalls irgendwann an den Punkt gelangen, wo das zurückgebrochene Signal nicht mehr nutzbar ist; das ist die LUF.

[question:AH210]
[question:AH211]
