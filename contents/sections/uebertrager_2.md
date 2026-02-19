% todo Hinweis: Es gibt nur eine einzige Frage zur Stromdichte.
Da alle stromführenden Leitungen nicht zu warm werden dürfen, damit die Isolation nicht schmilzt oder der Leiter gar zu glühen anfängt, darf eine maximale Stromstärke bezogen auf den Leiterquerschnitt nicht überschritten werden.
Bildet man das Verhältnis von Stromstärke bezogen auf den Leiterquerschnitt in $\unit{\milli\meter\square}$, dann erhält man einen Wert für die Stromdichte $S$.
Die Berechnungsformel lautet:
Stromdichte $S = \frac{I}{A} $ in  $\unit{\ampere\per\milli\meter\squared}$

(siehe Formelsammlung Seite 236 Mitte rechts -  Stichwort: Belastbarkeit von Wicklungen)
Nach VDE ist für frei verlegte Leiter aus Kupfer die maximal zulässige Stromstärke mit $\qty{12}{\ampere}$ bei einer Querschnittsfläche von $\qty{0,75}{\milli\meter\squared}$ festgelegt.
Bei Schmelzsicherungen kann die Stromdichte bis zu $\qty{3000}{\ampere\per\milli\meter\squared}$ erreichen.

Bei Transformatoren muss eine maximale Stromdichte von ca. $\qty{2,5}{\ampere\per\milli\meter\squared}$  eingehalten werden, da die Wicklungen die Wärme nicht optimal abstrahlen können.

Zur Berechnung der Stromdichte ist aus dem Drahtdurchmesser die Querschnittsfläche in $\unit{\milli\meter\squared}$ zu ermitteln.
Querschnittsfläche $A = d^2 \cdot \frac{\pi}{4}$
(siehe Formelsammlung Seite 234 Mitte links -  Stichwort: Widerstand von Drähten)

Querschnittsfläche des Drahtes: $A = (\qty{0,5}{\milli\meter})^2 \cdot \frac{3,14}{4} = \qty{0,2}{\milli\meter\squared}$
Die Aufgabe kann nur mit der nach $I$ umgestellten Formel berechnet werden:
Strom $I = S \cdot A = \qty{2,5}{\ampere\per\milli\meter\squared} \cdot \qty{0,2}{\milli\meter\squared} = \qty{0,5}{\ampere}$
[question:AC307]

% todo Der Begriff Gegeninduktion sollte in das Kapitel Trafo 1 verschoben werden.
Das Trafo-Prinzip beruht auf einem besonderen physikalischen Effekt.
Wenn sich ein Magnetfeld in einer Spule ändert, und dies geschieht beim Anlegen einer Wechselspannung, dann wird in einer magnetisch gekoppelten Spule eine elektrische Spannung induziert, die der Ursache entgegengesetzt gerichtet ist. Deshalb spricht man von Gegeninduktion. Auch bei jedem Motor gibt es diesen Effekt, deshalb benötigt man eine Kraft, um den Motor zu drehen. Wäre es keine Gegeninduktion, dann hätten wir ein Perpetuum Mobile, der Motor wird ein Mal angestoßen und läuft dann ohne Kraftzuführung weiter.

Anpassungsübertrager
Transformatoren werden in der Hochfrequenztechnik auch als Anpassungsübertrager eingesetzt.
Dabei besteht der Transformatorkern nicht aus Eisen sondern aus gepresstem Eisen- oder Ferritpulver.
% todo Bild: Ferrit Ringkernübertrager mit Typenbezeichnung und Farbmarkierung
% todo Bild: Eisenpulver Ringkernübertrager mit Typenbezeichnung und Farbmarkierung
Ein Anpassungsübertrager hat die Aufgabe, eine Impedanz an eine andere anzupassen.
Als Beispiel betrachten wir eine endgespeiste Antenne, deren Eingangsimpedanz ca. $\qty{2450}{\ohm}$ beträgt.
Sie soll an einen Sender für $\qty{50}{\ohm}$ Lastimpedanz angepasst werden soll.

Die Berechnung der Impedanzübertragung läßt sich aus den TRAFO-Grundformeln ermitteln.
Die Formel für die Impedanzübertragung lautet:
$ \frac {Z_p}{Z_s}$ = $ü^2$ =$( \frac {N_p}{N_s})^2$ = $( \frac {U_p}{U_s})^2$
Merke: Das Impedanzverhältnis ist das Quadrat des Spannungsverhältnisses und damit auch das Quadrat des Windungszahlenverhältnisses.

oder ü =$ \sqrt \frac {Z_p}{Z_s}$ = $ \frac {N_p}{N_s}$ =  $ \frac {U_p}{U_s}$ = $  \frac {I_s}{I_p}$



% todo Bild: Anpassungsübertrager mit Lastimpedanz Z2

<indepth>
 Ableitung der Formel zur Impedanzübertragung:
 $ P_p$ =$ P_s$
  $U_p$ * $I_p$ = $U_s$ * $I_s$
  Für $U$ das Ohmsche Gestz einsetzen: U = I * R;
  $R$ wird durch $Z$ ersetzt
($I_p$ * $Z_p$) * $I_p$ = ($I_s$ * $Z_s$) * $I_s$
 Das Impedanzverhältmnis auf einer Seite bilden:
 $ \frac {Z_p}{Z_s}$ =$ \frac {{I_s}^2}{{I_p}^2}$ = $ü^2$
  oder
  Für $I$ das Ohmsche Gesetz einsetzen:
  I = $\frac {U}{R}$ 
  $R$ wird durch $Z$ ersetzt
$ \frac {U_p}{Z_p} * U_p$  = $\frac {U_s}{Z_s} * U_s$
 Das Impedanzverhältnis auf einer Seite bilden:
 $ \frac {Z_p}{Z_s}$ =$ \frac {{U_p}^2}{{U_s}^2}$ = $ü^2$
</indepth>
Impedanzübertragung 1 : 49  bedeutet: $ü^2$ =49  ; daraus die Wurzel ergibt ü=7
% todo BILD: UNUN mit EndFED
Beispielrechnung Q1038:

[question:AC301]
[question:AC302]
[question:AC303]
[question:AC304]
[question:AC305]
[question:AC306]

<margin>
Lösungshilfe:

AC 302: $\qty{30}{\milli\ampere}$
AC 303: $\qty{1}{\kilo\ohm}$
AC 304: $\qty{0,4}{\kilo\ohm}$
AC 305: Verhältnis 3 : 1
AC 306: Verhältnis 1 : 7

 *Zusammenfassung*:
 Formelsammlung auf Seite 234
 Querschnittsfläche $A = d^2 \cdot \frac{\pi}{4}$ 
Stromdichte $S = \frac{I}{A} $ 
  
$ \frac {Z_p}{Z_s}$ = $ü^2$ =$( \frac {N_p}{N_s})^2$ = $( \frac {U_p}{U_s})^2$
ü =$ \sqrt \frac {Z_p}{Z_s}$ = $ \frac {N_p}{N_s}$ =  $ \frac {U_p}{U_s}$ = $  \frac {I_s}{I_p}$
  
</margin>