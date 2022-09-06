### **Tarea 1**

**Modelos de distribución multivariados (variables discretas)**

Equipo: 
* Patricia Muñoz López
* Michel Carmía Corona Bermúdez 
* Gregorio Alberto Álvarez Álvarez

<br/><br/>1. Sea X e Y variables aleatorias bidimensionales discretas con función de masa probabilidad conjunta

| X\Y | 1   | 3   |
|-----|-----|-----|
| 0   | 0   | 1/8 |
| 1   | 3/8 | 0   |
| 2   | 3/8 | 0   |
| 3   | 0   | 1/8 |


**a)** Obtenga la función de distribución acumulada para los siguientes intervalos:

$$F(x, y) = P(X \leq x, Y \leq y) = \left\{
            \begin{array}{ll}
                0 \text{ } si \text{ } x < 0, \text{ y } y < 1 \\\\
                0 \text{ } si \text{ } 0 \leq x < 1, 1 \leq y < 3\\\\
                \frac{1}{8} \text{ } si \text{ } 0 \leq x < 1, y \geq 3\\\\
                \frac{4}{8} \text{ } si \text{ } 1 \leq x < 2, y \geq 1\\\\
                \frac{7}{8} \text{ } si \text{ } 2 \leq x < 3, y \geq 1\\\\
                \frac{6}{8} \text{ } si \text{ } x
                \geq 3, 1 \leq y < 3\\\\
                1 \text{ } si \text{ } x
                \geq 3, y \geq 3\\
            \end{array}
            \right.$$

<br/><br/>
**2.** A continuación, se muestra la distribución de masa de probabilidad conjunta de 𝑋, 
el  número  de  contratos  otorgados  a  la  empresa  𝐴  y  𝑌,  el  número  de  contratos 
otorgados a la empresa 𝐵

| X\Y | 0   | 1   | 2   |
|-----|-----|-----|-----|
| 0   | 1/9 | 2/9 | 1/9 |
| 1   | 2/9 | 2/9 | 0   |
| 2   | 1/9 | 0   | 0   |

<br/><br/>
**a)** Encuentre $𝑓_{𝑋𝑌}(0,1)$. ¿Cuál es la interpretación de este valor?

$f_{XY}(0,1) = \frac{2}{9}$

Es la probabilidad de que no le den contratos a la empresa A y que le den un contrato a la empresa B.

**b)** Proporcione las funciones de probabilidad marginal de 𝑋 y 𝑌.

$f_{X}(0) = \frac{4}{9} \approx0.44$

$f_{X}(1) = \frac{4}{9} \approx 0.44$

$f_X(2) = \frac{1}{9} \approx 0.11$

$f_Y(0) = \frac{4}{9} \approx0.44$

$f_Y(1) = \frac{4}{9} \approx 0.44$

$f_Y(2) = \frac{1}{9} \approx 0.11$

**c)** Proporcione la función de probabilidad condicional para 𝑌 dado que 𝑋 = 2.

$f_{Y|X}(Y = 0|X = 2) = \frac{f_{YX}(0, 2)}{f_X(2)} = \frac{1/9}{1/9} = 1$

$f_{Y|X}(Y = 1|X = 2) = \frac{f_{YX}(1, 2)}{f_X(2)} = \frac{0}{1/9} = 0$

$f_{Y|X}(Y = 2|X = 2) = \frac{f_{YX}(2, 2)}{f_X(2)} = \frac{0}{1/9} = 0$

**d)** Proporcione la función de probabilidad condicional para 𝑋 dado que 𝑌 = 1

$f_{X|Y}(X = 0|Y = 1) = \frac{f_{XY}(0, 1)}{f_Y(1)} = \frac{2/9}{4/9} = \frac{1}{2}$

$f_{X|Y}(X = 1|Y = 1) = \frac{f_{XY}(1, 1)}{f_Y(1)} = \frac{2/9}{4/9} = \frac{1}{2}$

$f_{X|Y}(X = 2|Y = 2) = \frac{f_{XY}(2, 1)}{f_Y(1)} = \frac{0}{4/9} = \frac{1}{2}$

**e)** ¿Cuál es la probabilidad de que se hayan otorgado dos contratos a la empresa B 
dado que se le otorgó un contrato a la empresa A?

