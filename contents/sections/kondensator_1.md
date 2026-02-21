Ein sehr wichtiges und häufig verwendetes Bauteil in der Funktechnik und Elektronik ist der Kondensator. Wie in Abbildung [ref:e_kondensator_aufbau] dargestellt, besteht ein Kondensator prinzipiell aus zwei leitenden Flächen (Platten, Schichten bzw. Elektroden), die durch einen Isolator – das sogenannte Dielektrikum – voneinander getrennt sind.


<margin>
[picture:922:e_kondensator_aufbau:Prinzipieller Aufbau eines Kondensators]
</margin>

Die geometrischen Abmessungen bestimmen eine wichtige Eigenschaft eines Kondensators, es ist die Fähigkeit, Ladungen zu speichern. Diese Fähigkeit wird als Kapazität bezeichnet und hierfür wird der Formelbuchstabe $C$ verwendet. Je größer die Kapazität ist, umso mehr elektrische Ladungen $Q$ können gespeichert werden. Wenn die angelegte Spannung erhöht wird, werden auch mehr Ladungen gespeichert.

Die Folgende Fomel zeigt den Zusammenhang. 

$Q = C \cdot U $ 

Diese Formel steht nicht in der Formelsammlung und wird auch nicht für die Prüfung benötigt.

<unit>
Die Einheit der Ladung $Q$ ist $\unit{\ampere\second}$
</unit>

<unit>
Die Einheit der Kapazität $C$ ist $\unit{\ampere\second\per\volt}$ oder kurz *Farad* $\unit{\farad}$ zu Ehren des englischen Naturforschers Michael Faraday (1791 - 1867). $\qty{1}{\farad}$ ist die Kapazität eines Kondensators, in dem eine Ladung von $\qty{1}{\ampere\second}$ bei einer Spannung von $\qty{1}{\volt}$ gespeichert wird.
</unit>

[question:EA101]

Wird an einen Kondensator eine Spannung angelegt, entsteht zwischen den leitenden Platten ein elektrisches Feld $E$. Diesen Zusammenhang haben wir bereits im Kapitel zum elektrischen Feld kennengelernt: Je höher die angelegte Spannung und je kleiner der Abstand zwischen den Platten ist, desto stärker ist das elektrische Feld. Mathematisch lässt sich dies ausdrücken durch:

$E = \frac{U}{d}$

Zur Berechnung der Kondensatorkapazität aus den Abmessungen dient folgende Formel aus der Formelsammlung:

---

$C = \frac{\varepsilon_0 \cdot \varepsilon_r \cdot A}{d}$

Im Folgenden sind die einzelnen Größen der Formel aufgeschlüsselt:

- $A$ ist die gegenüberstehende Fläche der leitenden Platten
- $d$ ist der Abstand zwischen den Flächen
- $\varepsilon_0 = \qty{0,855e-11}{\ampere\second\per\volt\meter}$ ist die elektrische Feldkonstante, eine Naturkonstante
- $\varepsilon_r$  (sprich: "Epsilon R") ist eine spezielle Eigenschaft des Isolators (Dielektrikum) ist die sogenannte relative Dielektrizitätszahl welche vom Verwendeten Material abhängt. Die Tabelle [ref:e_Dielektrizitätszahl] mit Materialwerten findet man auch in der Formelsammlung.

