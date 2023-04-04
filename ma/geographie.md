{% include mathe.html %}
# Geometrie

## Koordinatensystem
besteht aus $$x_1$$-,$$x_2$$- und $$x_3$$-Achsen und acht Oktanten (deren genaue Position man sicher im Internet recherchieren kann)

## Vektoren
(= Menge seiner Repräsentanten)  
→ bestimmte Richtung und Länge  
→ Tripel dreier Koordinaten: $$\vec{a}=\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix}$$

Besondere Vektoren:
- Nullvektor (Ursprung): $$\vec{0}=\begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}$$
- Gegenvektor zu $$\vec{a}$$: $$-\vec{a}$$
- Ortsvektor: $$\overrightarrow{0A}=\vec{A}$$ (vom Ursprung zum eigentlichen Punkt)
- Verbindungsvektor: $$\overrightarrow{AB}=\vec{B}-\vec{A}$$ („Spitze minus Fuß”)
- Vektorkette: $$\overrightarrow{AB}+\overrightarrow{BC}+\overrightarrow{CD}=\overrightarrow{AD}$$
- Einheitsvektor (Länge 1): $$\vec{a^0}=\frac{1}{\mid\vec{a}\mid}\cdot \vec{a} \Rightarrow\mid\vec{a^0}\mid=1$$

- Länge eines Vektors: $$\mid\vec{a}\mid=\mid\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}\mid=\sqrt{a_1\,^2+a_2\,^2+a_3\,^2}$$ (Pythagoras im dreidimensionalen Raum)  
- Kommutativ- und Assoziativgesetz gelten  
- Skalarmultiplikation ($$s \in \mathbb{R}$$ ist ein Skalar): $$s\cdot\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}=\begin{pmatrix} s\cdot a_1 \\ s\cdot a_2 \\ s\cdot a_3 \end{pmatrix}$$  
  → mit Assoziativ- und Distributivgesetz
- lineare Abhängigkeit:
  - bei zwei Vektoren: Vielfaches voneinander ($$\vec{a}=r\cdot\vec{b}$$)
  - bei drei Vektoren: Linearkombination ($$\vec{a}=r\cdot\vec{b}+s\cdot\vec{c}$$)  
  (sonst: „linear unabhängig”)

### Skalarprodukt
$$\vec{a}\circ\vec{b}=\cdot\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}\circ\begin{pmatrix} b_1 \\ b_2 \\ b_3 \end{pmatrix}=a_1b_1+a_2b_2+a_3b_3$$  

- Winkel zwischen zwei Vektoren: $$\cos(\varphi)=\frac{\vec{a}\circ\vec{b}}{\mid\vec{a}\mid\cdot\mid\vec{b}\mid}$$
- 90&deg;-Winkel wenn $$\vec{a}\circ\vec{b}=0$$

### Vektorprodukt/Kreuzprodukt
$$\vec{a}\times\vec{b}=\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}\times\begin{pmatrix} b_1 \\ b_2 \\ b_3 \end{pmatrix}=\begin{pmatrix} a_2b_3-a_3b_2 \\ a_3b_1-a_1b_3 \\ a_1b_2-a_2b_1 \end{pmatrix}$$  

