## Messungen für Funkamateure

* Wichtige Messungen: Ausgangsleistung und HF-Spannungen
* Messung der Senderausgangsleistung erfordert definierten Abschluss
* Übliche Impedanz im Amateurfunk: 50 Ohm
* Direktes Messen in der Schaltung nur bei kleinen Leistungen sinnvoll

---
## HF-Spannungsmessung

* HF-Spannung wird mit einem HF-Tastkopf gemessen
* Diodengleichrichtung und Glättung mit nachgeschaltetem Kondensator

---
### HF-Tastkopf mit einfacher Gleichrichtung



<left>
[picture:576:a_messung_hf_tastkopf_leistungsmessung:Messkopf zur HF-Leistungsmessung über einen Spannungsteiler]
</left>
<right>
* Eine Diode am Ausgang liefert die Spitzenspannung der HF-Spannung
* Abzüglich Forward-Spannung der Diode und evtl. Spannungsteiler
</right>

---
[question:AI608]

---
### HF-Tastkopf mit doppelter Gleichrichtung

<left>
[picture:770:a_messung_hf_tastkopf_doppeldiode:HF-Tastkopf mit zwei Dioden für beide Halbwellen]
</left>
<right>
* Zwei Dioden zur Erhöhung der Messgenauigkeit, insbesondere bei kleinen Leistungen
* Beide Halbwellen werden gleichgerichtet
* Ergebnis: Doppelte Spitzenspannung abzüglich zweimal der Forward-Spannung der Dioden
</right>

---
[question:AI605]

---
[question:AI604]

---
### Messen hoher HF-Leistungen

* Erfordert belastbares Dämpfungsglied
* Nimmt einen Großteil der Leistung auf
* Dämpfungsglied muss in die Berechnung einbezogen werden

---
[question:AI609]

<note>
Keine Berechnung notwendig, da es nur eine Antwort mit Dämpfungsglied gibt
</note>

---
## Kalibrierung von Messschaltungen

* Notwendig für exakte Leistungsmessungen
* Korrekturwerte müssen erstellt werden

---
[question:AI612]

---
### Berechnung eines HF-Tastkopfes

<left>
[picture:576:a_messung_messschaltung_beispiel_1:Beispiel einer HF-Messschaltung]
</left>
<right>
* Eingangssignal wird impedanzrichtig abgeschlossen
* Spannung wird durch Spannungsteiler halbiert
* Nach Gleichrichtung durch Diode verbleibt die Spitzenspannung abzüglich Forward-Spannung
</right>

---
[question:AI610]

--- style="font-size: smaller;"
#### Lösungsweg

* gegeben: $P_E = 1W$
* gegeben: $U_F = 0,23V$
* gegeben: $R_V = 110Ω$, $R_T = 330Ω$
* gesucht: $U_A$


<fragment>
$\begin{split}R &= (\frac{1}{R_T + R_T} + \frac{1}{R_V} + \frac{1}{R_V})^{-1}\\ &= (\frac{1}{330Ω + 330Ω} + \frac{1}{110Ω} + \frac{1}{110Ω})^{-1}\\ &= 50,77Ω\end{split}$
</fragment>

--- style="font-size: smaller;"
* gegeben: $P_E = 1W$
* gegeben: $U_F = 0,23V$
* berechnet: $R = 50,77Ω$
* gesucht: $U_A$

<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ \Rightarrow U_{E,eff} &= \sqrt{P_E \cdot R}\\ &= \sqrt{1W \cdot 50,77Ω}\\ &= 7,125V\end{split}$
</fragment>

--- style="font-size: smaller;"
* gegeben: $U_F = 0,23V$
* berechnet: $U_{E,eff} = 7,125V$
* gesucht: $U_A$

<left>
<fragment>
$\begin{split}U_S &= U_{E,eff} \cdot \sqrt{2}\\ &= 7,071V \cdot 1,414\\ &= 10,07V\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_A &= \frac{U_S}{2}\,-\,U_F\\ &= \frac{10,07V}{2}\,-\,0,23V\\ &= 5,035V\,-\,0,23V\\ &= 4,805V \approx 4,8V\end{split}$
</fragment>
</right>

---
### Berechnung der Eingangsleistung aus gemessener Gleichspannung

<left>
[picture:577:a_messung_messschaltung_beispiel_2:Beispiel einer HF-Messschaltung]
</left>
<right>
* Spannung am Spannungsteiler entspricht der Ausgangsspannung zzgl. der Diodenspannung
* Effektivwerte berechnen
* Ermittlung der Eingangsleistung über den Schaltungswiderstand
</right>

---
[question:AI611]

