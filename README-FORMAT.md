# DARCdown

Im folgenden werden die entsprechenden Kommandos von DARCdown beschrieben: Grundsätzliche gilt wie bei Makdown: Den Text einfach so hinschreiben. Allerdings gibt es ein paar Spezialbefehle die wir im folgenden beschreiben wollen. 

## Fragen, Zeichnungen und Fotos

Fragen, Bilder und Fotos werden mit [ ]-Befehlen eingebunden, wobei der Doppelpunkt als Trennzeichen verwendet wird. Als erstes kommt der Befehl, dann die ID, bei Bildern folgt noch ein interner Bezeichner (für Referenzen) und dann die Bildbeschreibung. Interne Bezeichner mit dem Kurznamen des Abschnitts beginnen lassen.

Prüfungsfrage:
```
[question:AB123]
```

Zeichung:
```
[picture:484:n_funkhorizont:Ausbreitung]
```

Foto:
```
[photo:123:n_wasserfalldiagramm_trx_collage:Ansichten verschiedener Transceiver]
```

## Referenzen

Auf Bilder und Tabellen kann im Text mit dem `ref`-Kommando verwiesen werden. Dabei ist der interne Bezeichner anzugeben:

```
[ref:n_funkhorizont]
```

## Tabellen

Tabellen werden mit senkrechten Strichen "gemalt". Der senkrechte Strich ist auf der Tastatur mit Alt-Gr und der kleiner-als-Taste links vom Y erreichbar. Die erste Zeile ist die Kopfzeile, dort wird die Ausrichtung der Spalte festgelegt (l: linksbündig, c: zentriert, r: rechtsbündig, X: mehrzeilig linksbündig). Am Ende muss ein Tabellen-Kommando folgen. Nach dem `table`-Befehl folgt hier wie bei den Bildern ein interner Bezeichner (für Referenzen) und die Tabellenbeschreibung.

```
| l: Vorname | l: Rufzeichen |
| Max | DO7MAX |
| Luisa | DL2LS |
| Noa | DG5NOA |
[table:n_rufzeichen_beispiele:Beispiele für Rufzeichen]
```

## Besondere Abschnitte

* Randbemerkung: `<margin>...</margin>`
* Achtung: `<attention>...</attention>`
* Vertiefung: `<indepth>...</indepth>`
* Tipp: `<tip>...</tip>`
* Randbemerkung im Web, aber nicht in LaTeX, dort wird es Fließtext: `<webmargin>...</webmargin>`
* Tipp als Randbemerkung im Web, aber nicht in LaTeX, dort wird es Fließtext: `<webtip>...</webtip>`
* Vertiefung als Randbemerkung im Web, in LaTeX geht es über die komplette Seitenbreite: `<webindepth>...</webindepth>`
* Nur im Web, nicht im LaTeX: `<webonly>...</webonly>`
* Nur im LaTeX, nicht im Web: `<latexonly>...</latexonly>`

> [!WARNING]
> Die Tags funktionieren nur, wenn das öffnende und schließende Tag jeweils für sich auf einer Zeile stehen:
>
> ```
> <attention>
> Bitte aufpassen!
> </attention>
> ```

## Aufzählungen

Eine Aufzählung kann mit * eingeleitet werden. Nach dem letzten Punkt _muss_ eine Leerzeile folgen.

```
* Apfel und Apfelsinen
* Bananen und Birnen
* Clementinen und Zitronen
```

Eine nummerierte Aufzählung erfolgt einfach indem die Nummern vorangestellt werden. Nach dem letzten Punkt _muss_ wieder eine Leerzeile folgen.

```
1. Netzteil einschalten
2. Transceiver einschalten
3. PTT drücken
```

## Hervorhebungen

Einzelne Wörter und Wortgruppen lassen sich mit dem Stern hervorheben:

Einige *wichtige Wörter* hervorheben

## Formeln und Einheiten

Für Formeln wird wie bisher der LaTeX-Mathemodus benutzt:

```
$R = \frac{U}{I}$
```


Für Einheiten das Paket [siunitx](https://ctan.org/pkg/siunitx?lang=de):

```
Die Endstufe hat eine Leistung von $\qty{750}{\watt}$.

Die Einheit der Frequenz ist $\unit{\hertz}$

Die Länge des Drahts muss zwischen $\qtyrange{1}{10}{\meter}$ liegen.
```

## Morsecode

Morsezeichen können mit dem Morse-Befehl geschrieben werden.

```
[morse:CQ CQ]
```

## QSOs

QSOs können ebenfalls wiedergegeben werden. `qso_own` sind die Funksprüche der einen Station und `qso_other` für die Gegenstation:

```
[qso_own:CQ CQ DE DL1PZ K]
[qso_other:DL1PZ DO2MAX U R 59 K]
```

## Kommentare

Kommentare gehen weiterhin per %-Zeichen, aber nur am Anfang der Zeile! TODO als Markierung für offene Aufgaben.

```
% TODO Der Absatz muss neu formuliert werden
```

## Links

Hyperlinks sollten immer über den 50ohm.de-URL-Shortener abgebildet werden. 

## Index

Indexeinträge für die Suche werden mit `[index:Begriff]` bzw. `[index:Hauptbegriff:Unterbegriff]` erzeugt. Ein optionales Leerzeichen vor dem Befehl wird beim Konvertieren entfernt.

Beispiel:

```
Im Betrieb werden Yagi-Antennen [index:Antenne:Yagi-Antenne] oft ...
```
