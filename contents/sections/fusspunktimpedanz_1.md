Bei einem resonanten, mittengespeisten Halbwellendipol im Freiraum liegt die Speiseimpedanz idealisiert bei etwa $\qty{73,1}{\ohm}$ und damit näherungsweise bei $\qty{75}{\ohm}$. Dieser Wert liegt zwar bereits in der Größenordnung von den gewünschten $\qty{50}{\ohm}$, stimmt aber nicht exakt damit überein. Wird ein solcher Dipol direkt mit einer $\qty{50}{\ohm}$-Speiseleitung betrieben, entsteht daher eine leichte Fehlanpassung. Für eine optimale Leistungsübertragung bzw. ein möglichst niedriges SWR kann deshalb auch bei einem Dipol eine Anpassung sinnvoll sein. Das gilt grundsätzlich auch bei Aufbauhöhen von etwa einer Wellenlänge oder mehr, wobei die tatsächliche Speiseimpedanz je nach Drahtstärke, Umgebung und Aufbauhöhe leicht abweichen kann, wie wir gleich sehen werden.

<margin>
[picture:788:e_fusspunktimpedanz_dipol:Fußpolimpedanz eines Dipols in Abhängigkeit von der Aufbauhöhe (Simuliert mit NECPP)]
</margin>

[question:EG207]

Bei Wechselwirkung mit dem Boden aufgrund geringerer Aufbauhöhe bewegt sich die Speiseimpedanz eines mittengespeisten Dipols im Bereich von $\qty{40}{\ohm}$ bis $\qty{90}{\ohm}$ wie in der Abbildung [ref:e_fusspunktimpedanz_dipol] dargestellt. 

[question:EG208]
[question:EG209]

Führt man einen Dipol als Faltdipol aus, dann verdoppelt sich aufgrund der in Reihe geschalteten jedoch teilweise parallel geführten Antennenabschnitte die anliegende Spannung und der benötigte Strom halbiert sich. Dies entspricht einer Vervierfachung der Speiseimpedanz. Deshalb hat ein Faltdipol eine Fußpunktimpedanz von $\qtyrange{240}{300}{\ohm}$.

[question:EG210]

---

Bei einer Groundplane-Antenne hingegen entfällt der eine Dipolschenkel und wird durch eine Erde mit möglichst geringem Widerstand ersetzt. Hier kommt man also auf einen Speisewiderstand von $\frac{\qty{73,1}{\ohm}}{2} \approx \qty{37}{\ohm}$, was der Hälfte des Speisewiderstands eines Dipols im Freiraum entspricht. Bei Groundplaneantennen mit um $\qty{45}{\degree}$ nach unten abgewinkelten Radialen ergibt sich durch zusätzliche Abstrahlung durch die Radiale ein Speisewiderstand von genau $\qty{50}{\ohm}$, so dass keine weitere Anpassung an übliche Koaxialkabel notwendig wird. Deshalb liegt die Fußpunktimpedanz einer Groundplane zwischen $\qtyrange{30}{50}{\ohm}$.

<indepth>
Bei schlechter Erdung oder Wechselwirkung mit dem Erdboden kann sich für eine Groundplane-Antenne auch bei horizontal verlegten Radialen (z. B. auf der Erdoberfläche) ein Speisewiderstand von über $\qty{37}{\ohm}$ ergeben. Der zusätzliche Widerstand ergibt sich dann durch Bodenverluste.
</indepth>

[question:EG211]