--- style="font-size: smaller;"
#### Lösungsweg
* gegeben: $U_A = 14,9V DC$
* gegeben: $U_F = 0,7V$
* gegeben: $R_1 = 54,1Ω$, $R_T = 330Ω$
* gesucht: $P_E$

<left>
<fragment>
$\begin{split}R &= (\frac{1}{R_T + R_T} + \frac{1}{R_1})^{-1}\\ &= (\frac{1}{330Ω + 330Ω} + \frac{1}{54,1Ω})^{-1}\\ &= 50Ω\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_S &= (U_A + U_F) \cdot 2\\ &= (14,9V + 0,7V) \cdot 2\\ &= 31,2V\end{split}$
</fragment>
</right>

--- style="font-size: smaller;"
<left>
* berechnet: $R = 50Ω$
* berechnet: $U_S = 31,2V$
* gesucht: $P_E$

<fragment>
$\begin{split}U_{E,eff}\\ &= \frac{U_S}{\sqrt{2}}\\ &= \frac{31,2V}{1,414}\\ &= 22,06V\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ &= \frac{(22,06V)^2}{50Ω}\\ &\approx 9,7W\end{split}$
</fragment>
</right>

---
### HF-Tastkopf mit doppelter Spitzenwertgleichrichtung

<left>
[picture:771:a_messung_hf_tastkopf_doppeldiode_2:HF-Tastkopf mit doppelter Spitzenwertgleichrichtung]
</left>
<right>
* Berechnung wie bei einfacher Gleichrichtung
* Zusätzliche Berücksichtigung der doppelten Spitzenspannung
* Doppelte Forward-Spannung der Dioden beachten
</right>

---
[question:AI607]

--- style="font-size: smaller;"
#### Lösungsweg

* gegeben: $U_A = 15,3V DC$
* gegeben: $U_F = 0,23V$
* gegeben: $R_{V1} = 56Ω$, $R_{V2} = 470Ω$
* gesucht: $P_E$

<left>
<fragment>
$\begin{split}R &= (\frac{1}{R_{V1}} + \frac{1}{R_{V2}})^{-1}\\ &= (\frac{1}{R_{56Ω}} + \frac{1}{R_{470Ω}})^{-1}\\ &= 50,04Ω\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_S &= \frac{U_A}{2} + U_F\\ &= \frac{15,3V}{2} + 0,23V\\ &= 7,88V\end{split}$
</fragment>
</right>

--- style="font-size: smaller;"
<left>
* berechnet: $R = 50,04Ω$
* berechnet: $U_S = 7,88V$
* gesucht: $P_E$

<fragment>
$\begin{split}U_{E,eff} &= \frac{U_S}{\sqrt{2}}\\ &= \frac{7,88V}{1,414}\\ &= 5,57V\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}P_E &= \frac{U_{E,eff}^2}{R}\\ &= \frac{{5,57V}^2}{50,04Ω}\\ &\approx 600mW\end{split}$
</fragment>
</right>

---
[question:AI606]

--- style="font-size: smaller;"
#### Lösungsweg

* gegeben: $U_A = 15,3V DC$
* gegeben: $U_F = 0,23V$
* gegeben: $R = 50Ω$ aus dem Messsystem
* gesucht: $P_E$

<left>
<fragment>
$\begin{split}U_S &= \frac{U_A}{2} + U_F\\ &= \frac{15,3V}{2} + 0,23V\\ &= 7,88V\end{split}$
</fragment>
</left>
<right>
<fragment>
$\begin{split}U_{E,eff} &= \frac{U_S}{\sqrt{2}}\\ &= \frac{7,88V}{1,414}\\ &= 5,57V\end{split}$
</fragment>
</right>
  
--- style="font-size: smaller;"
* berechnet: $U_{E,eff} = 5,57V$
* gegeben: $R = 50Ω$ aus dem Messsystem
* gesucht: $P_E$

<fragment>
$\begin{split}P_E &= \frac{(U_{E,eff} \cdot 10)^2}{R}\\ &= \frac{(5,57V \cdot 10)^2}{50Ω}\\ &\approx 60W\end{split}$
</fragment>

--- style="font-size: smaller;"
## Feldstärkeanzeiger zur Leistungsmessung

<left>
[picture:496:a_messung_feldstaerkeanzeiger:Feldstärkeanzeiger]
</left>
<right>
* Messung der HF-Leistung über eine Antenne
* Empfangene HF wird gleichgerichtet und gepuffert
* Anzeige über empfindliches Strommessgerät
* Je höher der Zeigerausschlag, desto höher die HF-Feldstärke
* Exakte Messungen erfordern Kalibrierung
</right>

---
[question:AI613]
