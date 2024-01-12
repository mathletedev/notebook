---
tags:
  - math_172
---

> If position is given as a function $s(t)$, then we know that the velocity is $s'(t) = v(t)$, so the overall distance travelled from time $t = a$ to time $t = b$ is:
> $$ \int_a^b v(t) \, dt = s(b) - s(a). $$

- Note: the last step is the **Fundamental Theorem of Calculus**

## Lab notes

> $\displaystyle \int_0^3 4x^3 \, dx$

$= x^4 \Big|_0^3$
$= (3)^4 - (0)^4$
$= 81$

---

> $\displaystyle \int_{-1}^2 3x \, dx$

$= \dfrac{3}{2}x^2 \Big|_{-1}^2$
$= \dfrac{3}{2}(2)^2 - \dfrac{3}{2}(-1)^2$
$= \dfrac{9}{2}$

---

> $\displaystyle \int (8x - 12)(4x^2 - 12x)^4 \, dx$

Let $u = 4x^2 - 12x$
$\dfrac{du}{dx} = 8x - 12$
$dx = \dfrac{du}{8x - 12}$

$= \displaystyle \int u^4 \, du$
$= \dfrac{u^5}{5} + C$
$= \dfrac{(4x^2 - 12x)^5}{5} + C$