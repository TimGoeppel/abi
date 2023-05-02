{% include mathe.html %}
# Stochastik

## Grundbegriffe
- Menge bzw. Ereignis $$A$$ mit Elementen $$a, b, c$$: $$A=\{a;b;c\}$$
- Ereignisraum $$\Omega$$ mit Elementarereignissen $$\omega_n$$: $$\Omega=\{\omega_0;\omega_1;\omega_2;...\}$$
- Schnittmenge $$C$$ von $$A$$ und $$B$$: $$C=A\cap B$$
- Vereinigungsmenge $$C$$ von $$A$$ und $$B$$: $$C=A\cup B$$
- Gegenereignis $$\overline{A}$$ von $$A$$: $$\overline{A}=\Omega \backslash A$$
- Wahrscheinlichkeitsverteilung $$P$$ von Ereignis $$A$$: $$P(A)$$
- Mächtigkeit einer Menge $$A$$: $$\mid A\mid: \text{„Anzahl der Elemente in A”}$$

## Kolmogorow-Axiome
Axiom = „als absolut richtig erkannter Grundsatz”

1. Nicht-Negativität: $$P(A) \geq 0$$
2. Normierung: $$P(\Omega)=1$$
3. Additivität: $$A\cap B=\varnothing \Rightarrow P(A\cup B)=P(A)+P(B)$$

→ z.B. $$P(A\cup B)=P(A)+P(B)-P(A\cap B)$$,  
  $$P(\overline{A})=1-P(A)$$ (bei „3-mal-mindestens-Aufgaben”: $$P(\text{„mindestens einer”})=1-P(\text{„keiner”})$$)

## Gesetze von de Morgan
$$\overline{A\cup B}=\overline{A}\cap\overline{B}$$  
$$\overline{A\cap B}=\overline{A}\cup\overline{B}$$

## Unabhängige Ereignisse
**Bedingte Wahrscheinlichkeit**: $$P_B(A)=\frac{P(A\cap B)}{P(B)}$$ („P von A unter der Bedingung B”)  
Sind die Ereignisse unabhängig voneinander, so müsste das Eintreten von $$B$$ nichts an der Wahrscheinlichkeit von $$A$$ ändern:  
$$P_B(A)=P(A) \Rightarrow P(A\cap B)=P(A)\cdot P(B)$$  
→ ist diese Gleichung erfüllt, sind $$A$$ und $$B$$ **stochastisch unabhängig**, sonst **stochastisch abhängig**.

## Darstellung
Vierfeldertafel (Schnittwahrscheinlichkeiten und totale Wahrscheinlichkeiten):

||$$A$$|$$\overline{A}$$||
|$$B$$|$$P(A\cap B)$$|$$P(\overline{A}\cap B)$$|$$P(B)$$|
|$$\overline{B}$$|$$P(A\cap\overline{B})$$|$$P(\overline{A}\cap\overline{B})$$|$$P(\overline{B})$$|
||$$P(A)$$|$$P(\overline{A})$$|$$P(\Omega)$$|

oder Baumdiagramm (bedingte Wahrscheinlichkeiten)

## Zufallsgröße
= Zusammenfassung verschiedener Ereignisse zu einem Wert einer Zufallsgröße (meist $$X, Y, Z$$)  
→ bspw. Augensumme beim Würfeln

Darstellungsmöglichkeiten:
- Wahrscheinlichkeitsverteilung: $$x$$-$$P(X=x)$$-Tabelle
- Histogramm: Säulendiagramm zur Wahrscheinlichkeitsverteilung ($$x$$-$$P(X=x)$$-Diagramm; Wahrscheinlichkeiten mit Breite 1 LE)  
  → auch kumulativ (Aufaddierung der Wahrscheinlichkeiten von 0 bis zum Maximalwert 1 am Ende)

- **Erwartungswert** (gewichteter Mittelwert) einer Zufallsgröße: $$E(X)=\mu=\sum\limits_{i=0}^n{x_i\cdot P(X=x_i)}$$  
  → ein Spiel wird bei $$\mu=0$$ als „fair” bezeichnet
