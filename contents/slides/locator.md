## Problemstellung

* Standort mitteilen, z.B. für Entfernungsmessungen
* Es ist nicht immer eine Stadt in der Nähe
* GPS-Koordinaten sind zu lang
* Oft ist ein ungefährer Standort ausreichend

---

## Maidenhead-Locator

* Erdoberfläche wird in $\num{18662400}$ Kästchen eingeteilt
* Ein Kästchen entspricht in Deutschland grob einer Genauigkeit von $\qty{5}{\kilo\meter}\times\qty{5}{\kilo\meter}$
* Diese Kästchen werden Subsquares genannt
* Übergeordnet sind Squares und Fields

<note>
* nach der *Stadt Maidenhead* benannt, die westlich von London im Vereinigten Königreich liegt.
* Dort fand 1980 eine Fachkonferenz der IARU statt, die das zuvor genutzte QRA-Locator-System reformierte.
</note>

---
[photo:2:n_locator_jo:Das Feld JO des Maidenhead-Locator-Systems, Kartendaten © OpenStreetMap-Mitwirkende, SRTM. Kartendarstellung © OpenTopoMap (CC-BY-SA)]

<note>
Es sind die Fields des Squares JO gezeigt
</note>

--- style="font-size: 0.7em;"
## Stufen des Maidenhead Locators

| X: Bezeichnung | l: Übersetzung | l: Alternative Bez. | c: | c: z.B. |
| Field | Feld | Größtfeld | AA-RR | JO |
| Square | Quadrat | Großfeld | 00-99 | 41 |
| Subsquare | Unter-Quadrat | Kleinfeld | AA-XX | RG |
[table:n_locator_stufen:Die einzelnen Stufen des Maidenhead-Locators]

<fragment>
Daraus ergibt sich dann zum Beispiel *JO41RG* für die DARC Geschäftsstelle in Baunatal bei Kassel
</fragment>
<note>
* Noch kleinere Felder sind möglich
* [Interaktive Karte](https://f5len.org/tools/locator/)
</note>

---
[question:BE111]

