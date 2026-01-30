# Inhalte 50ohm.de

Dieses Repository enthält die Inhalte der Plattform 50ohm.de. Der Plattform-Code findet sich in einem gesonderten [Repository](https://github.com/DARC-e-V/50ohm). Die Lernplattform ist ein Angebot des AJW-Referats des DARC (Deutscher Amateur-Radio-Club e.V.). Viele ehrenamtlichen Mitarbeiterinnen und Mitarbeiter sind daran beteiligt.

# DARCdown

Für die Inhalte nutzen wir einen Markdown dialekt namens DARCdown. Im folgenden werden die entsprechenden Kommandos beschrieben: Grundsätzliche gilt wie bei Makdown: Den Text einfach so hinschreiben. Allerdings gibt es ein paar Spezialbefehle die wir im folgenden beschreiben wollen. 


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

Auf Bilder und Tabellen kann im Text mit dem ref-Kommando verwiesen werden. Dabei ist der interne Bezeichner anzugeben:

```
[ref:n_funkhorizont]
```

## Tabellen

Tabellen werden mit senkrechten Strichen "gemalt". Der senkrechte Strich ist auf der Tastatur mit Alt-Gr und der kleiner-als-Taste links vom Y erreichbar. Die erste Zeile ist die Kopfzeile, dort wird die Ausrichtung der Spalte festgelegt (l: linksbündig, c: zentriert, r: rechtsbündig, X: mehrzeilig linksbündig). Am Ende muss ein Tabellen-Kommando folgen. Nach dem table-Befehl folgt hier wie bei den Bildern ein interner Bezeichner (für Referenzen) und die Tabellenbeschreibung.

```
| l: Vorname | l: Rufzeichen |
| Max | DO7MAX |
| Luisa | DL2LS |
| Noa | DG5NOA |
[table:n_rufzeichen_beispiele:Beispiele für Rufzeichen]
```

## Besondere Abschnitte

Randbemerkung: `<margin>...</margin>`
Achtung: `<attention>...</attention>`
Vertiefung: `<indepth>...</indepth>`
Tipp: `<tip>...</tip>`
Randbemerkung im Web, aber nicht in LaTeX, dort wird es Fließtext: `<webmargin>...</webmargin>`

Tipp als Randbemerkung im Web, aber nicht in LaTeX, dort wird es Fließtext: `<webtip>...</webtip>`
Vertiefung als Randbemerkung im Web, in LaTeX geht es über die komplette Seitenbreite: `<webindepth>...</webindepth>`
Nur im Web, nicht im LaTeX: `<webonly>...</webonly>`
Nur im LaTeX, nicht im Web: `<latexonly>...</latexonly>`

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

Einzele Wörter und Wortgruppen lassen sich mit dem Stern hervorheben:

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
QSOs
```

QSOs können ebenfalls wiedergegeben werden. qso_own sind die Funksprüche der einen Station und qso_other für die Gegenstation:

```
[qso_own:CQ CQ DE DL1PZ K]
[qso_other:DL1PZ DO2MAX U R 59 K]
```

## Kommentare

Kommentare gehen weiterhin per %-Zeichen, aber nur am Anfang der Zeile! TODO als Markierung für offene Aufgaben.

```
% TODO Der Absatz muss neu formuliert werden
```

## Zeichnungen

Die Zeichnungen werden durch LaTeX und TikZ umgesetzt. Hierbei kommt insbesondere die Bibliothek [CircuiTikZ](https://ctan.org/pkg/circuitikz?lang=de) zum Einsatz. Ein direktes modifizieren der SVG-Dateien ist nicht vorgesehen.

TODO: PYTHON SCRIPT TIKZ2SVG

## Links

Hyperlinks sollten immer über den 50ohm.de-URL-Shortener abgebildet werden. 

## Lizenz und Pull-Request

Die Inhalte stehen unter der [CC BY 4.0 Lizenz](https://creativecommons.org/licenses/by/4.0/deed.de)

== Hinweis zur Namensnennung (CC BY)

Bei der Verwendung der Materialien auf 50ohm.de müssen angemessene Urheber- und Rechteangaben gemacht sowie ein Link zur verwendeten Lizenz beigefügt werden. Zudem ist anzugeben, ob Änderungen an den Materialien vorgenommen wurden.

Diese Angaben dürfen in jeder angemessenen Art und Weise erfolgen, jedoch nicht so, dass der Eindruck entsteht, der Lizenzgeber unterstütze oder befürworte die jeweilige Nutzung in besonderer Weise.

Bitte nennen Sie als Urheber:

```
50ohm.de – Autorenteam Koordiniert durch das AJW-Referat des DARC e. V.

Matthias Amberg (DG4MA), Henrik Bartels (DL6OCH), Jan Behrens (DL9JBE), Helmut Berka (DL2MAJ), Mathias Dahlke (DJ9MD), Michael Danowski (DK6QW), Christian Dasch (DO1CMD), Sabrina Deharde (DO7XK), Lucas Ebersberger (DA1EE), Klaus Finkenzeller (DL5MCC), Christoph Fischer (DC6GF), Michael Funke (DL4EAX), Tim Grelka (DA2TG), Michael Groni (DB7YI), Prof. Dr. Michael Hartje (DK5HH), Christian Hillmer (DM7EE), Ronny Jerke (DG2RON), Prof. Dr. Matthias Jung (DL9MJ), Thomas Kamp (DF5JL), Erich Kless (DD4UQ), Karlheinz Krause (DL4DBY), Stephan Kregel (DG1HXJ), Dr. Andreas Krüger (DJ3EI), Michael Lowack (DK1KC), Rüdiger Maaß (DF7LYN), Daniel Mittendorf (DK5WP), Michael Moller (DG9NDT), Christian Reiber (DL8MDW), Harald Rode (DL4HR), Florian Schmid (DL1FLO), Prof. Dr. Herrmann Schumacher (DF2DR), Alexander Schumacher (DL1ASN), Marco Schwan (DC8WAN), Prof. Dr. Klaus Solbach (DK3BA), Björn Swierczek (DL1PZ), Aaron Thielmann (DB9TT), Carmen Weber (DM4EAX), Lars Weiler (DC4LW), Daniel Wendt-Fröhlich (DL2AB), Severin Wiedemann (DL9SW)
```

### Prüfungsfragen

Die enthaltenen Prüfungsfragen sind dem amtlichen Fragenkatalog entnommen: Prüfungsfragen zum Erwerb von Amateurfunkprüfungsbescheinigungen, Bundesnetzagentur, 3. Auflage, März 2024, (www.bundesnetzagentur.de/amateurfunk), [Datenlizenz Deutschland – Namensnennung – Version 2.0](https://www.govdata.de/dl-de/by-2-0)

Am Fragenkatalog, welcher in Kooperation mit der Bundesnetzagentur entstand, waren und sind folgende Personen von Seiten des DARC e. V. beteiligt:

```
Fabian Amann (DC1SAF), Matthias Amberg (DG4MA), Henrik Bartels (DL6OCH), Jan Behrens (DL9JBE), Michael Berger (DF7SA), Helmut Berka (DL2MAJ), Dr.-Ing. Hartmut Büttig (DL1VDL), Mathias Dahlke (DJ9MD), Michael Danowski (DK6QW), Sabrina Deharde (DO7XK), Hendrik Dietrich (DG3HDA), Marcus Engelmann (DL2DCX), Klaus Finkenzeller (DL5MCC), Christian Frieß (DL2MDU), Michael Funke (DL4EAX), Michael Gebhardt (DM1CHL), Lukas Greiner (KN6PSU), Michael Groni (DB7YI), Prof. Dr.-Ing. Michael Hartje (DK5HH), Gerrit Herzig (DH8GHH), Thomas Hillen (DF2TH), Christian Hillmer (DM7EE), Martin Jerabek (DK1MJ), Ronny Jerke (DG2RON), Prof. Dr.-Ing. Matthias Jung (DL9MJ), Klaus Jung (DL5KJ), Thomas Kamp (DF5JL), Erich Kless (DD4UQ), Peter Kornherr (DK4KP), Karlheinz Krause (DL4DBY), Stephan Kregel (DG1HXJ), Dr. Andreas Krüger (DJ3EI), Martin Kuhn (DL3SFB), Stefan Lampprecht (DL1SL), Manfred Lauterborn (DK2PZ), Markus Lör (DO2MLS), Michael Lowack (DK1KC), Jürgen Lutz (DK3OL), Hannes Matuschek (DM3MAT), Günther Mildenberger (DL4BX), Daniel Mittendorf (DK5WP), Michael Moller (DG9NDT), Roy Muselick (DM4ET), Andreas Nützel (DG4MIC), Ralph Oppelt (DL2NDO), Dr.-Ing. Henning Paul (DC4HP), Marei Peischl, Peter Pfann (DL2NBU), Christian Reiber (DL8MDW), LL.B. Lukas Reinhardt (DO7VLR), Harald Rode (DL4HR), Uwe Rüdiger (DG2DBF), Paul Schimanski (DF4ZL), Florian Schmid (DL1FLO), Werner Schmidt (DL4YBZ), Malte Schmitz (DE7LMS), Stefan Scholl (DC9ST), Alexander Schumacher (DL1ASN), Marco Schwan (DC8WAN), Björn Swierczek (DL1PZ), Aaron Thielmann (DB9TT), Jann Traschewski (DG8NGN), Alexander Vidoni (DK6AV), Werner Vollmer (DF8XO), Carmen Weber (DM4EAX), Michael Weber (DL1XMW), Lars Weiler (DC4LW), Wolfgang Welter (DL2KBJ), Daniel Wendt-Fröhlich (DL2AB), Severin Wiedemann (DL9SW), Udo Witte (DJ4FV), Dipl.-Ing. Claus-Dieter Wittek (DF8QJ), Bernhard Zimmermann (DG3BZ)
```

### Pull-Requests

Durch einen Pull-Request akzeptiert man autoamtisch die CC BY Lizenzbedingungen.

Wir behalten uns im Sinne der Qualitätssicherung sowie zur Einhaltung der Vorgaben des vom DARC e. V. entwickelten Lehrplans und der Philosophie von 50ohm.de vor, eingereichte Pull Requests abzulehnen oder zu modifizieren.

# Kontakt

Verantwortlich für das Betreiben von 50ohm.de ist das AJW-Referat des DARC e. V. in Baunatal. Bei Anfragen bitte die Email-Adresse [50ohm@darc.de](mailto:50ohm@darc.de) nutzen. Weiterhin findet man viele der Beitragenden im Matrix-Kanal [Ausbilder-Netzwerk](https://matrix.to/#/#AusbilderNetzwerk:darc.de).