Wichtige Messungen für den Funkamateur an Sendern sind Messungen von Ausgangsleistungen an Sendern oder die Messung von HF-Spannungen in HF-Schaltungsteilen. Bei Messung von Senderausgangsleistungen muss der Sender mit einer definierten Impedanz, die zur Ausgangsimpedanz des Senders passt, abgeschlossen werden. Im Amateurfunk beträgt die übliche Impedanz (Senderabschluss) $\qty{50}{\ohm}$. Der Abschluss kann auch direkt in der Messschaltung erfolgen, was jedoch nur bei kleinen Leistungen sinnvoll ist.

Die Messung von HF-Spannungen erfolgt mittels eines HF-Tastkopfes über Diodengleichrichtung und anschließende Glättung der entstehenden Gleichspannung mit einem nachgeschalteten Kondensator. Abbildung [ref:hf_messkopf_0] zeigt das Prinzip eines HF-Tastkopfes mit einfacher Gleichrichtung und Glättung der Gleichspannung. Die HF-Spannung wird über einen Widerstand (oder eine Kombination aus Widerständen) am Eingang impedanzrichtig abgeschlossen. Anschließend erfolgt die Gleichrichtung mittels Diode, deren Ausgangsspannung sich als Spitzenwert abzüglich der Forward-Spannung der Diode berechnet und im nachgeschalteten Kondensator gepuffert wird. Abbildung [ref:hf_messkopf_1] zeigt einen selbstgebauten HF-Tastkopf, Abbildung [ref:hf_messkopf_2] den Schaltplan dazu.

<margin>
[picture:576:hf_messkopf_0:Prinzip eines HF-Tastkopfes mit einfacher Gleichrichtung und Glättung der Gleichspannung]
[photo:338:hf_messkopf_1:Selbstgebauter HF-Tastkopf von DL3JOP]
[photo:339:hf_messkopf_2:Schaltplan HF-Tastkopf von DL3JOP]
</margin>

[question:AI608]

Bei höheren HF-Leistungen muss ein entsprechend belastbares Dämpfungsglied vorgeschaltet werden, das einen Großteil der Senderausgangsleistung, die gemessen werden soll, aufnimmt. Das Dämpfungsglied ist bei der Berechnung der Leistung zu berücksichtigen.

[question:AI609]

---

Für eine möglichst genaue Messung von HF-Spannungen und -Leistungen muss die verwendete Messschaltung zunächst kalibriert werden. Dazu werden bekannte Referenzsignale eingespeist und die Abweichungen zwischen dem tatsächlichen und dem gemessenen Wert bestimmt. Aus diesen Abweichungen können frequenz- und pegelabhängige Korrekturwerte ermittelt und beispielsweise in einer Tabelle wie in [ref:a_frequenzgang_messwerte] gespeichert werden.

Bei einer späteren Messung wird der angezeigte Messwert mit dem entsprechenden Korrekturwert berichtigt. Werden die Messwerte in $\unit{\dBm}$ angegeben, kann z. B. die bei der Kalibrierung bestimmte Abweichung für die entsprechende Frequenz als Korrekturwert in $\unit{\dB}$ zum Messwert addiert werden.

<margin>
| c: Frequenz in MHz | c: Sendeleistung $\qty{-40}{\dBm}$ | c: Sendeleistung $\qty{-20}{\dBm}$ |
| 10   | $\qty{-40,24}{\dBm}$ | $\qty{-20}{\dBm}$    |
| 50   | $\qty{-40,24}{\dBm}$ | $\qty{-20}{\dBm}$    |
| 100  | $\qty{-40,26}{\dBm}$ | $\qty{-20,12}{\dBm}$ |
| 200  | $\qty{-40,26}{\dBm}$ | $\qty{-20,2}{\dBm}$  |
| 300  | $\qty{-40,51}{\dBm}$ | $\qty{-20,32}{\dBm}$ |
| 400  | $\qty{-40,46}{\dBm}$ | $\qty{-20,28}{\dBm}$ |
| 500  | $\qty{-40,84}{\dBm}$ | $\qty{-20,64}{\dBm}$ |
| 600  | $\qty{-40,7}{\dBm}$  | $\qty{-20,41}{\dBm}$ |
| 700  | $\qty{-40,7}{\dBm}$  | $\qty{-20,53}{\dBm}$ |
| 800  | $\qty{-40,8}{\dBm}$  | $\qty{-20,55}{\dBm}$ |
| 900  | $\qty{-40,37}{\dBm}$ | $\qty{-20,2}{\dBm}$  |
| 1000 | $\qty{-40,33}{\dBm}$ | $\qty{-20,09}{\dBm}$ |
| 1100 | $\qty{-40,12}{\dBm}$ | $\qty{-19,85}{\dBm}$ |
| 1200 | $\qty{-39,94}{\dBm}$ | $\qty{-19,62}{\dBm}$ |
| 1300 | $\qty{-39,69}{\dBm}$ | $\qty{-19,49}{\dBm}$ |
| 1400 | $\qty{-40,18}{\dBm}$ | $\qty{-19,79}{\dBm}$ |
| 1500 | $\qty{-40,13}{\dBm}$ | $\qty{-19,97}{\dBm}$ |
| 1600 | $\qty{-40,95}{\dBm}$ | $\qty{-20,62}{\dBm}$ |
| 1700 | $\qty{-41,55}{\dBm}$ | $\qty{-21,64}{\dBm}$ |
| 1800 | $\qty{-41,47}{\dBm}$ | $\qty{-20,92}{\dBm}$ |
| 1900 | $\qty{-43,1}{\dBm}$  | $\qty{-23,27}{\dBm}$ |
| 2000 | $\qty{-42,34}{\dBm}$ | $\qty{-21,89}{\dBm}$ |
[table:a_frequenzgang_messwerte:Gemessene Pegel in Abhängigkeit von der Frequenz für den HF-Tastkopf von DL3JOP]
</margin>

