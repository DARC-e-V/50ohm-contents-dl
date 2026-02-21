## Der Prozess des Samplings

* Analoge Signale werden in diskrete Samples umgewandelt  
* Sampling: Abtastung eines kontinuierlichen Signals in festgelegten Zeitabständen  
* Vergleichbar mit einer Kamera, die in regelmäßigen Intervallen Bilder aufnimmt

---

### Sampling – Das Kamerabeispiel

* Eine Kamera nimmt z. B. $\num{24}$ Bilder pro Sekunde auf
* Zwischen den Bildern können schnelle Bewegungen auftreten, die nicht erfasst werden  
* Wie bei der Kamera kann ein plötzliches Ereignis (z. B. eine Fliege) zwischen zwei Aufnahmen verloren gehen  
* Dadurch entsteht ein Verlust an zeitlicher Information

---

### Informationsverlust und Rekonstruktionsgrenze

* Zwischen den Samples können schnelle Signaländerungen unentdeckt bleiben  
* Für eine fehlerfreie Rekonstruktion muss vor und nach jedem Signalwechsel ein Sample vorliegen  
* Ist dies nicht der Fall, gehen Details verloren – Aliasing tritt auf

---

## Das Nyquist-Shannon-Abtasttheorem

* Für ein Signal mit maximaler Frequenz $f_{max}$ muss die Abtastrate $\gt 2 \cdot f_{max}$ betragen  
* Nur so können alle Signalwechsel korrekt erfasst und rekonstruiert werden  
* Wird diese Grenze unterschritten, entstehen Alias-Effekte

---

[question:AF617]

---

### Praktisches Beispiel: CD-Player

* CD-Player arbeiten typischerweise mit $\qty{44,1}{\kilo\sps}$ ($\num{44100}$ Samples pro Sekunde)
* Daraus folgt: Frequenzen bis ca. $\qty{22}{\kilo\hertz}$ können korrekt abgebildet werden
* Dies entspricht dem HiFi-Frequenzbereich guter Stereoanlagen  
* Merke: Die Abtastfrequenz sollte stets knapp über dem Doppelten der maximal zu verarbeitenden Frequenz liegen

---

[question:AF616]

---

[question:AF618]

---

[question:AF619]
