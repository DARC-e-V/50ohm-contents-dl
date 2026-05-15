Sinusförmige Wechselspannungen ändern ihren Wert fortlaufend. Um sie besser beschreiben zu können, wollen wir uns im Folgenden drei wichtige Kenngrößen ansehen:

1. $\hat{U}$: Den Spitzenwert eine Wechselspannung
2. $U_\text{SS}$: der Spitze-Spitze-Wert 
3. $U_\text{eff}$: der Effektivwert

<margin>
[picture:834:e_wechselspannung_kenngroessen:Die drei Kenngrößen einer Wechselspannung]
</margin>

---

Der *Spitzenwert* einer Wechselspannung $\hat{U}$ entspricht der Amplitude, die wir bereits in der Klasse N kennengelernt haben (vgl. Abbildung [ref:e_wechselspannung_kenngroessen]). Er ist unter anderem wichtig für die Spannungsfestigkeit von Kondensatoren. Abbildung [ref:e_spannungsfestigkeit_elkos] zeigt zwei bedrahtete Elektrolytkondensatoren, auf denen die zulässige Spannungsfestigkeit aufgedruckt ist. Der Spitzenwert der anliegenden Spannung darf diesen Grenzwert nicht überschreiten, da sonst die Zerstörung des Kondensators droht. Häufig wählt man Bauteile mit einer höheren Spannungsfestigkeit als erforderlich – entweder aus Sicherheitsgründen oder zur Verlängerung der Lebensdauer.

<margin>
[photo:198:e_spannungsfestigkeit_elkos:Elektrolytkondensatoren mit den Spannungsfestigkeiten 16 Volt und 25 Volt]
</margin>

Eine weitere Kenngröße ist der *Spitze-Spitze-Wert*. Das ist der Unterschied zwischen dem höchsten und dem niedrigsten Ausschlag. Für Sinusförmige Wechselspannungen gilt:

$U_\text{SS} = 2\cdot \hat{U}$.
 
[question:EB406]
[question:EB407]

Wenn nicht die Spannungs-, sondern die Leistung von Geräten oder die Wärmebelastung von Bauteilen und Leitungen im Vordergrund steht, ist der Spitzenwert nicht hilfreich. Für diesen Fall hat man den *Effektivwert* definiert. Der Effektivwert einer Wechselspannung entspricht dem Wert einer Gleichspannung, die einen ohmschen Widerstand genauso stark erwärmen würde. 

---

Bei sinusförmigen Spannungen ist der Spitzen- oder Scheitelwert etwa 1,4-mal so groß wie der Effektivwert (siehe Abbildung [ref:e_wechselspannung_kenngroessen]). Die genaue Rechnung führt zu einer einfachen Formel:

$U_\text{eff} = \frac{\hat{U}}{\sqrt{2}}$ oder $\hat{U} = U_\text{eff} \cdot \sqrt{2}$

Wird eine Wechselspannung nur mit dem Buchstaben $U$ ohne Zusatz angegeben, ist in der Regel der Effektivwert gemeint. Das bekannteste Beispiel ist unsere Netzspannung von $\qty{230}{\volt}$ – auch hierbei handelt es sich um den Effektivwert. Die Spitzenspannung liegt deutlich höher, nämlich bei

$\hat{U} = \qty{230}{\volt} \cdot \sqrt{2} \approx \qty{325}{\volt}$.

<indepth>
Die genaue Herleitung dieser Formel erfolgt mithilfe der Integralrechnung und geht über das für die Amateurfunkprüfung erforderliche Wissen hinaus. Wer mit der Integralrechnung vertraut ist und sich dafür interessiert, kann die Herleitung hier nachlesen: [Wikipedia](https://50ohm.de/ew)
</indepth>

[question:EB401]

Der Wert für $U_\text{SS}$ ergibt für die Netzspannung dann das Doppelte des Spitzenwerts: 

$ U_\text{SS} = 2 \cdot \qty{230}{\volt} \cdot \sqrt{2} \approx \qty{651}{\volt}$

[question:EB402]

Nach dem gleichen Prinzip funktionieren auch die beiden folgenden Fragen: 

[question:EB403]
[question:EB404]

---

% TODO referenz auf das Leistungskapitel einfügen:

Bei der nächsten Frage wird indirekt nach dem Effektivwert der Spannung gefragt. Wenn man weiß, das $\frac{1}{\sqrt{2}} \approx 0,7$ ist kann man die beiden Ergebnisse direkt ablesen. 

<indepth>
Wichtig ist, dass sowohl die Gleichspannung $\qty{0,7}{\volt}$ als auch die Gleichspannung $\qty{-0,7}{\volt}$ zum gleichen Ergebnis führen. Das liegt daran, dass sich bei einer negativen Spannung auch das Vorzeichen des Stroms ändert, was jedoch trotzdem zur gleichen Leistung führt – denn es gilt $P = U \cdot I$.
</indepth>

[question:EB405]

Übrigens: Alles hier über Wechselspannungen Geschriebene gilt analog für Wechselströme.