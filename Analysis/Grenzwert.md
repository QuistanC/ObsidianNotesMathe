Der Grenzwert betrachtet das Verhalten der y-Werte einer Funktion, wenn der x-Wert gegen einen spezifischen Wert läuft. Wenn die Funktionen gegen einen festen Wert strebt und nicht weiter wächst, spricht man entweder von einer Konvergenz oder einer Divergenz. Wenn sie unendlich wächst, spricht man von einer **Divergenz.** Wenn die Funktion gegen einen festen Wert strebt, spricht man von einer **Konvergenz.**

## Notation:

$$\lim_{ n \to \infty } f(x) = L$$

## Formale Definition
Intuitiv: Egal wie eng ich das Zielband um L wähle (Epsilon), ich kann immer ein Eingabeband um a finden (Delta), das garantiert, dass f(x) im Zielband bleibt.
$$\lim f(x)=L: \leftrightarrow \forall \varepsilon>0 \exists \delta>0:0<|x-a|<\delta \implies|f(x)-L|<\varepsilon$$
![[Pasted image 20260325192454.png]]

**Beweisstrategie (Beispiel):**
Sei $\lim_{x \to_{2}}(2x+1)=5$
1. **Was zu zeigen ist:** $\forall \varepsilon>0\exists\delta>0:0<|x-2|<\delta \implies|(2x+1)-5|<\varepsilon$
2. **Ausdruck vereinfachen:** $|(2x+1)-5|=|2x-4|=2*|x-2|$
3. **$\delta$ wählen:** $2*|x-2|< \varepsilon \leftrightarrow|x-2|<\frac{\varepsilon}{2}\implies \delta=\frac{\varepsilon}{2}$
4. **Nachprüfen:** Sei $\varepsilon>0, \delta=\frac{\varepsilon}{2}$. Dann: $|x-2|<\delta \implies|(2x+1)-5|=2|x-2|<2\delta=\varepsilon$

## Unbestimmte Ausdrücke
Unbestimmte Ausdrücke sind nicht direkt auswertbar und erfordern weitere Umformungen oder die Verwendung der [[Regel von L'Hôpital]]:
- $\frac{0}{0}$
- $\frac{\infty}{\infty}$
- $0*\infty$
- $\infty-\infty$
- $0^0,\infty^0$
- $1^\infty$
## Rechenregeln (sofern Limes existiert)
- **Summenregel:** $\lim_{ n \to \infty } (f+g) = \lim_{ n \to \infty }f + \lim_{ n \to \infty } g$
- **Differenzregel:** $\lim_{ n \to \infty } (f-g)=\lim_{ n \to \infty } f - \lim_{ n \to \infty } g$
- **Produktregel:** $\lim_{ n \to \infty } (f*g)=\lim_{ n \to \infty } f * \lim_{ n \to \infty } g$
- **Quotientenregel:** $\lim_{ n \to \infty } \frac{f}{g} = \frac{\lim_{ n \to \infty }f}{\lim_{ n \to \infty }g}$
- **Potenzregel:** $\lim_{ n \to \infty } (f(x))^n = (\lim_{ n \to \infty })^n$
- **Stetige Funktionen:** $\lim_{ n \to \infty }f(g(x))=f(\lim_{ n \to \infty }g(x))$

## Regel von L'Hôpital
**Die Grundidee:** Wenn Zähler und Nenner beide gegen 0 oder beide gegen ∞ gehen, sagt uns die Ratio der Ableitungen, _wie schnell_ jede Seite dorthin läuft – und genau das bestimmt den Grenzwert.

**Voraussetzung:** $\lim \frac{f(x)}{g(x)} = \frac{0}{0} \lor \frac{\infty}{\infty} \land g'(x) \ne 0$

$$\lim \frac{f(x)}{g(x)} = \lim \frac{f'(x)}{g'(x)} $$
Zähler und Nenner werden dabei getrennt voneinander abgeleitet: Es wird **keine** Quotientenregel verwendet!
Man darf die Regel erneut auf die jeweiligen Terme anwenden, falls das Ergebnis wieder unbestimmt ist.

**Wann L'Hôpital nicht hilft**
- Zyklische Ableitungen (sin/cos)
- Auch wenn $\lim\frac{f'}{g'}$ nicht existiert, sagt das nichts über die Existenz $\lim \frac{f}{g}$ aus