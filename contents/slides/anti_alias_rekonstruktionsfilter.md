--- style="font-size: smaller;"

## Filter bei der A/D- und D/A-Umsetzung

[picture:1131:a_adc_dac_filter:A/D- und D/A-Umsetzung mit Anti-Aliasing- und Rekonstruktionsfilter]

* Vor dem A/D-Umsetzer: *Anti-Aliasing-Filter*
* Nach dem D/A-Umsetzer: *Rekonstruktionsfilter*
* Beide Filter unterdrücken unerwünschte Frequenzanteile

<note>
Die Abbildung zeigt die gesamte Signalkette von einem analogen Eingangssignal über die digitale Signalverarbeitung bis zurück zu einem analogen Ausgangssignal.

Vor dem A/D-Umsetzer befindet sich das Anti-Aliasing-Filter. Hinter dem D/A-Umsetzer befindet sich das Rekonstruktionsfilter.

Warum beide Filter benötigt werden, schauen wir uns nun genauer an.
</note>

---

## Aliasing am A/D-Umsetzer

* Für die Abtastung gilt: $f_\mathrm{S}>2\cdot f_\mathrm{max}$
* Am Eingang können auch unerwünschte höhere Frequenzen vorhanden sein
* Ist die Samplingrate dafür zu gering, entstehen scheinbare Frequenzen
* Diese werden als *Aliase* bezeichnet

<note>
Über eine Antenne empfangen wir in der Regel nicht nur das gewünschte Signal, sondern viele weitere Frequenzanteile.

Ist die Samplingrate für einen dieser Frequenzanteile zu gering, kann er nach der Digitalisierung als eine andere Frequenz erscheinen, die im ursprünglichen Signal gar nicht vorhanden war.

Diesen Effekt haben wir bereits beim Abtasttheorem kennengelernt.
</note>

--- style="font-size: smaller;"

## Anti-Aliasing-Filter

[picture:1131:a_adc_dac_filter_aa:A/D- und D/A-Umsetzung mit Anti-Aliasing- und Rekonstruktionsfilter]

* Das Filter befindet sich *vor* dem A/D-Umsetzer
* Es begrenzt den Frequenzbereich des Eingangssignals
* Tiefpass- oder Bandpassfilter können eingesetzt werden
* Kritische Frequenzanteile müssen ausreichend unterdrückt werden

<fragment>
Insbesondere dürfen Frequenzen oberhalb von $\frac{f_\mathrm{S}}{2}$ nicht ungehindert zum A/D-Umsetzer gelangen.
</fragment>

<note>
Das Anti-Aliasing-Filter verhindert, dass Frequenzen zum A/D-Umsetzer gelangen, für die die Samplingrate nicht ausreichend hoch ist.

Je nach Anwendung kann dazu beispielsweise ein Tiefpass- oder Bandpassfilter eingesetzt werden. Für Sprachsignale kann beispielsweise ein Bandpass sinnvoll sein.

Entscheidend ist, dass Frequenzanteile, die zu Aliasing führen könnten, vor der Digitalisierung ausreichend unterdrückt werden.
</note>

---

[question:AF622]

---

[question:AF623]

---
## Abtastratengenerator

<left>
[picture:1132:a_anit_alias:Anti-Aliasing-Filter, A/D-Umsetzer und Taktgenerator]
</left>
<right>
* Der A/D-Umsetzer benötigt einen Takt für die Abtastung
* Der Takt legt die Zeitpunkte der einzelnen Samples fest
* Seine Frequenz bestimmt die Samplingrate
* Die Taktrate kann fest oder steuerbar sein
</right>

<note>
Der Abtastratengenerator gibt vor, wann der A/D-Umsetzer jeweils ein neues Sample aufnimmt.

Seine Frequenz bestimmt damit unmittelbar die Samplingrate. Die Taktrate kann fest vorgegeben oder beispielsweise durch einen Mikrocontroller gesteuert werden.
</note>

---

[question:AF620]

---

## Zurück zum analogen Signal

* Der D/A-Umsetzer erzeugt aus digitalen Samples wieder analoge Spannungswerte
* Die Werte werden in festen zeitlichen Abständen ausgegeben
* Am Ausgang entsteht zunächst kein ideal glatter Signalverlauf
* Scharfe Übergänge enthalten hohe Frequenzanteile

<note>
Auf der Ausgangsseite findet der umgekehrte Vorgang statt.

Der D/A-Umsetzer gibt die einzelnen digitalen Werte als analoge Spannungswerte aus. Durch die zeitdiskrete Ausgabe entsteht zunächst kein ideal glatter Verlauf.

Insbesondere scharfe Kanten und Übergänge enthalten zusätzliche hochfrequente Signalanteile.
</note>

--- style="font-size: smaller;"

## Rekonstruktionsfilter

<left>
[picture:300:a_adc_4bit:Signal vor dem Rekonstruktionsfilter]
</left>
<right>
[picture:299:a_adc_12bit:Signal nach dem Rekonstruktionsfilter]
</right>

* Das Rekonstruktionsfilter befindet sich *hinter* dem D/A-Umsetzer
* Es lässt den gewünschten Nutzfrequenzbereich passieren
* Unerwünschte höherfrequente Signalanteile werden unterdrückt
* Tiefpass- oder Bandpassfilter können eingesetzt werden

<fragment>
Dadurch entsteht wieder ein möglichst sauberes analoges Ausgangssignal.
</fragment>

<note>
Das Rekonstruktionsfilter entfernt unerwünschte höherfrequente Signalanteile am Ausgang des D/A-Umsetzers.

Links ist ein Signal vor der Filterung dargestellt. Die deutlich sichtbaren Kanten enthalten hohe Frequenzanteile.

Nach der Filterung entsteht ein glatterer Signalverlauf, der dem gewünschten analogen Signal näherkommt.

Je nach Anwendung kann dafür beispielsweise ein Tiefpass- oder Bandpassfilter verwendet werden.
</note>

---

[question:AF624]

---

[question:AF625]