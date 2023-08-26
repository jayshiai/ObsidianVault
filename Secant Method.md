---
aliases: Chord Method
---

Similar to [[Regula Falsi Method]] except for the condition $f(x_1)f(x_2) < 0$

`Slope of AB` = `Slope of AC`

$$
\dfrac{f(x_1) - f(x_0)}{x_1-x_0} = \dfrac{0-f(x_0)}{x - x_0}
$$

$$\therefore x = \dfrac{x_0f(x_1) - x_1f(x_0)}{f(x_1) - f(x_0)}$$
General formula : 

$$
x_{n+1} = \dfrac{x_{n-1}f(x_n) - x_n f(x_{n-1})}{f(x_n) - f(x_{n-1})}
$$
this method_ fails if 
$f(x_n) = f(x_{n-1})$


tldr; screw Secant Metod, just do [[Regula Falsi Method]]
