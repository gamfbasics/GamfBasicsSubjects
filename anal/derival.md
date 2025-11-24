# Deriválás

- A derivált a függvény meredekségét adja meg egy adott pontban

**Elemi függvények deriváltjai**
|$$f$$                 |$$f'$$                       |
|:--------------------:|:---------------------------:|
|$$f(x) = c$$          |$$f'(x) = 0$$                |
|$$f(x) = x^n$$        |$$f'(x) = n*x^{n-1}$$        |
|$$f(x) = a^x$$        |$$f'(x) = a^x\ln a$$         |
|$$f(x) = e^x$$        |$$f'(x) = e^x$$              |
|$$f(x) = \log_{a}{x}$$|$$f'(x) = \frac{1}{x*\ln a}$$|
|$$f(x) = \ln x$$      |$$f'(x) = \frac{1}{x}$$      |
|$$f(x) = \sin x$$     |$$f'(x) = \cos x$$           |
|$$f(x) = \cos x$$     |$$f'(x) = -\sin x$$          |
|$$f(x) = \tg x$$      |$$f'(x) = \frac{1}{cos^2x}$$ |
|$$f(x) = \ctg x$$     |$$f'(x) = -\frac{1}{sin^2x}$$|

**Deriválási szabályok**
- Ha az f és a g függvény differenciálható az $$x_0$$ pontban és $$c \in \mathbb{R}$$, akkor az alábbi függvényeknek is létezik az adott pontban a deriváltjuk:
  - $$(cf)'(x_0) = cf'(x_0)$$
  - $$(f \pm g)'(x_0) = f'(x_0) \pm g'(x_0)$$
  - $$(f * g)'(x_0) = f'(x_0)g(x_0) + f(x_0)g'(x_0)$$
  - $$\left( \frac{f}{g} \right)'(x_0) = \frac{f'(x_0)g(x_0) - f(x_0)g'(x_0)}{g^2(x_0)}$$
- Ha a függvény differenciálható az $$x_0$$ pontban és az $$f$$ függvény differenciálható a $$g(x_0)$$ pontban, akkor az $$f \circ g$$ függvény is differenciálható az $$x_0$$ pontban:
  - $$(f(g(x_0)))' = f'(g(x_0))g'(x_0)$$

$$\cot{3}$$
