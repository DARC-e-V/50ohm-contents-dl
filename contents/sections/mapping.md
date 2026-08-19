Bei digitalen Übertragungsverfahren müssen die zu übertragenden Bits den verschiedenen möglichen Symbolen zugeordnet werden. Diese Zuordnung wird als *Mapping* bezeichnet. Der Baustein, der diese Zuordnung vornimmt, wird als *Mapper* bezeichnet. Das Blocksymbol eines Mappers ist in Abbildung [ref:a_mapper] dargestellt. Der Mapper nimmt einen digitalen Bitstrom entgegen und ordnet die enthaltenen Bitkombinationen den entsprechenden Symbolen in einem Konstellationsdiagramm zu.

<margin>
[picture:1102:a_mapper:Blockschaltbild eines Mappers]
</margin>

---

Um das Prinzip des Mappings kennenzulernen, betrachten wir zunächst die bereits aus Klasse E bekannte *Amplitudenumtastung* (*Amplitude-Shift Keying*, ASK). Die Abbildung [ref:a_ask] zeigt eine binäre ASK in der Zeitdarstellung. Dabei wird die Amplitude des Trägersignals zwischen zwei Werten umgeschaltet. Beispielsweise kann eine große Amplitude das Bit $1$ und eine kleine Amplitude das Bit $0$ darstellen.

<margin>
[picture:700:a_ask:ASK (Amplitude-Shift Keying) im zeitlichen Verlauf]
</margin>

---

Die beiden möglichen Symbole lassen sich auch in dem zuvor kennengelernten Konstellationsdiagramm darstellen. Da sich bei diesem Beispiel nur die Amplitude ändert und die Phasenlage gleich bleibt, liegen beide Signalpunkte auf der I-Achse. Der unterschiedliche Abstand vom Ursprung entspricht den beiden unterschiedlichen Amplituden. Jedem der beiden Signalpunkte wird nun über das Mapping ein Bitwert zugeordnet.

<margin>
[picture:1128:a_ask_mapping:ASK (Amplitude-Shift Keying) im Konstellationsdiagramm]
</margin>

---

Eine Amplitudenumtastung ist nicht auf zwei mögliche Amplituden beschränkt. Werden beispielsweise vier unterschiedliche Amplituden verwendet, stehen vier verschiedene Symbole zur Verfügung. Da sich mit zwei Bits vier unterschiedliche Bitkombinationen bilden lassen, kann jedem Symbol eine der Kombinationen $00$, $01$, $10$ oder $11$ zugeordnet werden.

Die Abbildung [ref:a_4_ask] zeigt eine solche *4ASK* mit vier unterschiedlichen Amplituden in der Zeitdarstellung. Beispielsweise können $\qty{25}{\percent}$, $\qty{50}{\percent}$, $\qty{75}{\percent}$ und $\qty{100}{\percent}$ der maximalen Amplitude verwendet werden. Mit jedem Symbol können dadurch zwei Bits übertragen werden.

<margin>
[picture:701:a_4_ask:Quaternäre Amplitudenumtastung (Quaternary Amplitude-Shift Keying)]
</margin>

Auch im Konstellationsdiagramm sind nun vier mögliche Signalpunkte vorhanden. Da sich weiterhin nur die Amplitude ändert, liegen in diesem Beispiel alle vier Punkte auf der I-Achse. Jedem Punkt ist eine bestimmte Bitkombination zugeordnet.

<margin>
[picture:1129:a_4_ask_mapping:Quaternäre Amplitudenumtastung (Quaternary Amplitude-Shift Keying) im Konstellationsdiagramm]
</margin>
