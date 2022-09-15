# Modelos de distribucion multivariables continuos

1. Sean 𝑋 e 𝑌 variables aleatorias continuas con función de densidad de probabilidad 
conjunta


$$ f_{XY}(x, y) =\begin{cases}
               \frac{1}{2}x + \frac{3}{2}y & 0 \leq x \leq 1, 0\leq y \leq 1\\\\
               0 & otros
            \end{cases}$$

Determine
a) La función de distribución acumulada.

$$ F_{XY}(x,y) = \int _0^x\int _0^y\frac{1}{2}x+\frac{3}{2}y_dydx $$

$$ F_{XY}(x,y) = \int _0^x\frac{1}{2}xy+\frac{3}{4}y^2_dx $$

$$ =  \boxed {\frac{1}{4}x^2y + \frac{3}{4}xy^2}$$

b) Las funciones de densidad de probabilidad marginal para 𝑋 e 𝑌.

$f_X(x) = \int_{0}^{1}\left( \frac{1}{2}x + \frac{3}{2} v\right) dv = \frac{1}{2}xv + \frac{3}{4} v^2 \Big|^{1}_0 = \boxed{\frac{1}{2}x + \frac{3}{4}}$

$f_Y(y) = \int_{0}^{1}\left( \frac{1}{2}u + \frac{3}{2} y\right) du = \frac{1}{4}u^2 + \frac{3}{2}yu \Big|^1_0 = \boxed{\frac{1}{4} + \frac{3}{2}y}$

c) Las funciones de densidad de probabilidad condicional de 𝑋 e 𝑌.

$$f_{X|Y}(x|y) = \boxed{\frac{\frac{1}{2}x + \frac{3}{2}y}{\frac{1}{4} + \frac{3}{2}y}}$$

$$f_{Y|X}(y|x) = \boxed{\frac{\frac{1}{2}x + \frac{3}{2}y}{\frac{1}{2}x + \frac{3}{4}}}$$

d) Si las variables aleatorias son independientes.

Si $f_{XY}(x,y) = f_X(x)f_Y(y)$ para toda x, y; entonces $X$ y $Y$ son independientes

$f_{X}(x) = \frac{1}{2}x + \frac{3}{4}$

$f_{Y}(y) = \frac{3}{2}y + \frac{1}{4}$

$fx_{x} fy_{y} = \left(\frac{1}{2}x+\frac{3}{4}\right)\left(\frac{3}{2}y+\frac{1}{4}\right)$

$fxy_{x,y} = \frac{1}{2}x + \frac{5}{2}y $

$$ {fxy_{x,y} \neq fx_{x} fy_{y}}$$

No son independientes

****

2. Un sistema electrónico tiene uno de cada dos tipos diferentes de componentes de 
operación en operación conjunta. Denote con 𝑋 y 𝑌 las duraciones aleatorias de los 
componentes  del  tipo  I  y  tipo  II  respectivamente.  La  función  de  densidad  de 
probabilidad conjunta está dada por

$$f_{X Y}(x, y) = \begin{cases}
\frac{1}{8} x e^{-(x+y) / 2} & x>0, y>0 \\\\
0 & \text { otros. }
\end{cases}$$

Las mediciones son en cientos de horas.

a) Encuentre $𝑃(𝑋> 1,𝑌> 1)$

$$𝑃(𝑋> 1,𝑌> 1) = \int^{\infty}_{1} \int^{\infty}_{1} \frac{1}{8}xe^{-(x + y)/2} dydx$$

$$= \frac{1}{8} \int^{\infty}_{1} xe^{x/2} \left[ -0 + 2e^{-1/2} \right]dx = -\frac{1}{4} e^{-1/2}  \int^{\infty}_{1} x e^{-x/2} dx$$

$$= \frac{1}{4} e^{-1/2} e^{-1/2}\left[ -2x -4 \right] \Big|^{\infty}_1 = -\frac{1}{4} e^{-1/2} e^{-1/2}\left[ -2 -4 \right]$$

$$\boxed{= \frac{3}{2e} \approxeq .5518}$$

b) Encuentre  la  probabilidad  de  que  el  componente  tipo  II  tenga  una  vida  útil  de 
más de 200 horas.

