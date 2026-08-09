In der Klasse E haben wir die AGC (Automatic Gain Control) bereites kennen gelernt. Bei starken Eingangssignalen wird durch die AGC die Verstärkung von Verstärkerstufen im Empfängerzweig reduziert und bei schwachen Eingangssignalen entsprechend erhöht. Hierdurch wird die Amplitude des demodulierten Signals und damit die Lautstärke des NF-Signals konstant gehalten.

Ohne eine AGC würden starke Signale die NF übersteuern und schwache Signale nur sehr leise in der NF hörbar sein. Die NF-Lautstärke müsste immer von Hand nachgeregelt werden. Die AGC gleicht somit die Dynamik des Empfangssignals aus und passt die Empfindlichkeit des Empfängerzweiges in Abhängigkeit der HF-Eingangssignale dynamisch an.

[question:AF224]

<margin>
[picture:1055:e_agc:AGC im Überlagerungsempfänger]
</margin>

---

Damit die AGC die Verstärkung automatisch an die Stärke des Empfangssignals anpassen kann, benötigt sie eine Information über dessen Amplitude. Dazu kann ein Teil des ZF-Signals gleichgerichtet und anschließend geglättet werden, wie in Abbildung [ref:e_agc_regelspannung] gezeigt.

Die Diode richtet das hochfrequente ZF-Signal gleich. Ein nachgeschaltetes RC-Glied unterdrückt die schnellen Wechselanteile, sodass eine Gleichspannung entsteht, deren Höhe von der Amplitude des ZF-Signals abhängt. Je stärker das empfangene Signal ist, desto größer ist auch der Betrag dieser Spannung. 

Diese *Regelspannung* wird zu den regelbaren HF- oder ZF-Verstärkerstufen zurückgeführt und dort zur Steuerung ihrer Verstärkung verwendet. Auf diese Weise entsteht ein geschlossener Regelkreis: Ein stärkeres Empfangssignal führt zu einer stärkeren Regelwirkung und damit zu einer geringeren Verstärkung.

<margin>
[picture:142:e_agc_regelspannung:AGC-Regelspannung]
</margin>

[question:AD503]