- **Varianz** (mittlere quadratische Abweichung vom Erwartungswert) einer Zufallsgröße: $$Var(X)=\sum\limits_{i=0}^n{P(X=x_i)\cdot (x_i-\mu)^2}$$  
  → Maß für die Streuung  
  → Einheit $$(Einheit)^2$$
- **Standardabweichung** einer Zufallsgröße: $$\sigma=\sqrt{Var(X)}$$  
  → keine quadratische Einheit  
  → Einzeichnung in das Histogramm möglich

## Ziehen ohne Zurücklegen
Wahrscheinlichkeiten verändern sich bei jedem Ziehen  
→ Berechnung mit $$\frac{\text{„Günstige”}}{\text{„Mögliche”}}$$ (dafür sind Laplace-Experimente notwendig!)
- Permutation
  - Anzahl der Möglichkeiten eines Zufallsexperiments unter Beachtung der Reihenfolge
    → Multiplikation der Möglichkeiten in den einzelnen Stufen
  - für $$n$$ Elemente gibt es $$n!$$ (Fakultät; mit $$0!=1$$) Möglichkeiten, sie anzuordnen
- Kombination
  - Anzahl der Möglichkeiten eines Zufallsexperiments ohne Beachtung der Reihenfolge
  - für „$$k$$ aus $$n$$” Elemente gibt es ohne Beachtung der Reihenfolge $$\binom{n}{k}$$ Möglichkeiten (Möglichkeiten mit Reihenfolge geteilt durch Möglichkeiten, diese anzuordnen)  
    → Binomialkoeffizient: $$\binom{n}{k}=\frac{n!}{(n-k)!\cdot k!}$$  
	($$\binom{n}{k}=\binom{n}{n-k}$$; $$\binom{n}{1}=\binom{n}{n-1}=n$$; $$\binom{n}{0}=\binom{n}{n}=1$$)
- hypergeometrische Verteilung
  - aus Urne mit $$N$$ Kugeln ($$S$$ schwarze, $$N-S$$ weiße) $$n$$ Kugeln ($$s$$ schwarze, $$n-s$$ weiße) ziehen
  - Wahrscheinlichkeit (für $$s$$ schwarze und $$n-s$$ weiße Kugeln): $$P(X=s)=\frac{\binom{S}{s}\cdot \binom{N-S}{n-s}}{\binom{N}{n}}$$
  
## Ziehen mit Zurücklegen
Wahrscheinlichkeiten über alle Züge hinweg konstant  
- n-mal Würfeln: stets dieselbe Wahrscheinlichkeit für jede Zahl, z.B. $$P(\text{„sieben mal die 1”})=(\frac{1}{6})^7$$
- Bernoulli-Experiment:
  - „Bernoulli-Kette” der *Länge* $$n$$ mit zwei möglichen Ergebnissen (Treffer und Niete) und der *Trefferwahrscheinlichkeit* $$p$$ (*Nietenwahrscheinlichkeit* $$q=1-p$$)  
  - $$X$$: Anzahl der Treffer
  - Wahrscheinlichkeit für $$k$$ Treffer: $$P_p^n(X=k)=B(n;p;k)=\binom{n}{k}\cdot p^k\cdot q^{n-k}$$
  - $$\mu=n\cdot p$$; $$Var(X)=n\cdot p\cdot q$$; $$\sigma=\sqrt{Var(X)}=\sqrt{n\cdot p\cdot q}$$
  - kumulative Wahrscheinlichkeiten ($$P_p^n(X\leq k)=\sum\limits_{i=0}^k{P_p^n(X=i)}$$) im Tafelwerk
  - Binomialverteilung: Histogramm einer Bernoulli-Kette ($$k$$-$$P_p^n(X=k)$$-Diagramm)  
    → Maximum um $$\mu$$ (bei $$\lfloor\mu \rfloor$$ bzw. $$\lceil\mu \rceil$$)