$P(Y > 2) = \int^{\infty}_2 \int^{\infty}_0 \frac{1}{8} x e^{-(x+y) / 2} dxdy = \frac{1}{8}  \int^{\infty}_2 e^{-y/2} \int^{\infty}_0 xe^{-x/2} dxdy$

$= \frac{1}{8}  \int^{\infty}_2 e^{-y/2} e^{-x/2} [2x - 4] dy \Big|^{\infty}_0$

$= \frac{1}{2} \int^{\infty}_2 e^{-y/2} dy = \frac{1}{2} \left[ -2e^{-y/2} \right] \Big|^{\infty}_2$

$$= \boxed{\frac{1}{e} \approxeq 0.3679}$$

****

3. Sea X e Y variables aleatorias continuas con función de densidad de probabilidad conjunta

$$f_{XY} = \begin{cases}
\frac{1}{4}(1 + xy(x^2 - y^2)), & -1 \leq x \leq 1, \quad -1 \leq y \leq 1 \\\\
0 & otros   
\end{cases}
$$

Determine

a) La función de distribución acumulada.

$$F_{XY}(x, y) = \int^{x}_0 \int^{y}_0 \frac{1}{4}(1 + xy(x^2 - y^2)) dy dx = \frac{1}{4}\int^{x}_0 \int^{y}_0 (1 + x^3y - xy^3) dy dx$$

$$= \frac{1}{4} \int^{x}_0 (y + \frac{1}{2}x^3y^2 - \frac{1}{4}xy^4) dx = \frac{1}{4} (xy + \frac{1}{8}x^4y^2 - \frac{1}{8}x^2y^4) = \boxed{\frac{1}{4} \left(xy + \frac{1}{8}x^2y^2(x^2 - y^2)\right)}$$

b) Las funciones de densidad de probabilidad marginal para 𝑋 e 𝑌.

$$f_X(x) = \int^{y}_0 \frac{1}{4}(1 + xy(x^2 - y^2)) dy = \boxed{\frac{1}{4} \left(y + \frac{1}{2}x^3y^2 - \frac{1}{4}xy^4\right)}$$

$$f_Y(y) = \int^{x}_0 \frac{1}{4}(1 + xy(x^2 - y^2)) dx = \boxed{\frac{1}{4}\left( x + \frac{1}{4}x^4y - \frac{1}{2}x^2y^3 \right)}$$

c) Las funciones de densidad de probabilidad condicional de 𝑋 e 𝑌.

$$f_{X|Y}(X \leq x|Y \leq y) = \boxed{\frac{(1 + xy(x^2 - y^2))}{\left( x + \frac{1}{4}x^4y - \frac{1}{2}x^2y^3 \right)}}$$

$$f_{Y|X}(Y \leq y|X \leq x) = \boxed{\frac{(1 + xy(x^2 - y^2))}{ \left(y + \frac{1}{2}x^3y^2 - \frac{1}{4}xy^4\right)}}$$

d) Si las variables aleatorias son independientes.

Si $f_{XY}(x,y) = f_X(x)f_Y(y)$ para toda x, y; entonces $X$ y $Y$ son independientes

$f_{XY}(x,y) = \frac{1}{4}(1 + xy(x^2 - y^2))$

$f_X(x)f_Y(y) = \frac{1}{4} \left(y + \frac{1}{2}x^3y^2 - \frac{1}{4}xy^4\right) \cdot \frac{1}{4}\left( x + \frac{1}{4}x^4y - \frac{1}{2}x^2y^3 \right)$
****
4. 	La administración en un restaurante de comida rápida está interesada en el comportamiento conjunto de las variables aleatorias X y Y.  X, representa el tiempo total entre la llegada de un cliente a la tienda y la salida de la ventanilla de servicio,  Y, el tiempo que un cliente espera en la fila antes de llegar a la ventanilla de servicio. Como X incluye el tiempo que un cliente espera en la fila, debemos tener X≥Y. La distribución de valores observados puede ser modelada por la siguiente función de densidad de probabilidad conjunta

$$f_{XY} = \begin{cases}
e^{-x}, & 0 \leq y \leq x < \infty \\\\
0 & otros   
\end{cases}
$$

con el tiempo medido en minutos. Encuentre

a)P(X<2,Y>1).

$$ 0 \leq y \leq x ,
 y \leq x < \infty
$$

$$ \int_{1}^{2}\int_{1}^{x} e^{-x} dydx $$

