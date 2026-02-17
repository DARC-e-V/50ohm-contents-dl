Am Anfang dieses Kapitels haben wir uns mit dem Dipol als Grundform aller Antennen beschäftigt. Der Halbwellendipol strahlt Funkwellen senkrecht zur Drahtrichtung ab. Andere Antennenformen können ihre Funkwellen je nach Bauform bevorzugt in eine oder mehrere Richtungen abstrahlen und dafür weniger in andere Richtungen:
* Eine Groundplane-Antenne strahlt in alle Himmelsrichtungen nahezu gleichmäßig ab, aber nicht nach oben oder unten.
* Bei einer Yagi-Uda-Antenne werden die Funkwellen wie bei einer Taschenlampe in einem Strahl nach vorn gebündelt und in alle anderen Richtungen reduziert.

Die vom Nachweisverfahren zum Schutz von Personen in elektromagnetischen Feldern vorgegebenen Grenzwerte muss eine Sendeanlage in jede Richtung einhalten. Wenn in einem bestimmten Abstand von der Antenne die Grenzwerte in die Richtung eingehalten werden, in die sie am stärksten abstrahlt, dann wird sie die Grenzwerte im gleichen Abstand auch in alle anderen Richtungen einhalten. Daher interessiert uns besonders die Richtung der stärksten Abstrahlung. Diese wird als *Hauptstrahlrichtung* bezeichnet.

---

Wie stark eine Antenne in ihre Hauptstrahlrichtung abstrahlt, wird durch den *Gewinnfaktor* bezogen auf den Halbwellendipol ausgedrückt. Dieser gibt an, wieviel besser eine Antenne im Vergleich zu einem Halbwellendipol in die jeweilige Hauptstrahlrichtung abstrahlt. Ein Gewinnfaktor von $\num{2}$ gegenüber dem Halbwellendipol bedeutet beispielsweise, dass eine Antenne in die Hauptstrahlrichtung doppelt so stark abstrahlt wie ein Halbwellendipol in seine Hauptstrahlrichtung.

<indepth>
% TODO: Editionsspezifisch machen
Anstelle des Gewinnfaktors von Antennen wird häufig der "Gewinn in Dezibel ($\unit{\dB}$)" angegeben. Mit der Einheit Dezibel beschäftigt sich der Kurs für die Klasse E.
</indepth>

---

Um nun anzugeben, wieviel eine konkrete Antenne in die Hauptstrahlrichtung abstrahlt wenn man eine bestimmte Sendeleistung eingibt, multipliziert man die Sendeleistung mit dem auf den Halbwellendipol bezogenen Gewinnfaktor. Dann erhält man die *effektive Strahlungsleistung*, die meist als ERP (vom englischen "effective radiated power") abgekürzt wird. Geben wir beispielsweise eine Sendeleistung von $\qty{5}{\watt}$ in eine Antenne mit einem Gewinnfaktor von $\num{2}$ gegenüber dem Halbwellendipol, dann ergibt sich eine Strahlungsleistung von $\qty{10}{\watt}$ ERP.

<margin>
Man kann sich die effektive Strahlungsleistung (ERP) auch so vorstellen: Es ist die Leistung, die man in einen Halbwellendipol einspeisen müsste, damit dieser in seiner Hauptstrahlrichtung genauso stark abstrahlt wie die betrachtete Antenne.
</margin>

Richtantennen können viel größere Gewinnfaktoren haben. Eine Yagi-Uda-Antenne aus 9 Elementen kann beispielsweise leicht einen Gewinnfaktor von $\num{10}$ oder mehr gegenüber dem Halbwellendipol erreichen. Gibt man in eine solche Antenne z. B. $\qty{100}{\watt}$ ein, beträgt die Strahlungsleistung bereits $\qty{1000}{\watt}$ ERP oder mehr!

[question:NG401]
