{% include mathe.html %}
# Analysis

## Differenzieren

### Mittlere Änderungsrate
Der Differenzenquotient $$\frac{\Delta y}{\Delta x}=\frac{f(b)-f(a)}{b-a}$$ ist die mittlere Änderungsrate.  
&#x2259; Steigung der Sekante zwischen $$(a|f(a))$$ und $$(b|f(b) )$$

### Lokale Änderungsrate
Lokale Änderungsrate von $$f$$ an der Stelle $$a$$:
„Differentialquotient” $$\lim\limits_{h \to 0} \frac{f(a+h)-f(a)}{h}$$  
&#x2259; Steigung der Tangente von $$f$$ bei $$x=a$$ bzw. $$f'(a)$$

→ existiert der Grenzwert (für positives und negatives h), ist $$f$$ an der Stelle $$a$$ **differenzierbar** („knickfrei”)

### Ableitungsfunktion
Die Ableitungsfunktion $$f'(x)$$ ordnet jedem x-Wert von $$f(x)$$ die dortige Steigung von f zu.

|$$F$$|Stammfunktion (von $$f$$)|
|$$f$$|(Normal)funktion|
|$$f'$$|Ableitung(sfunktion) (von $$f$$)|

$$f'(x)=\lim\limits_{h \to 0}{\frac{f(x+h)-f(x)}{h}}=\frac{df}{dx}$$

### Ableitungsregeln

|Regel|Normalfunktion|Ableitung|
|-----|--------------|---------|
|Addition einer Konstante|$$f(x)=g(x)+c$$|$$f'(x)=g'(x)$$|
|Summenregel|$$f(x)=u(x)+v(x)$$|$$f'(x)=u'(x)+v'(x)$$|
|Produktregel|$$f(x)=u(x)\cdot v(x)$$|$$f'(x)=u'(x)\cdot v(x)+u(x)\cdot v'(x)$$|
|Quotientenregel|$$f'(x)=\frac{z(x)}{n(x)}$$|$$f(x)=\frac{„NAZ - ZAN”}{„N^2”}=\frac{n(x)\cdot z'(x)-z(x)\cdot n'(x)}{(n(x))^2}$$|
|Kettenregel|$$f(x)=u(v(x))$$|$$f'(x)=u'(v(x))\cdot v'(x)$$<br/>($$v'(x)$$: „Nachdifferenzieren”)|

## Integrieren
„Berechnung der Fläche unter $$G_f$$”  
→ $$f(x)$$ ist die **Integrandenfunktion**  
→ Unter- ($$s_n$$) und Obersumme ($$S_n$$): Fläche mit $$n$$ Rechtecken/„Streifen” annähern  
→ Fläche unterhalb der x-Achse negativ, oberhalb positiv!


$$\int\limits_a^b f(x) dx$$
(**Bestimmtes Integral** über $$f(x)$$ mit unterer Grenze $$a$$ und oberer Grenze $$b$$)  
= $$\lim\limits_{n \to \infty} s_n$$ (Untersumme)  
= $$\lim\limits_{n \to \infty} S_n$$ (Obersumme)  
→ Unter- und Obersumme nähern sich (bei $$n \to \infty$$) demselben Grenzwert an

### Hauptsatz der Differential- und Integralrechnung
**Integralfunktion** $$I_a(x)=\int\limits_a^x{f(t)dt}$$  
→ ergibt abgeleitet die Integrandenfunktion: $$I_a'(x) = f(x)$$  
→ Nullstelle bei $$I_a(a)$$  
→ jede Integrandenfunktion von $$f$$ ist eine Stammfunktion,  
  aber nur Stammfunktionen mit mindestens einer Nullstelle sind Integrandenfunktionen  

→ **Die Integration ist die Umkehrung der Differentiation!**

**Unbestimmtes Integral** $$\int{f(x)dx}=F(x)+c$$ mit $$c \in \mathbb{R}$$  
→ Menge aller Stammfunktionen zu $$f$$

Berechnung des bestimmten Integrals:  
$$\int\limits_a^b{f(x)dx}=[F(x)]_a^b=F(b)-F(a)$$

### Integrationsregeln

