In der Klasse E haben wir das SWR-Meter und seine Anwendung bereits kennengelernt. In der Klasse A wollen wir verstehen, wie ein Stehwellenmessgerät intern funktioniert. Ein SWR-Meter besteht in der Regel aus zwei Richtkopplern. Zu nächst wollen wir uns mit deren Funktionsweise vertraut machen. 

Ein *Richtkoppler* dient dazu, einen kleinen Teil eines HF-Signals aus einer Speiseleitung auszukoppeln. Seine Besonderheit besteht darin, dass er dabei unterscheiden kann, in welche Richtung sich die Welle auf der Leitung ausbreitet. Dazu wird das Signal auf zwei unterschiedliche Arten erfasst. Über eine kapazitive Kopplung wird eine Spannung $U_C$ gewonnen, die von der Spannung auf der Speiseleitung abhängt. Gleichzeitig erzeugt die induktive Kopplung eine Spannung $U_I$, die vom Strom auf der Speiseleitung abhängt. Der Richtkoppler wird so dimensioniert, dass die kapazitiv und induktiv gewonnenen Signalanteile an seinen Ausgängen gleich groß sind. An den beiden Ausgängen werden diese Anteile jedoch mit unterschiedlichem Vorzeichen miteinander kombiniert.

Bei einer Welle, die sich in einer bestimmten Richtung auf der Leitung ausbreitet, z. B. von links nach rechts wie in Abbildung [ref:a_richtkoppler_rechts_links] dargestellt, addieren sich die kapazitiv und induktiv gewonnenen Spannungen an einem Ausgang. Am anderen Ausgang sind sie gegensinnig und heben sich im Idealfall gegenseitig auf. Das Signal erscheint daher hauptsächlich an nur einem der beiden Ausgänge.

<margin>
[picture:1109:a_richtkoppler_rechts_links:Richtkoppler, die Welle läuft von links nach rechts]
</margin>

---

Kehrt sich die Ausbreitungsrichtung der Welle um, wie z. B. von rechts nach links wie in Abbildung [ref:a_richtkoppler_rechts_links] dargestellt, kehrt sich auch die Richtung des Stroms relativ zur Spannung um. Dadurch ändert die induktiv gekoppelte Spannung $U_I$ ihr Vorzeichen, während sich die kapazitiv gekoppelte Spannung $U_C$ entsprechend der Leitungsspannung ergibt.

<margin>
[picture:1110:a_richtkoppler_rechts_links:Richtkoppler, die Welle läuft von rechts nach links]
</margin>

Damit vertauschen sich auch die beiden Ausgänge des Richtkopplers: Der Ausgang, an dem sich die beiden Anteile zuvor addiert haben, wird nun weitgehend ausgelöscht, während sie sich am anderen Ausgang addieren.

Auf diese Weise kann ein Richtkoppler zwischen einer *vorlaufenden Welle* in Richtung Antenne und einer *rücklaufenden Welle* in Richtung Sender unterscheiden.

---

Diese Eigenschaft der Richtkoppler wird in einem *Stehwellenmessgerät* beziehungsweise *SWR-Meter* genutzt: Man misst hierzu die  die Ausgangsspannungen zweier in die Leitung eingeschleifter Richtkoppler, die in gegensätzlicher Richtung betrieben werden. Die HF-Spannungen an den Ausgängen der Richtkoppler werden mit Dioden gleichgerichtet und geglättet. Dadurch entstehen Gleichspannungen, die mit einem Messinstrument angezeigt werden können.

[question:AI401]

Die Abbildung [ref:a_rswr_meter] zeigt den prinzipiellen Aufbau eines Stehwellenmessgeräts mit zwei Richtkopplern. Dabei nehmen wir an, dass sich der Sender auf der linken und die Antenne auf der rechten Seite befindet.

[question:AI402]

Der obere Leiter ist Teil der Speiseleitung zwischen Sender und Antenne. An ihm werden zwei Größen erfasst: Über die kapazitive Kopplung wird ein kleiner Anteil der HF-Spannung ausgekoppelt. Über die induktive Kopplung wird gleichzeitig ein Anteil gewonnen, der vom Strom auf der Speiseleitung abhängt.

Die jeweils nicht zur Messung verwendete Seite der Koppelleitung wird mit einem *Abschlusswiderstand* abgeschlossen. Dieser Widerstand entspricht näherungsweise dem Wellenwiderstand $Z_0$ der Koppelleitung. Dadurch wird die dort ankommende HF-Leistung aufgenommen und nicht wieder in die Koppelleitung zurückreflektiert. Solche Reflexionen würden die Trennung zwischen vorlaufender und rücklaufender Welle verschlechtern.

Diese beiden Signalanteile werden im Richtkoppler miteinander kombiniert. Für eine Welle, die vom Sender zur Antenne läuft, addieren sie sich in einem der beiden Koppler, während sie sich im anderen weitgehend gegenseitig aufheben. Bei einer Welle in der entgegengesetzten Richtung ist es genau umgekehrt.

Die beiden nahezu spiegelbildlich aufgebauten Schaltungsteile können dadurch unterschiedliche Laufrichtungen erfassen:

* Der eine Richtkoppler liefert ein Signal proportional zur *vorlaufenden Welle* vom Sender zur Antenne.
* Der andere Richtkoppler liefert ein Signal proportional zur *rücklaufenden Welle* von der Antenne zum Sender.

Die ausgekoppelten Signale sind zunächst HF-Wechselspannungen. Die Dioden richten diese Spannungen gleich, und die Kondensatoren glätten sie. Dadurch entstehen Gleichspannungen, die mit den beiden Messwerken eines Kreuzzeigerinstruments angezeigt werden können, oder durch einen Mikrocontroller mit A/D-Umsetzer gemessern werden können. Die einstellbaren Widerstände dienen dabei zum Abgleich beziehungsweise zur Kalibrierung der Anzeige. Sie sind von den Abschlusswiderständen der Koppelleitungen zu unterscheiden, die für einen reflexionsarmen Abschluss mit $Z_0$ sorgen.

<margin>
[picture:499:a_rswr_meter:SWR-Meter mit zwei Richtkopplern]
</margin>
