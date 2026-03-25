Nullstellen bezeichnen Punkte einer Funktion bei denen der y-Wert an dem Punkt x null ist. Auch gelesen als $f(x)=0$.
Eine **Nullstelle** ist ein $x_0$ ​, für das gilt: $f(x_0) = 0$
Die Funktion schneidet (oder berührt) dort die x-Achse.

# Methoden zum Errechnen der Nullstellen
## 1. Ausklammern
$f(x)=x^3−4x=x(x^2−4)⟹x_{1}​=0,x_{2}=4$

## 2. Substitution
Bei $x^4-5x^2+4=0$ setze $u=x^2$:

$u^2-5u+4=0\implies u_{1,2}=\dots \implies x=\pm\sqrt{ u }$

## 3. Mitternachtsformel (Quadratische Gleichungen)
Am besten für $ax^2+bx+c=0$ geeignet:
$$x_{1,2}= \frac{-b \pm \sqrt{ b^2-4ac }}{2a}$$
## 4. pq-Formel
Benötigt $x^2+px+q=0$, d.h. $a=1$:
$$x_{1,2}=-\frac{p}{2} \pm \sqrt{ (\frac{p}{2})^2 -q}$$
## 5. Diskriminante
$D=b^2-4ac$:
- **D>0**: 2 reelle Nullstellen
- **D=0:** 1 doppelte Nullstelle
- **D<0:** keine reellen Nullstellen

## 6. Horner-Schema (Polynome höheren Grades)

Wenn $x_0$ ​ eine bekannte (oder geratene) Nullstelle ist, lässt sich das Polynom durch $(x−x_{0})$ teilen und so um einen Grad reduzieren.