|Regel|Rechnung|
|Abschnittsweise Integration|$$\int\limits_a^b{f(x)dx}+\int\limits_b^c{f(x)dx}=\int\limits_a^c{f(x)dx}$$|
|Vertauschen der Grenzen|$$\int\limits_b^a{f(x)dx}=-\int\limits_a^b{f(x)dx}$$|
|Untere und obere Grenze gleich|$$\int\limits_a^a{f(x)dx}=0$$|
|Summenregel|$$\int{f(x)+g(x)dx}=\int{f(x)dx}+\int{g(x)dx}$$|
|Faktorregel|$$\int{k \cdot f(x)dx}=k \cdot \int{f(x)dx}$$|
|Lineare Transformation|$$\int{f(ax+b)dx}=\frac{1}{a}\cdot F(ax+b)+c$$|
|e-Funktion|$$\int{f'(x)\cdot e^{f(x)}dx}=e^{f(x)}+C$$<br/>(auch mit Faktorregel kombinierbar)|
|Brüche|$$\int{\frac{f'(x)}{f(x)}dx}=\ln(\|f(x)\|)+c$$|

## Besondere Funktionen

|Stammfunktion|Normalfunktion|Ableitungsfunktion|
|$$\frac{1}{r+1}\cdot x^{r+1} + c$$|$$x^r$$|$$r\cdot x^{r-1}$$|
|$$-\cos(x)+c$$|$$\sin(x)$$|$$\cos(x)$$|
|$$\sin(x)+c$$|$$\cos(x)$$|$$-\sin(x)$$|
|$$e^x+c$$|$$e^x$$|$$e^x$$|
|$$\ln\|x+c\|$$|$$\frac{1}{x}$$|$$-x^{-2}$$|
|$$\ln(x)\cdot x-x+c$$|$$\ln(x)$$|$$\frac{1}{x}$$|
|$$$$|$$$$|$$$$|

## Steigungswinkel
Für den Winkel zwischen der x-Achse und der Tangente von $$f$$ an der Stelle $$a$$ gilt:

$$tan(\alpha) = m$$  
→ $$\alpha=\arctan(m)=\arctan(f'(a))$$

## Monotonie
- $$G_f$$ ist s.m.s. (streng monoton **steigend**) in einem Intervall, wenn $$f'(x)$$ dort **positiv** ist.
- $$G_f$$ ist s.m.f. (streng monoton **fallend**) in einem Intervall, wenn $$f'(x)$$ dort **negativ** ist.  
→ Umkehrung gilt nicht (s. $$f'(x)=0$$)

## Extrema und Terrassenpunkte
$$f'(a)=0$$

|Maximum|$$f'$$ wechselt Vorzeichen von + zu -|$$f''(a) < 0$$ (rechtsgekrümmt)|
|Minimum|$$f'$$ wechselt Vorzeichen von - zu +|$$f''(a) > 0$$ (linksgekrümmt)|
|Terrassenpunkt (Sattelpunkt)|$$f'$$ hat keinen Vorzeichenwechsel (gerade Nullstelle)|$$f''(a) = 0$$|

→ Vorzeichentabelle von $$f'(x)$$ und $$G_f$$ (mit Einsetzen bzw. Limites) *oder* Krümmungsverhalten mit zweiter Ableitung

## Symmetrie
- $$f(-x) = f(x)$$: achsensymmetrisch zur y-Achse
- $$f(-x) = -f(x)$$: punktsymmetrisch zum Ursprung  
→ am besten immer erst $$f(-x)$$ berechnen

## Newton-Verfahren
→ Nullstellen herausfinden (geht aber nicht immer)

Beliebiger Startwert $$x_n$$  
→ $$x_{n+1}=x_n-\frac{f(x_n)}{f'(x_n)}$$ als bessere Näherung  
→ damit als Iterationsformel (geht gut am Taschenrechner) weiterrechnen

## Gebrochen-rationale Funktionen
= Bruch mit Polynomen in Zähler und Nenner

### waagrechte/schräge Asymptote

|Zählergrad < Nennergrad|waagrechte Asymptote $$y=0$$ (x-Achse)|
|Zählergrad = Nennergrad|waagrechte Asymptote (Parallele der x-Achse)|
|Zählergrad = Nennergrad + 1|schräge Asymptote (lineare Funktion)|

(bei höherem Nennergrad sind auch andere Funktionen möglich)

→ berechenbar mit $$\lim\limits_{x \to \pm \infty}$$ *oder* durch Aufteilen in linearen Summanden und gebrochen-rationalen Summanden (mit Zählergrad < Nennergrad)

### Polstelle
Polstelle liegt dort, wo eine Definitionslücke ($$„Nenner” = 0$$) ist  
→ z.B. bei Definitionslücke $$x_0$$ von $$f$$ liegt die Polstelle bei $$x=x_0$$ (senkrechte Asymptote)

$$\lim\limits_{x \to x_0}{f(x)}=\pm \infty$$

Achtung: Bei einer **(be)hebbaren Definitionslücke** (die herausgekürzt werden kann, sodass nur ein „Loch” im Graphen übrig bleibt)
gibt es keine Polstelle!

## Umkehrbarkeit
„Spiegelung einer Funktion an der Winkelhalbierenden des I. und III. Quadranten”  
→ bei $$x^2$$ ist die Umkehrfunktion $$\sqrt{x}$$ (negativer Ast wird ausgelassen!)

Eine Funktion ist in einem Intervall eindeutig **umkehrbar**, wenn sie in diesem **streng monoton** steigt bzw. fällt.  
→ Berechnung durch Vertauschen von $$x$$ und $$y$$, dann Umformung.

|Funktion|Umkehrfunktion|
|$$f(x)$$|$$f^{-1}(x)$$|
|$$\mathbb{D}_f$$|$$\mathbb{D}_{f^{-1}}=\mathbb{W}_f$$|
|$$\mathbb{W}_f$$|$$\mathbb{W}_{f^{-1}}=\mathbb{D}_f$$|

## e-Funktion und natürlicher Logarithmus
$$e \approx 2,71828$$ (irrationale Zahl wie $$\pi$$)  
($$e = \lim\limits_{n \to \infty}{(1+\frac{1}{n})^n}$$)  
→ Besonderheit: Die e-Funktion/natürliche Exponentialfunktion ($$e^x$$) ist ihre eigene Ableitung.  

Ableiten: $$(e^{f(x)})' = e^{f(x)}\cdot f'(x)$$ mit „Sonderfall” $$(e^x)' = e^x$$

Der natürliche Logarithmus (***l**ogarithmus **n**aturalis*) $$\log_e(x)=\ln(x)$$ ist die Umkehrfunktion der natürlichen Exponentialfunktion $$e^x$$.  
→ $$\ln(e^x)=x$$

Die e-Funktion steigt sehr schnell, der natürliche Logarithmus sehr langsam.  
→ relevant bei Grenzwertaufgaben („e-Funktion gewinnt immer”, „ln verliert immer”)

Weitere Exponentialfunktionen (mit konstanter Basis $$c$$) ableiten:  
$$(c^x)'=((e^{\ln(c)})^x)'=(e^{\ln(c) \cdot x})'=\ln(c) \cdot e^{\ln(c) \cdot x} = \ln(c) \cdot c^x$$

## Krümmungsverhalten
Die zweite Ableitung einer Funktion beschreibt deren Krümmung (= Abweichung von einer Gerade).  
- $$f$$ ist linksgekrümmt, wenn $$f''$$ positiv ist.
- $$f$$ ist rechtsgekrümmt, wenn $$f''$$ negativ ist.

## Wendepunkt
= Punkt, an dem sich das Vorzeichen der Krümmung ($$f''$$) ändert  
→ Ort maximaler bzw. minimaler Steigung  
(Wendetangente: Steigungstangente am Wendepunkt)

→ $$f''(x)=0$$  
→ auf ungerade Nullstelle überprüfen (Vorzeichentabelle → $$f'''(x) \neq 0$$)

## Flächenberechnung
- mit Annäherung (z.B. geometrische Formen)
- zwischen zwei Funktionen $$f(x)$$ und $$g(x)$$:
  - Schnittpunkte finden: $$f(x)=g(x)$$ (z.B. $$x_1=a; x_2=b; x_3=c$$)
  - abschnittweise integrieren und Beträge addieren: $$A=\mid\int\limits_a^b{f(x)-g(x)dx}\mid+\mid\int\limits_b^c{f(x)-g(x)dx}\mid$$
  
## Integration im Unendlichen
Geometrische Reihe: $$1; \frac{1}{2}; \frac{1}{4}; \frac{1}{8};$$ usw.  
→ endlicher Grenzwert: $$\lim\limits_{n \to \infty}\sum\limits_{k=0}^n{\frac{1}{2^k}}=2$$

Integral im Unendlichen kann auch endlich sein:  
$$\lim\limits_{n \to \infty}\int\limits_1^n{\frac{1}{x^2}dx}=\int\limits_1^\infty{\frac{1}{x^2}}dx=[-x^{-1}]_1^\infty=\lim\limits_{x \to \infty}{(-\frac{1}{x}-(-\frac{1}{1^1})}=0+1=1$$  
→ zweite Notation ohne Limes geläufig