<margin>
| Material | $\varepsilon_r$  |
| Luft (trocken) | 1,00059 |
| Voll-PE (Polyäthylen | 2,29 |
| Schaum-PE | 1,5 |
| PTFE (Teflon) | 2,0 |
[table:e_Dielektrizitätszahl:Relative Dielektrizitätszahl $\varepsilon_r$ ]
</margin>

Mit Hilfe der Formel kann man bereits eine Reihe von Prüfungsfragen lösen. Man stellt zunächst fest, dass die Spannung $U$ in der Formel nicht vorkommt. 

[question:EC205]

Die Kapazität eines Kondensators sinkt, wenn der Plattenabstand größer wird. 

[question:EC204]
[question:EC203]

---

Betrachten wir zunächst den Kondensator im Gleichstromfall. In Abbildung [ref:e_stromkreis_kondensator] ist eine Schaltung zum Aufladen eines Kondensators dargestellt. Dabei wird angenommen, dass der Kondensator $C$ zunächst ungeladen ist, also noch keine elektrische Ladung gespeichert hat. Wird der Schalter geschlossen, so wird der Kondensator $C$ über einen Widerstand $R$ an eine Gleichspannungsquelle (Batterie) angeschlossen.

Durch die angelegte Spannung entsteht ein elektrisches Feld zwischen den Kondensatorplatten. Dieses Feld bewirkt eine Umlagerung von Ladungen: Elektronen werden vom negativen Pol der Spannungsquelle auf die angeschlossene Kondensatorplatte gedrückt, sodass sich dort ein Elektronenüberschuss bildet. Gleichzeitig werden Elektronen von der gegenüberliegenden Platte zum positiven Pol der Spannungsquelle abgezogen, wodurch dort ein Elektronenmangel entsteht. Obwohl kein Strom durch das Dielektrikum fließt, führt diese Ladungstrennung zur Aufladung des Kondensators. 

<margin>
[picture:1015:e_stromkreis_kondensator:Stromkreis zum Aufladen eines Kondesators]
</margin>

---

Das bedeutet: Zu Beginn fließt ein hoher Strom, der lediglich durch den Widerstand $R$ begrenzt wird. Mit der Zeit werden immer mehr Ladungen im Kondensator gespeichert. Dadurch nimmt der Strom kontinuierlich ab, während die Spannung $U_C$ am Kondensator ansteigt, bis dieser vollständig aufgeladen ist. In diesem Zustand fließt schließlich kein Strom mehr.

Dieser Vorgang erfolgt jedoch nicht schlagartig, sondern zeitlich verzögert. Die Kondensatorspannung steigt dabei nach einer sogenannten Exponentialfunktion an, wie in Abbildung [ref:e_ladekurve_c] gezeigt. Die Dauer dieses Ladevorgangs hängt vom vorgeschalteten Widerstand ab: Je größer der Widerstand ist, desto länger dauert es, bis der Kondensator „vollständig“ geladen ist. Mit einem Oszilloskop, wie in Abbildung [ref:e_lade_entladespannung_mit_oszilloskop] gezeigt, das wir bereits kennengelernt haben, lässt sich dieser zeitliche Verlauf anschaulich beobachten und untersuchen.

<margin>
[picture:185:e_ladekurve_c:Ladespannung eines Kondesators]
</margin>

<margin>
[photo:247:e_lade_entladespannung_mit_oszilloskop:Lade-und Entladespannung an einem Kondensator]  
</margin>
 
Beim Entladevorgang fließt der Strom entgegen der Ladestromrichtung und die Spannung am Kondensator baut sich langsam ab.

[question:EC201]

Im Fall von Wechselstrom und Wechselspannungen müssen wir einen weiteren wichtigen Aspekt berücksichtigen: Ein Kondensator verhält sich wie ein frequenzabhängiger Widerstand. Dieser lässt sich durch die Beziehung

$|X_C| = \frac{1}{\omega\cdot C} = \frac{1}{2\pi\cdot f \cdot C}$

beschreiben und wird als kapazitiver Blindwiderstand $X_C$ bezeichnet (vgl. Formelsammlung).

Die genauen physikalischen Hintergründe dazu lernen wir erst in der Klasse A kennen. Für die Klasse E ist es jedoch bereits wichtig zu wissen, dass der Widerstand eines Kondensators umgekehrt proportional von der Frequenz abhängt: Verringert man die Frequenz, so wird der kapazitive Blindwiderstand $X_C$ größer. Erhöht man hingegen die Frequenz, nimmt der Widerstand entsprechend ab.

[question:EC202]

---

Nun haben wir bereits einige grundlegende elektrische Eigenschaften eines Kondensators kennengelernt, und im Folgenden wollen wir uns noch mit den verschiedenen Bauformen beschäftigen. Die Abbildung [ref:e_kondensatorvarianten] zeigt verschiedene Kondensatorvarianten.

<margin>
[photo:206:e_kondensatorvarianten:Kondensatorvarianten]
</margin>

Als Dielektriukumg, also Isolatorschicht, können unterschiedliche Materialien verwendet werden:

1.  Luft beim Luftdrehkondensator oder Lufttrimmer
2. Kunststofffolie beim Folienwickelkondensator
3. Keramik für HF-Kondensatoren mit hoher Güte und bei SMD-Kondensatoren
4. Metalloxid beim Elektrolytkondensator.

Je nach Aufbau unterscheidet man außerdem:

* Festkondensatoren in Form von Keramikkondensatoren, Folienkondensatoren und Elektrolytkondensatoren
* Veränderliche Kondensatoren in Form von Drehkondensatoren und Trimmkondensatoren

---

*Luftkondensatoren* und *Keramikkondensatoren*, wie in Abbildung [ref:e_aufbau_keramik_c] gezeigt, werden z.B. gerne für HF-Filter verwendet. 
[question:ED216] 

<margin>
[picture:923:e_aufbau_keramik_c: Keramikkondensator]
</margin>

*Elektrolytkondensatoren* (kurz ELKO) enthalten eine dünne, aufgerauhte ALU-Folie, die in einen Elektrolyten (z.B. Borax) eingetaucht ist. Dabei verursacht der Elektrolyt eine chemische Oxidation der Aluminiumoberfläche. Die entstehende Oxidschicht ist sehr dünn und deshalb steigt die Kapazität bei geringer Baugröße sehr stark an. Allerdings hat die dünne Schicht nur eine begrenzte Spannungsfestigkeit, die auf dem ELKO anggeben wird.
Elektrolytkondensatoren dürfen nur an Gleichspannung betrieben werden. Die Polung ist deshalb zu beachten, da sich sonst die Oxidschicht abbaut und somit die Spannungsfestigkeit sinkt. Der Kondesator wird zerstört. Alle anderen Kondensatoren können auch an Wechselspannung angeschlossen werden.
[question:EC207]

%<margin>
%TODO: Bild Elko
%</margin>

Für Folien-Wickelkondensatoren werden Kunststoffe in speziellen Verfahren zu extrem dünnen Folien verarbeitet, mit Elektroden versehen und anschließend entweder zu einem Wickel aufgewickelt oder aus einzelnen Lagen geschichtet und zu einem Kondensator zusammengefügt, wie in Abbildung [ref:e_aufbau_wickel_c] dargestellt. Neben Keramikkondensatoren und Elektrolytkondensatoren zählen sie zu den am häufigsten eingesetzten Kondensatorbauarten.

<margin>
[picture:49:e_aufbau_wickel_c:Folien-Wickelkondensator]
</margin>

Drehkondensatoren werden häufig in Endstufen und Anpassnetzwerken eingesetzt. Bei ihnen lässt sich die Kapazität einstellen, indem ein Teil der Kondensatorplatten auf einer isolierten Achse montiert ist und zwischen feststehenden Platten rotiert. Dadurch ändert sich die wirksame Überlappungsfläche der Platten und somit die Kapazität, wie in Abbildung [ref:e_drehkondensator] dargestellt. Trimmkondensatoren arbeiten nach einem ähnlichen Prinzip, sind jedoch nicht für eine regelmäßige Verstellung vorgesehen. Sie dienen vielmehr zum einmaligen oder gelegentlichen Abgleich von Schaltungen, etwa bei der Inbetriebnahme oder Kalibierung.

[question:EC206]

<margin>
 [picture:840:e_drehkondensator:Aufbau eines Drehkondensators]
</margin>

Die verwendeten Schaltzeichen für die verschiedenen Kondensatoren unterscheiden sich auch wie in Abbildung [ref:e_kondensator_schaltzeichen] dargestellt.

<margin>
[picture:924:e_kondensator_schaltzeichen:Schaltzeichen verschiedener Kondensatorarten]

Schaltzeichenzuordnung: 
a) Festkondensator 
b) gepolter Kondensator/ Elektrolytkondensator (Elko)/Tantalkondensator
c) Drehkondensator (Drehko) 
d) Trimmkondensator für Abgleichzwecke
</margin>
