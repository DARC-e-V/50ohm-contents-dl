Ein ideales rein sinusförmiges Signal besteht nur aus seiner *Grundwelle* welche auch *1. Harmonische* genannt wird. Sobald ein Signal nicht mehr der Sinusform entspricht und auch nur leicht davon abweicht, enthält das Signal *ganzzahlige Vielfache* seiner Grundschwingung, die auch *Oberwellen oder Oberschwingungen* genannt werden. Hierbei ist es wichtig zwischen den beiden Begriffen Oberwellen und Harmonischen zu differenzieren.

Die Abbildung [ref:zusammenhang_oberwellen_harmonische] und die Tabelle [ref:a_harmonische] zeigt den Zusammenhang zwischen Oberwellen und Harmonischen, den man sich nur einmal einprägen muss. Die 1. Oberwelle entspricht hierbei der 2. Harmonischen der Grundschwingung und befindet sich auf der doppelten Frequenz der Grundschwingung. Die 2. Oberwelle entspricht der 3. Harmonischen der Grundschwingung und befindet sich auf der dreifachen Frequenz der Grundschwingung. Nach diesem Prinzip werden alle Harmonischen und Oberwellen auf die Grundwelle bezogen und mit einer Ordnungszahl $N$ durchnummeriert.

<margin>
[picture:869:zusammenhang_oberwellen_harmonische:Zusammenhang zwischen Oberwellen und Harmonischen]

| l: Vielfaches der Grundfrequenz | l: Harmonische | l: Oberwelle |
| $f_0$ | 1 | ~ |
| $2 \cdot f_0$ | 2 | 1 |
| $3 \cdot f_0$ | 3 | 2 |
| $4 \cdot f_0$ | 4 | 3 |
[table:a_harmonische:Harmonische und Oberwellen]
</margin>

<indepth>
Je nach Art der Verzerrung eines Signals entstehen im Verhältnis mehr geradzahlige oder ungeradzahlige Oberwellen in dessen Frequenzspektrum. Rechteckförmige Signale, welche z.B. durch Übersteuerung von Verstärkerstufen entstehen (hierbei werden die Spitzen der Amplituden begrenzt und abgeflacht), enthalten ungeradzahlige Harmonische bzw. geradzahlige Oberwellen.

<webonly>
[include:applet_rectangle]

An den Sprungstellen zeigt die Fourier-Näherung das sogenannte Gibbs-Phänomen: Selbst bei sehr vielen Harmonischen bleibt dort ein kleines Über- und Unterschwingen bestehen.
</webonly>

Sägezahnförmige Signale enthalten überwiegend geradzahlige Harmonische bzw. ungeradzahlige Oberwellen.
</indepth>

[question:AB403]
[question:AB401]
[question:AB402]

Ist die Grundfrequenz eines Signals bekannt, ergibt sich die Frequenz der $N$-ten Harmonischen durch Multiplikation der Grundfrequenz mit der Ordnungszahl $N$:

$f_N = N \cdot f_0$

Für die $N$-te Oberwelle gilt dagegen:

$f_\mathrm{Oberwelle,N} = (N+1)\cdot f_0$

[question:AJ201]
[question:AJ205]
[question:AJ202]
[question:AJ206]

Auch wenn ein Signal auf dem Oszilloskop zunächst sinusförmig erscheint, kann das Signal trotzdem nennenswerte Oberwellenanteile (bzw. Harmonische der Grundwelle) enthalten. Um den Oberwellenanteil eines Signals quantitativ und qualitativ beurteilen zu können benötigt man einen *Spektrumanalysator* der das Signal im Frequenzbereich (Frequency-Domain) darstellen kann und hierbei die Amplitudenwerte der einzelnen Oberwellen logarithmisch darstellen kann, so dass deren Anteile am Gesamtsignal messbar sind.

[question:AI615]
[question:AI614]
