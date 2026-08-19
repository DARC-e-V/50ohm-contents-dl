## Fourier-Transformation und Signalzerlegung

* Signale können sowohl im Zeit- als auch im Frequenzbereich dargestellt werden  
* Im Zeitbereich: X-Achse $\rightarrow$ Zeit, Y-Achse $\rightarrow$ Spannung oder Leistung  
* Im Frequenzbereich: X-Achse $\rightarrow$ Frequenz, Y-Achse $\rightarrow$ Amplitude oder Leistung

---

### Zerlegung von Signalen

* Jedes Signal lässt sich als Überlagerung von Sinusschwingungen darstellen  
* Jede Sinusschwingung hat eine bestimmte Amplitude und Phase  
* Dieses Prinzip ermöglicht es, komplexe Signale in ihre Bestandteile zu zerlegen

---

### Fourier-Transformation

* Mathematisch komplexes Verfahren, das ein zeitliches Signal analysiert  
* Zeigt an, welche Sinus-Schwingungen (Frequenzen) im Signal enthalten sind  
* Das Ergebnis wird als Frequenzspektrum dargestellt (X-Achse: Frequenz, Y-Achse: Amplitude/Leistung)

---

### Fast Fourier Transformation (FFT)

* Effiziente Berechnung der diskreten Fourier-Transformation (DFT)  
* Reduziert den Rechenaufwand erheblich  
* Weit verbreitet in Soft- und Hardware zur Signalverarbeitung

--- style="font-size: smaller;"

## Spektren typischer Signalformen

* *Sinus*: nur eine Frequenz: $f$
* *Rechteck*: nur ungeradzahlige Vielfache: $f$, $3f$, $5f$, $7f$, ...
* *Sägezahn*: alle ganzzahligen Vielfachen: $f$, $2f$, $3f$, $4f$, ...
* *Dreieck*: nur ungeradzahlige Vielfache: $f$, $3f$, $5f$, $7f$, ... (hohe Oberwellen fallen schneller ab als beim Rechteck)

In der Prüfung muss man nur Sinus und Rechteck unterscheiden können. 

<note>
Rechteck- und Dreiecksignal enthalten beide nur ungeradzahlige Oberwellen. Der Unterschied liegt im Abfall der Amplituden: Beim Dreiecksignal werden die höheren Oberwellen deutlich schneller kleiner.
</note>

---

[question:AF630]

---

[question:AB404]

---

[question:AB405]

---

[question:AB406]

---

[question:AB407]