- rechtshändiges Dreibein (vgl. Rechte-Hand-Regel) → dritter Vektor steht im 90&deg;-Winkel zu den anderen beiden Vektoren
- anti-kommutativ: $$\vec{a}\times\vec{b}=-\vec{b}\times\vec{a}$$
- Winkel zwischen zwei Vektoren: $$\sin(\varphi)=\frac{\vec{a}\times\vec{b}}{\mid\vec{a}\mid\cdot\mid\vec{b}\mid}$$
- Flächeninhalt eines von $$\vec{a}$$ und $$\vec{b}$$ aufgespannten Parallelogramms: $$A_{Par}=\mid\vec{a}\times\vec{b}\mid$$
- Flächeninhalt eines von $$\vec{a}$$ und $$\vec{b}$$ aufgespannten Dreiecks: $$A_\Delta=\frac{1}{2}\mid\vec{a}\times\vec{b}\mid$$
- *Volumen eines $$\vec{a}$$, $$\vec{b}$$ und $$\vec{c}$$ aufgespannten Spats: $$V_{Spat}=\mid(\vec{a}\times\vec{b})\circ\vec{c}\mid$$*
- Volumen einer von $$\vec{a}$$, $$\vec{b}$$ und $$\vec{c}$$ aufgespannten, dreiseitigen Pyramide: $$V_{Pyr}=\frac{1}{6}\mid(\vec{a}\times\vec{b})\circ\vec{c}\mid$$
- *Volumen einer von $$\vec{a}$$, $$\vec{b}$$ und $$\vec{c}$$ aufgespannten Pyramide mit einem Parallelogramm als Grundfläche: $$V_{Pyr}=\frac{1}{3}\mid(\vec{a}\times\vec{b})\circ\vec{c}\mid$$*  
→ Dreieck und dreiseitige Pyramide in der [Formelsammlung](https://www.isb.bayern.de/download/13107/merkhilfe_fuer_das_fach_mathematik_standard.pdf){:target="_blank"}

## Kugel
- Mittelpunkt $$\vec{M}$$, Radius $$r$$
- Oberflächeninhalt: $$A=4\pi\cdot r^2$$
- Volumen: $$V=\frac{4}{3}\pi\cdot r^3$$
- Formel: $$\overline{XM}=r \text{ (Die Strecke von jedem Punkt auf der Kugel bis zu ihrem Mittelpunkt ist so lang wie der Radius.)}\\\\\Rightarrow\mid\overrightarrow{XM}\mid=r\\\\\Rightarrow\sqrt{(m_1-x_1)^2+(m_2-x_2)^2+(m_3-x_3)^2}=r\\\\\Rightarrow(m_1-x_1)^2+(m_2-x_2)^2+(m_3-x_3)^2=r^2$$ (Koordinatenform)

## Geraden
- Geradengleichung in Parameterform:  
  $$g:\vec{X}=\vec{A}+\lambda\cdot\vec{u}$$  
  ($$\vec{A}$$: Aufpunkt; $$\lambda$$: Parameter; $$\vec{u}$$: Richtungsvektor)  
  → Gerade kann durch einen Aufpunkt und einen Richtungsvektor oder durch zwei Punkte ($$\vec{u}=\overrightarrow{AB}$$) definiert werden
- Geradengleichung kann auch zeilenweise geschrieben werden:  
$$
g:\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix}=\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}+\lambda\cdot\begin{pmatrix} u_1 \\ u_2 \\ u_3 \end{pmatrix}\\
\Downarrow\\
(I)\ x_1=a_1+\lambda\cdot u_1\\
(II)\ x_2=a_2+\lambda\cdot u_2\\
(III)\ x_3=a_3+\lambda\cdot u_3\\
$$

- Spurpunkte: Schnittpunkte mit den Koordinatenebenen (eine Gleichung gleich $$0$$ setzen und $$\lambda$$, dann den Punkt bestimmen)

## Ebenen
- Ebenengleichung in Parameterform:  
  $$E:\vec{X}=\vec{A}+\lambda\cdot\vec{u}+\mu\cdot\vec{v}$$  
  ($$\vec{A}$$: Aufpunkt; $$\lambda$$, $$\mu$$: Parameter; $$\vec{u}$$, $$\vec{v}$$: Richtungsvektoren)  
  → Gerade kann durch einen Aufpunkt und zwei Richtungsvektoren oder durch drei Punkte ($$\vec{u}=\overrightarrow{AB}$$ und $$\vec{v}=\overrightarrow{AC}$$) definiert werden
- Ebenengleichung in Normalenform:  
  $$E:\vec{n}\circ(\vec{X}-\vec{A})=0$$ (der Normalenvektor muss senkrecht auf dem Verbindungsvektor von einem beliebigen Punkt auf der Ebene und dem Aufpunkt stehen)  
  mit $$\vec{n}=\vec{u}\times\vec{v}$$  
  → Gerade kann durch einen Aufpunkt und einen Normalenvektor definiert werden
- Ebenengleichung in Koordinationform:  
  Normalenform ausmultiplizieren:  
