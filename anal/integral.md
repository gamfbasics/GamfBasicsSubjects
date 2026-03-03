# Integrálás

> Az elemi függvények deriváltjait a [deriválás](/anal/derival) oldalon láthatod

## Elemi függvények integráltjai
| $$f(x)$$                    | $$\int f(x) \, dx$$ |
| --------------------------- | ------------------- |
| $$a$$                       | $$ax+C, \quad ha \,a \in \R$$ |
| $$x^n$$                     | $$\frac{x^{n+1}}{n+1}+C, \quad ha \,a \neq -1$$ |
| $$\frac{1}{x}$$             | $$\ln\| x\|+C$$ |
| $$e^x$$                     | $$e^x+C$$ |
| $$a^x$$                     | $$\frac{a^x}{\ln a}+C$$ |
| $$\sin x$$                  | $$-\cos x+C$$ |
| $$\cos x$$                  | $$\sin x+C$$ |
| $$\frac{1}{\cos^2x}$$       | $$\tg x+C$$ |
| $$\frac{1}{\sin^2x}$$       | $$-\ctg x+C$$ |
| $$\frac{1}{\sqrt{1-x^2}}$$  | $$\arcsin x+C$$ |
| $$-\frac{1}{\sqrt{1-x^2}}$$ | $$\arccos x+C$$ |
| $$\frac{1}{1+x^2}$$         | $$\arctg x+C$$ |
| $$-\frac{1}{1+x^2}$$        | $$\arcctg x+C$$ |

## Primitív függvények
- **Definíció**: Az F függvényt *f* egy primitív függvényének nevezzük az I intervallumon, ha F'(x) = *f* (x) minden x ∈ I esetén
- **Példa**: *f* (x) = 2x
  - $$F (x) = x^2 + C$$
  - Mert $$x^2$$ deriváltja $$2*x^{2-1} = 2x$$

$$\int \Big( f(x) \pm g(x) \Big) = \int f(x) \pm \int g(x)$$

$$\int x^4 \,dx = \frac{x^5}{5}+C$$