[question:AI612]

Betrachten wir nun die Berechnung der Schaltungen im Detail. Bei HF-Tastköpfen mit nur einer Diode ist am Messausgang die Spitzenspannung der zugeführten HF-Spannung abzüglich der Forward-Spannung der verwendeten Diode und eines ggf. vorhandenen vorgeschalteten Spannungsteilers messbar. Ein HF-Tastkopf mit einfacher Gleichrichtung und anschließender Glättung wird wie folgt berechnet:

Das HF-Eingangssignal wird durch den vorhandenen Widerstand (oder Kombination aus Einzelwiderständen) am Eingang impedanzrichtig abgeschlossen. In der dargestellten Schaltung (vgl. Abbildung [ref:hf_messkopf_0]) wird die HF-Spannung durch den nachfolgenden Spannungsteiler halbiert (wobei dieser ebenfalls bzgl. der Impedanz wirksam ist). Anschließend erfolgt die Spitzenwert-Gleichrichtung mittels Diode, deren Ausgangsspannung sich als Spitzenwert abzüglich der Forward-Spannung der Diode berechnet und im nachgeschalteten Kondensator gepuffert wird.

---

[question:AI610]

<tip>
Bei allen Schaltungen mit HF-Messköpfen kann man pauschal davon ausgehen, dass der Eingangswiderstand $\qty{50}{\ohm}$ ist. Man muss es nicht nochmal nachrechnen sondern man kann diesen Schritt für die Prüfungsfragen überspringen.
</tip>

Umgekehrt kann aus der gemessenen Gleichspannung die der Schaltung zugeführte Leistung berechnet werden. Probier aus, ob du auf die Lösung kommst!

[question:AI611]

Neben HF-Tastköpfen mit nur einer Diode gibt es Schaltungen mit zwei Dioden. Ihr Vorteil besteht darin, dass sowohl die positive als auch die negative Spitze des HF-Signals erfasst wird. Dadurch steht am Ausgang eine ungefähr doppelt so große Messspannung zur Verfügung wie bei einer einfachen Spitzenwertgleichrichtung. Dies ist insbesondere dann hilfreich, wenn kleine HF-Spannungen mit einem nachgeschalteten Gleichspannungsmessgerät erfasst werden sollen.

[question:AI605]
[question:AI604]

Die positive und die negative Spitze des HF-Signals werden dabei getrennt erfasst und in Kondensatoren gespeichert. Die beiden Spannungen addieren sich am Ausgang. Idealerweise entspricht die Ausgangsspannung damit der Spitze-Spitze-Spannung des HF-Signals:

$U_\mathrm{A} \approx U_\mathrm{SS} = 2\hat U$

In der realen Schaltung müssen zusätzlich die Durchlassspannungen der beiden Dioden berücksichtigt werden. Näherungsweise gilt daher:

$U_\mathrm{A} \approx 2\hat U - 2U_\mathrm{F}$

Soll aus der gemessenen Ausgangsspannung wieder auf die HF-Spannung geschlossen werden, ergibt sich:

$\hat{U} \approx \frac{U_\mathrm{A}+2U_\mathrm{F}}{2}$

Aus dem Spitzenwert kann anschließend der Effektivwert und daraus bei bekanntem Widerstand die HF-Leistung berechnet werden.

[question:AI607]
[question:AI606]

Um anzuzeigen, dass ein Sender über seine Antenne Leistung abstrahlt, kann ein Feldstärkeanzeiger verwendet werden. Hierbei wird über eine Messantenne der Diode die empfangene HF zugeführt und durch die Diode gleichgerichtet. Anschließend wird die gleichgerichtete Spannung über HF-Drosseln einem Kondensator zugeführt, der die gleichgerichtete Spannung puffert. Die Anzeige erfolgt durch ein empfindliches Strommessgerät. Je höher der Zeigerausschlag des Messinstruments ausfällt, desto höher ist die an der Antenne gemessene HF-Feldstärke. Um exakte Messungen vornehmen zu können, muss sowohl die Messantenne als auch der Feldstärkemesser kalibriert werden.

[question:AI613]