$$
E:\vec{n}\circ(\begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix}-\begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix})=0\\
E:n_1x_1+n_2x_2+n_3x_3-(n_1a_1+n_2a_2+n_3a_3)=0\\
E:n_1x_1+n_2x_2+n_3x_3-c=0
$$
  - zurück zu Normalenform: Normalenvektor mit Vorfaktoren bestimmen; für den Aufpunkt irgendeinen Punkt, der die Gleichung der Koordinatenform erfüllt, einsetzen
  - zurück zu Parameterform: beliebigen Aufpunkt nehmen; $$\vec{u}$$ und $$\vec{v}$$ bestimmen, indem (pro Richtungsvektor) eine Koordinate von $$\vec{n}$$ gleich $$0$$ gesetzt wird, die anderen vertauscht werden und bei einer von diesen das Vorzeichen geändert wird

- Koordinatenebenen: z.B. $$x_1x_2$$-Ebene mit $$\vec{n}=\begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$$
- Spurpunkte: Schnittpunkte mit den Koordinatenachsen (in Koordinatenform zwei Variablen gleich $$0$$ setzen und die übrige bestimmen)

## Lagebeziehungen

### Gerade-Gerade
- Richtungsvektoren linear abhängig
  - Aufpunkt einer Gerade auch auf der anderen (zeilenweise einsetzen)  
    → identisch
  - Aufpunkt einer Gerade nicht auch auf der anderen (zeilenweise einsetzen)  
    → parallel
- Richtungsvektoren linear unabhängig
  - haben Schnittpunkt (zeilenweise gleichsetzen)  
    → Schnittpunkt
  - haben keinen Schnittpunkt (zeilenweise gleichsetzen)  
    → windschief

### Gerade-Ebene
- Schnittpunkt berechnen → „zeilenweise” Geradengleichung in Koordinatenform der Ebene einsetzen
  - allgemeingültige Gleichung  
    → Gerade liegt in der Ebene
  - Wert für $$\lambda$$  
    → in Gerade einsetzen, um Schnittpunkt zu erhalten
  - Widerspruch (z.B. $$1=0$$) 
    → sind parallel zueinander (schneiden sich nicht)

### Ebene-Ebene
- Normalenvektoren linear abhängig
  - Aufpunkt einer Ebene auch in der anderen  
    → identisch
  - Aufpunkt einer Ebene nicht auf der anderen  
    → parallel
- Normalenvektoren nicht linear abhängig  
  → schneiden sich

### Schnittwinkel
Vektoren $$\vec{u}$$ und $$\vec{v}$$ (bei Geraden: Richtungsvektoren; bei Ebenen: Normalenvektoren)  
$$\varphi=\arccos(\mid\frac{\vec{u}\circ\vec{v}}{\mid\vec{u}\mid\cdot\mid\vec{v}\mid}\mid)\\$$  
Achtung! Zwischen Ebene und Gerade beträgt der Schnittwinkel $$90^\circ-\varphi$$

### Abstand Punkt-Gerade
- kürzeste Strecke zwischen Punkt $$\vec{P}$$ und Gerade $$g$$ ist das Lot auf der Gerade zum Punkt  
  → Strecke muss senkrecht auf Richtungsvektor stehen  
  → $$\overrightarrow{PX}\circ\vec{u}$$  
  → ausmultiplizieren → Gerade zeilenweise einsetzen → nach $$\lambda$$ auflösen → in Geradengleichung eingesetzt Punkt $$\vec{X}$$ herausfinden  
  → $$d(P;g)=\mid\overrightarrow{PX}\mid$$

### Abstand Punkt-Ebene
Hesse-Normalform (HNF): Normalenvektor muss ein Einheitsvektor sein  
→ $$E: \frac{n_1x_1+n_2x_2+n_3x_3-c}{\mid\vec{n}\mid}=0$$  
→ bis auf Vorzeichen eindeutig

Für den Abstand zur Ebene den Punkt in die linke Seite einsetzen:  
$$d(P; E)=\frac{n_1x_1+n_2x_2+n_3x_3-c}{\mid\vec{n}\mid}$$  
→ falls positiv, liegt der Punkt auf der Seite von $$\vec{n}$$  
→ Abstand ist aber eigentlich der Betrag