Dieser Abschnitt zeigt, wie analoge Signale in digitale Werte und digitale Werte wieder in analoge Signale umgesetzt werden. Dazu werden *A/D-Umsetzer* (Analog-Digital-Umsetzer) und *D/A-Umsetzer* (Digital-Analog-Umsetzer) verwendet. Die Abbildung [ref:a_adc_dac] zeigt die Blockschaltbilder eines A/D- und eines D/A-Umsetzers.

<margin>
[picture:1130:a_adc_dac:A/D- und D/A-Umsetzer]
</margin>

Ein A/D-Umsetzer tastet ein analoges Eingangssignal zu bestimmten Zeitpunkten ab und erzeugt daraus digitale Zahlenwerte, die anschließend von weiteren Teilen einer Schaltung digital verarbeitet werden können.

Da ein A/D-Umsetzer nur mit einer begrenzten Anzahl möglicher digitaler Werte arbeitet, kann er die Amplitude eines analogen Eingangssignals nur in bestimmten Stufen erfassen. Wir erinnern uns dabei an das zuvor verwendete Beispiel mit Dimmer und Stufenschalter. Liegt der tatsächliche Wert zwischen zwei möglichen Stufen, muss er einer davon zugeordnet werden. Dadurch entsteht ein *Quantisierungsfehler*.

[question:AF607]

---

Die Anzahl der möglichen Stufen eines A/D-Umsetzers wird als dessen *Auflösung* bezeichnet. Sie wird häufig in Bit (Einheit: $\unit{\bit}$) angegeben. Kann ein Umsetzer beispielsweise $\num{256}$ unterschiedliche Werte unterscheiden, besitzt er eine Auflösung von $\qty{8}{\bit}$, denn mit $\qty{8}{\bit}$ lassen sich $\num{256}$ verschiedene Werte darstellen. Ein $\qty{16}{\bit}$-Umsetzer kann bereits $\num{65536}$ unterschiedliche Werte unterscheiden.

Bei Signalen, die sowohl positive als auch negative Werte annehmen können, wird typischerweise ein Teil dieser Werte für den positiven und ein Teil für den negativen Signalbereich verwendet.

Die Abbildung [ref:a_adc_4bit] zeigt ein Sinussignal, das durch einen A/D-Umsetzer mit einer Auflösung von $\qty{4}{\bit}$ digitalisiert und anschließend wieder in ein analoges Signal umgesetzt wurde. Die Abbildung [ref:a_adc_12bit] zeigt dasselbe Sinussignal, das jedoch durch einen A/D-Umsetzer mit einer Auflösung von $\qty{12}{\bit}$ digitalisiert und anschließend wieder in ein analoges Signal umgesetzt wurde. Man erkennt deutlich, dass die zusätzlichen $\qty{8}{\bit}$ zu einer wesentlich feineren Auflösung führen (um Faktor 256 besser), sodass das rekonstruierte Signal dem ursprünglichen Sinussignal bereits sehr nahe kommt.

<margin>
[picture:300:a_adc_4bit:Sinussignal digitalisiert durch einen 4-Bit-A/D-Umsetzer und anschließende D/A-Umsetzung]
[picture:299:a_adc_12bit:Sinussignal digitalisiert durch einen 12-Bit-A/D-Umsetzer und anschließende D/A-Umsetzung]
</margin>

[question:AF608]

Eine weitere wichtige Eigenschaft eines A/D-Umsetzers ist die zeitliche Genauigkeit der Abtastung. Die einzelnen Samples sollten möglichst exakt in den vorgesehenen zeitlichen Abständen aufgenommen werden. Dazu ist ein möglichst stabiler Abtasttaktgenerator erforderlich.

In der Praxis können die tatsächlichen Abtastzeitpunkte jedoch geringfügig von den idealen Zeitpunkten abweichen. Diese zeitlichen Schwankungen werden als *Jitter* bezeichnet. Jitter kann zu zusätzlichen Fehlern und damit zu zusätzlichem Rauschen im digitalisierten Signal führen. Der gleiche Mechanismus tritt auf der Seite des D/A-Umsetzers auf. Dort führt Jitter zu zusätzlichem Rauschen im Analogsignal.

[question:AF621]

---

Der Gegenspieler des A/D-Umsetzers ist der *D/A-Umsetzer*. Er erzeugt aus einem digitalen Datenstrom beziehungsweise aus digitalen Samples wieder ein analoges Signal.

Auch ein D/A-Umsetzer kann nicht beliebig viele unterschiedliche Ausgangswerte erzeugen. Wie beim A/D-Umsetzer besitzt er eine bestimmte Auflösung in Bit und damit nur eine endliche Anzahl möglicher Ausgangswerte.

Ein D/A-Umsetzer kann außerdem nur Spannungen innerhalb eines bestimmten Wertebereichs erzeugen, beispielsweise von $\qty{0}{\volt}$ bis $\qty{1}{\volt}$ oder von $\qty{-2}{\volt}$ bis $\qty{2}{\volt}$.

Bei einem linear arbeitenden D/A-Umsetzer sind die möglichen Ausgangswerte gleichmäßig über diesen Spannungsbereich verteilt. Besitzt ein D/A-Umsetzer beispielsweise eine Auflösung von $\qty{4}{\bit}$, stehen

$\num{2^4}=\num{16}$

mögliche Stufen zur Verfügung.

[question:AF609]

Verteilen sich diese auf einen Spannungsbereich von $\qty{0}{\volt}$ bis $\qty{1}{\volt}$, gibt es zwischen den $\num{16}$ Stufen insgesamt $\num{15}$ Zwischenschritte. Die Schrittweite beträgt daher

$\frac{\qty{1}{\volt}}{16-1}\approx\qty{67}{\milli\volt}.$

[question:AF611]
[question:AF610]

---

A/D- und D/A-Umsetzer werden beispielsweise in SDR-Empfängern und Transceivern eingesetzt. Analoge Eingangssignale werden zunächst durch einen A/D-Umsetzer digitalisiert und anschließend digital verarbeitet. Soll daraus wieder ein analoges Signal entstehen, werden die digitalen Werte mit einem D/A-Umsetzer zurück in analoge Spannungswerte umgesetzt.

Dabei kann es vorkommen, dass ein Eingangssignal nur einen kleinen Teil des verfügbaren Wertebereichs eines A/D-Umsetzers nutzt. In diesem Fall wird entsprechend auch nur ein Teil der verfügbaren digitalen Stufen verwendet.

Umgekehrt kann ein Eingangssignal den maximalen Wertebereich eines A/D-Umsetzers überschreiten. Werte oberhalb der maximal erfassbaren Eingangsspannung können dann nicht mehr korrekt dargestellt werden und werden nur noch mit dem maximal möglichen Wert abgebildet. Dieser Effekt wird als *Clipping* bezeichnet. Im Signalverlauf erscheinen die betroffenen Bereiche dadurch abgeschnitten.

Auch ein D/A-Umsetzer kann keine Ausgangsspannung außerhalb seines vorgesehenen Wertebereichs erzeugen.

Je höher die Auflösung eines A/D- oder D/A-Umsetzers ist, desto feiner können unterschiedliche Amplitudenwerte digital dargestellt beziehungsweise wieder in analoge Spannungswerte umgesetzt werden. Bei einer geringen Auflösung stehen dagegen nur wenige mögliche Stufen zur Verfügung, sodass die Abstufungen deutlicher sichtbar werden.

[question:AF613]
[question:AF612]
[question:AF614]