$$ \int _1^xe^{-x}dy$$

$$ =\left[e^{-x}y\right]^x_1 $$

$$ =e^{-x}x-e^{-x} $$


$$ \int _1^2\left(e^{-x}x-e^{-x}\right)dx $$

$$ =\int _1^2e^{-x}xdx-\int _1^2e^{-x}dx $$

$$ = -\frac{3}{e^2}+\frac{2}{e}-\left(\frac{1}{e}-\frac{1}{e^2}\right) $$

$$ = \frac{e-2}{e^2} $$

b) 	Las funciones de densidad marginal para X y Y.

$$ fx (x) = \int_{y}^{\infty} e^{-x} dy = e^{-y} $$

$$ fy (y) = \int_{0}^{x} e^{-x} dx =  -e^{-x}+1 $$

c) ¿Cuál es la función de densidad condicional de X dado que Y=y?

$$ \frac{e^{-x}}{-e^{-x}+1}$$

d) ¿Cuál es la función de densidad condicional de Y dado que X=x?
e) ¿La función de densidad condicional que obtuvo en el inciso c es la misma que la función de densidad marginal hallada en el inciso b?
f) ¿Qué implica su respuesta del inciso e?
****

5. 	Considere la función de densidad de probabilidad conjunta de X, la proporción de la capacidad de un tanque que ha sido abastecido al principio de la semana y Y, la proporción de la capacidad vendida durante la semana.

$$f_{XY} = \begin{cases}
3x, & 0 \leq y \leq x \leq 1  \\\\
0 & otros   
\end{cases}
$$

a) 	Encuentre P(X≤1/2,Y≤1/3)

P(X≤1/2,Y≤1/3) = $$ \int_{0}^{1/3}\int_{y}^{1/2} 3x dydx $$

$$ = \int_{0}^{1/3} 3/8 - 3/2 y^2 dy $$

$$ \frac{3}{8} y - \frac{3}{6} y^3 \Big|_0^\frac{1}{3} = \frac{3}{8} (\frac{1}{3}) - \frac{3}{6}(\frac{1}{3})^3 $$

$$ = \boxed{\frac{23}{216}\approxeq 0.1065} $$

b)	Encuentre P(Y≤1/2 X), la probabilidad de que la cantidad vendida sea menor que la mitad de la cantidad comprada.

$$ \int_{0}^{1}\int_{0}^{\frac{1}{2}x} 3x dydx $$

$$ = \int_{0}^{\frac{1}{3}}3x(\frac{1}{2}x)dx = \frac{1}{2}x \Big|_0^1 $$

$$ \boxed {P(Y≤1/2 X) = \frac{1}{2}} $$

c) 	¿Serán X y Y independientes?

$$ {fxy_{x,y} \neq fx_{x} fy_{y}}$$

No son independientes
****

6. 	Sean X e Y variables aleatorias continuas con función de densidad de probabilidad conjunta

$$ f_{XY}(x, y) =\begin{cases}
               4xy & 0 \leq x \leq 1, 0\leq y \leq 1\\\\
               0 & otros
            \end{cases}$$
            
Determine

a) 	Las funciones de densidad de probabilidad marginal para X e Y.

$$ fx (x) = \int_{0}^{1} 4xy dy = 2x $$

$$ fy (y) = \int_{0}^{1} 4xy dx = 2y $$

b) 	P(X≤1/2|Y≥3/4)

$$ 0 \leq x \leq 1/2,
 3/4 \leq y \leq 1
$$

$$ \frac{\int_{0}^{1/2}\int_{3/4}^{1} 4xy dydx}{\int_{3/4}^{1} 2ydy} $$

$$ \frac{0.109375}{0.4375} = 0.25$$

c)  Las funciones de densidad de probabilidad condicional de X e Y.

$$ f_{X|Y} = \frac{4xy}{2y} = 2x $$

$$ f_{Y|X} = \frac{4xy}{2x} = 2y $$

d) 	P(X≤3/4|Y=1/2)

$$ \int _0^{\frac{3}{4}}2xdx $$ 

$$ =2\left[\frac{x^2}{2}\right]^{\frac{3}{4}}_0 $$

$$ =2\cdot \frac{9}{32}  = \frac{9}{16} = \:0.5625$$


<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({ tex2jax: {inlineMath: [['$', '$']]}, messageStyle: "none" });
</script>