$f_{Y|X}(Y = 2| X = 1) = \frac{f_{YX}(2, 1)}{f_X(1)} = \frac{0}{4/9} = 0$

**f)** ¿𝑋 y 𝑌 son independientes? ¿Por qué sí o por qué no?

Para comprobar independiencia utilizamos

$f_{XY}(x,y) = f_X(x)f_Y(Y)$ para toda $x$ e $y$ si se cumple para por lo menos un valor de x y y

Entonces,

$f_{XY}(0,0) = \frac{1}{9} \not = f_X(0)f_Y(0) = \frac{16}{81}$

Por la propiedad de que la probabilidad conjunta sea igual a producto de las probabilidades marginales, no es verdadero.

<br/><br/>
**3.**  A  continuación,  se  da  la  función  de  masa  de  probabilidad  conjunta  asociada  con 
datos obtenidos en un estudio de accidentes automovilísticos en los que un niño (de 
menos  de  5  años)  estaba  en  el  auto  y  hubo  al  menos  una  persona  muerta. 
Específicamente  el  estudio  se  concentró  en  si  el  niño  sobrevivió  y  qué  tipo  de 
cinturón de seguridad (si lo había) utilizaba. 

| X/Y | 0    | 1    | 2    |
|-----|------|------|------|
| 0   | 0.38 | 0.14 | 0.24 |
| 1   | 0.17 | 0.02 | 0.05 |

Defina


$X = \left\{
            \begin{array}{ll}
                0 \text{ si el niño sobrevivió}\\
                1 \text{ si no}\\
            \end{array}
            \right.$


$Y = \left\{
            \begin{array}{ll}
                0 \text{ si no usaba cinturón}\\
                1 \text{ si usaba cinturón para adulto}\\
                2 \text{ si usaba cinturón del asiento del auto}\\
            \end{array}
            \right.$

**a)** Encuentre 𝐹(1,1). ¿Cuál es la interpretación de este valor?

F(1,1) = 0.71. Representa la probabilidad acumulada de sobreviviencia a accidentes automovilísticos de menores de 5 años.

**b)** Proporcione las funciones de probabilidad marginal de 𝑋 y 𝑌.

$f_{X}(0) = 0.76$

$f_{X}(1) = 0.24$

$f_Y(0) = 0.55$

$f_Y(1) = 0.16$

$f_Y(2) = 0.29$

<br/><br/>
<br/><br/>
**c)** Proporcione la función de probabilidad condicional para 𝑌 dado que 𝑋 = 0.


$f_{Y|X}(Y = 0|X = 0) = \frac{f_{YX}(0, 0)}{f_X(0)} = \frac{0.38}{0.76} = 0.50$

$f_{Y|X}(Y = 1|X = 0) = \frac{f_{YX}(1, 0)}{f_X(0)} = \frac{0.14}{0.76} \approx 0.18$

$f_{Y|X}(Y = 2|X = 0) = \frac{f_{YX}(2, 0)}{f_X(0)} = \frac{0.24}{0.76} \approx 0.32$

**d)** Proporcione la función de probabilidad condicional para 𝑋 dado que 𝑌 = 2

$f_{X|Y}(X = 0|Y = 2) = \frac{f_{XY}(0, 2)}{f_Y(2)} = \frac{0.24}{0.29} \approx 0.83$

$f_{X|Y}(X = 1|Y = 2) = \frac{f_{XY}(1, 2)}{f_Y(2)} = \frac{0.05}{0.29} \approx 0.17$

**e)** ¿Cuál  es  la  probabilidad  de  que  un  niño  sobreviva  dado  que  llevaba  puesto  el 
cinturón del asiento del auto?

$f_{X|Y}(X = 0|Y = 2) = \frac{f_{XY}(0, 2)}{f_Y(2)} = \frac{0.24}{0.29} \approx 0.83$

**f)** ¿𝑋 y 𝑌 son independientes? ¿Por qué sí o por qué no?

$f_{XY}(x,y) = f_X(x)f_Y(Y)$ para toda $x$ e $y$ si se cumple para por lo menos un valor de x y y

Entonces,

$f_{XY}(0,0) = 0.38 \not = f_X(0)f_Y(0) = 0.76 \cdot 0.55 = 0.42$

Por la propiedad de que la probabilidad conjunta sea igual a producto de las probabilidades marginales, no es verdadero y por tanto, no son independientes.

<br/><br/>
**4. De  un  grupo  de  tres  republicanos,  dos  demócratas  y  uno  independiente  se  ha  de 
seleccionar  aleatoriamente  un  comité  de  dos  personas.  La  función  de  masa  de 
probabilidad conjunta asociada con el número de republicanos (𝑋) y el número de 
demócratas (𝑌) que conforman un comité se muestra a continuación

| Y/X | 0    | 1    | 2    |
|-----|------|------|------|
| 0   | 0    | 3/15 | 3/15 |
| 1   | 2/15 | 6/15 | 0    |
| 2   | 1/15 | 0    | 0    |

**a)** Encuentre  la  probabilidad  de  que  en  el  comité  haya  dos  republicanos  y  un 
demócrata.

$f_{XY}(2,1) = 0$

**b)** Encuentre la probabilidad de que en el comité haya un republicano.

$f_{X}(1) = \frac{9}{15} = \frac{3}{5}$

**c)** Encuentre la probabilidad de que en el comité haya dos demócratas.

$f_{Y}(2) = \frac{1}{15}$

**d)** Encuentre  la  probabilidad  de  que  en  el  comité  no  haya  demócratas  dado  que 
haya dos republicanos.

$f_{Y|X}(Y=0|X=2) = \frac{3/15}{3/15} = 1$

**e)** Encuentre  la  probabilidad  de  que  en  el  comité  haya  un  republicano  dado  que 
haya un demócrata.

$F_{X|Y}(X=1|Y=1) = \frac{6/15}{8/15} = \frac{3}{4} = 0.75$

**f)** ¿𝑋 y 𝑌 son independientes? ¿Por qué sí o por qué no?


$f_{XY}(x,y) = f_X(x)f_Y(Y)$ para toda $x$ e $y$ si se cumple para por lo menos un valor de x y y

Entonces,

$f_{XY}(1,1) = \frac{2}{5} = 0.4  \not = f_X(1)f_Y(0) = \frac{3}{5} \cdot \frac{8}{15} = \frac{8}{25} = 0.32$

Por la propiedad de que la probabilidad conjunta sea igual a producto de las probabilidades marginales, no es verdadero y por tanto, no son independientes.

<br/><br/>
**5.** A  continuación,  se  muestra  la  función  de  masa  de  probabilidad  conjunta  sobre  la 
población  de  departamentos  en  renta  de  Hong  Kong  donde  𝑋  representa  la  renta 
mensual de los departamentos e 𝑌 representa el tipo de departamento.


| Renta\Tipo            | Público | Privado | Otros |
|-----------------------|---------|---------|-------|
| Baja ( ≤ 1𝑘)          | 0.17    | 0.01    | 0.02  |
| Media (1𝑘,5𝑘])        | 0.35    | 0.03    | 0.01  |
| Media alta ((5𝑘,12𝑘]) | 0.09    | 0.07    | 0.01  |
| Alta ( > 12𝑘)         | 0       | 0.14    | 0.10  |


Calcule las siguientes probabilidades y de una interpretación de los resultados.
**a)** P (X=Media, Y=Privado) 

$P(X=Media, Y=Privado)  = 0.03$

**b)** P(X=Baja, Y=Público) 

$P(X=Baja, Y=Público) = 0.17$

**c)** P (Y=Otros)

$P (Y=Otros) = 0.14$

**d)** P (X=Alta)

$P(X=Alta) = 0.24$

**e)** P (X=Alta | Y=Privado)

$P(X=Alta | Y=Privado) = \frac{0.14}{0.25} = 0.56$

**f)** P (Y=Otros | X=Media alta)

$P(Y=Otros | X=Media alta) = \frac{0.01}{0.17} \approx 0.06$

**g)** ¿El precio de la renta es independiente del tipo de departamento?

$f_{XY}(x,y) = f_X(x)f_Y(Y)$ para toda $x$ e $y$ si se cumple para por lo menos un valor de x y y

Entonces,

$f_{X,Y}(Baja, Publico) = 0.17 \not = f_X(1)f_Y(0) = 0.2 \cdot 0.61 \approx 0.12$

Por la propiedad de que la probabilidad conjunta sea igual a producto de las probabilidades marginales, no es verdadero y por tanto, no son independientes.

<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({ tex2jax: {inlineMath: [['$', '$']]}, messageStyle: "none" });
</script>