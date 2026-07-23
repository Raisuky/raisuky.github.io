### Problema 1
![[Pasted image 20260720220302.png]]
si tenemos 
$$
\hat{p}{^2} = -\frac{\hbar{^2}}{2m}\frac{d{^2}}{dx{^2}}
$$
entonces
$$
 -\frac{\hbar{^2}}{2m}\frac{d{^2}}{dx{^2}}\psi(x) + \psi(x)(\frac{1}{2} m \omega{^2}  x- E) =0
$$
Analizamos el comportamiento asintótico de la función de onda en los extremos; 

### Problema 2
![[Pasted image 20260721161757.png]]

Para determinar $A$ hay que usar $\int |\Psi|{^2}dx =1$
$$
A^2 \int_{-\infty}^\infty \left( 1-2 \sqrt{\frac{mw}{\hbar} } x\right)^4 e^{-\frac{m\omega}{\hbar}x^2} =1
$$
Definimos $u=\sqrt{ \frac{m\omega}{\hbar} }x$ tal que $dx=\sqrt{\frac{\hbar}{m \omega} }du$
$$
A^2 \sqrt{\frac{\hbar}{m \omega} } \int (1-2u)^4 e^{-u^2} du = 1
$$
$$
A^2 \int_{-\infty}^{\infty} (1-4u+4u^2)^2 e^{-u^2}du = \sqrt{\frac{m\omega}{\hbar}}
$$
$$
A^2 \int_{-\infty}^\infty (1-8u+24u^2-32u^3+16u^4) e^{-u^2}du = \sqrt{ \frac{m\omega}{\hbar} }
$$
$$
A^2 \int_{-\infty}^\infty (1+24u^2+16u^2)e^{-u^2} = \sqrt{ \frac{m\omega}{\hbar} }
$$
$$
A^2 (25\sqrt{ \pi }) = \sqrt{ \frac{m\omega}{\hbar} }
$$
$$
A = \frac{1}{5} \left(\frac{m\omega}{\pi \hbar}\right)^{1/4}
$$
Volviendo a la función de onda:
$$
\Psi(x,0) =  \frac{1}{5} \left(\frac{m\omega}{\pi \hbar}\right)^{1/4} \left( 1-2 \sqrt{ \frac{m\omega}{\hbar} } x \right)^2 e^{-\frac{m\omega}{2\hbar} x^2}
$$
 Usando $u=\sqrt{ \frac{m\omega}{\hbar}}x$. Expandiendo el binomio $(1-2u)^2=1-4u+4u^2$  y usamos los polinomios de Hermite 
$$
H_{0}(u)=1, 2H_{1}(u)=4u, H_{2}(u)=4u^2-2
$$
Despejamos $4u^2$ tal que: $4u^2=H_{2}(u)-2$ y reemplazamos en la ec. de onda tal que
$$
\Psi(x,0) =  \frac{1}{5} \left(\frac{m\omega}{\pi \hbar}\right)^{1/4} (H_{0}(u)-2H_{1}(u)+H_{2}(u)+2) e^{-\frac{m\omega}{2\hbar} x^2}
$$
Como $H_{0} = 1$ entonces podemos sumarlo con el  $2$ y tomar que $3 = 3H_{0}$
$$
\Psi(x,0) =  \frac{1}{5} \left(\frac{m\omega}{\pi \hbar}\right)^{1/4} (3H_{0}(u)-2H_{1}(u)+H_{2}(u)) e^{-\frac{m\omega}{2\hbar} x^2}
$$
Para que esto se asemeje al oscilador armónico usamos varios unos convenientes con $\sqrt{\frac{2^nn!}{2^nn!} }$ donde usamos $n=0,1,2$ por los polinomios de Hermite y definimos $N=(\frac{m\omega}{\pi\hbar})^{1/4}$, donde $N$ es la constante de normalización en el oscilador armónico cuántico típico. Desarrollando:

$$
\Psi(x,0) = \frac{1}{5}N \left( \frac{3}{1}H_{0}-\frac{2\sqrt{ 2 }}{\sqrt{ 2 }}H_{1}+  \frac{\sqrt{8}}{\sqrt{8} }H_{2} \right) e^{-\frac{m\omega}{2\hbar }x^2}
$$
$$
\Psi(x,0) = \frac{1}{5} \left( 3 (NH_{0}e^{-\frac{m\omega}{2\hbar }x^2})
-2\sqrt{ 2 }\left(N \frac{H_{1}}{\sqrt{ 2 }}e^{-\frac{m\omega}{2\hbar }x^2}\right) 
+ \sqrt{ 8 } \left( N\frac{H_{2}}{\sqrt{ 8 }}e^{-\frac{m\omega}{2\hbar }x^2}\right) \right) 
$$
con esto podemos escribir la función de onda en base del QHO quantum harmonic oscilator
$$
\Psi(x,0)  = \frac{1}{5} (3 \psi_{0}- 2\sqrt{ 2 }\psi_{1} + \sqrt{ 8} \psi_{3} )
$$
### Problema 3
![[Pasted image 20260722224318.png]]
Determinando la esperanza de $\hat{p}$
$$
\langle \hat{p} \rangle = \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \int_{-\infty}^\infty xe^{-m\omega x^2/2\hbar} (-i\hbar D_{x}(xe^{-m\omega x^2/2\hbar})) dx
$$
$$
D_{x}(xe^{-m\omega x^2/2\hbar}) = e^{-m\omega x^2/2\hbar}(1 - 2x^2 \frac{m\omega}{2\hbar} )
$$
$$
\langle\hat{p}\rangle = \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \int_{-\infty}^\infty xe^{-m\omega x^2/\hbar} (1 - 2x^2 \frac{m\omega}{2\hbar} ) dx
$$
$$
\langle\hat{p}\rangle = 0  \leftarrow \text{por paridad de la función en la integral.}
$$
Determinando la esperanza de $\hat{p}^2$
$$
\langle \hat{p}^2 \rangle = \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2}

\int_{-\infty}^\infty xe^{-m\omega x^2/2\hbar} (-\hbar^2 D_{x}^2(xe^{-m\omega x^2/2\hbar})) dx
$$
del cálculo anterior
$$
D_{x}(xe^{-m\omega x^2/2\hbar}) = e^{-m\omega x^2/2\hbar}(1 - 2x^2 \frac{m\omega}{2\hbar} )
$$
$$
D_{x}^2 (xe^{-m\omega x^2/2\hbar})= 
e^{-m\omega x^2/2\hbar} \left( -2x\frac{m\omega}{\hbar} 
- 4x \frac{m\omega}{2\hbar} 
+ 4x^3 \left( \frac{m\omega}{2\hbar} \right)^2 \right) = e^{-m\omega x^2/2\hbar} \left( 4x^3 (\frac{m\omega}{2\hbar})^2 -6x \frac{m\omega}{2\hbar} \right)
$$
$$
\begin{aligned}
\langle \hat{p}^2 \rangle &= -\hbar^2 \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \int_{-\infty}^\infty \left[ 4x^4 \left( \frac{m\omega}{2\hbar} \right)^2 e^{-\frac{m\omega}{\hbar} x^2} - 6x^2 \left( \frac{m\omega}{2\hbar} \right) e^{-\frac{m\omega}{\hbar} x^2} \right] dx \\[10pt]
&= -\hbar^2 \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \left[ 4\left( \frac{m^2\omega^2}{4\hbar^2} \right) \int_{-\infty}^\infty x^4 e^{-\frac{m\omega}{\hbar} x^2} dx - 6\left( \frac{m\omega}{2\hbar} \right) \int_{-\infty}^\infty x^2 e^{-\frac{m\omega}{\hbar} x^2} dx \right] \\[10pt]
&= -\hbar^2 \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \left[ \left( \frac{m^2\omega^2}{\hbar^2} \right) \left( \frac{3\sqrt{\pi}}{4} \left(\frac{\hbar}{m\omega}\right)^{5/2} \right) - \left( \frac{3m\omega}{\hbar} \right) \left( \frac{\sqrt{\pi}}{2} \left(\frac{\hbar}{m\omega}\right)^{3/2} \right) \right] \\[10pt]
&= -\hbar^2 \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \left[ \frac{3\sqrt{\pi}}{4} \left(\frac{\hbar}{m\omega}\right)^{1/2} - \frac{3\sqrt{\pi}}{2} \left(\frac{\hbar}{m\omega}\right)^{1/2} \right] \\[10pt]
&= -\hbar^2 \left( \frac{2 m^{3/2} \omega^{3/2}}{\sqrt{\pi} \hbar^{3/2}} \right) \left[ -\frac{3\sqrt{\pi}}{4} \left(\frac{\hbar}{m\omega}\right)^{1/2} \right] \\[10pt]
&= \hbar^2 \left( \frac{2 m^{3/2} \omega^{3/2}}{\sqrt{\pi} \hbar^{3/2}} \right) \left( \frac{3\sqrt{\pi}}{4} \frac{\hbar^{1/2}}{m^{1/2}\omega^{1/2}} \right) \\[10pt]
&= \frac{6}{4} \hbar^2 \left( \frac{m^{3/2} \omega^{3/2}}{\hbar^{3/2}} \right) \left( \frac{\hbar^{1/2}}{m^{1/2}\omega^{1/2}} \right) \\[10pt]
&= \frac{3}{2} m \hbar \omega
\end{aligned}
$$
Ahora la esperanza de $\hat{x}$ que es directamente cero por paridad, entonces
$$
\langle\hat{x}\rangle = 0
$$
calculando la esperanza de $\hat{x}^{2}$
$$
\begin{aligned}
\langle\hat{x}^2\rangle &= \left( \frac{4m^3\omega^3}{\pi \hbar^3} \right)^{1/2} \int_{-\infty}^{\infty} x^4 e^{-\frac{m\omega}{\hbar} x^2} dx \\[10pt]
&= \left( \frac{2 m^{3/2} \omega^{3/2}}{\sqrt{\pi} \hbar^{3/2}} \right) \left( \frac{3\sqrt{\pi}}{4} \left(\frac{\hbar}{m\omega}\right)^{5/2} \right) \\[10pt]
&= \left( \frac{2 m^{3/2} \omega^{3/2}}{\sqrt{\pi} \hbar^{3/2}} \right) \left( \frac{3\sqrt{\pi} \hbar^{5/2}}{4 m^{5/2} \omega^{5/2}} \right) \\[10pt]
&= \frac{6}{4} \left( \frac{\hbar^{5/2}}{\hbar^{3/2}} \right) \left( \frac{m^{3/2}}{m^{5/2}} \right) \left( \frac{\omega^{3/2}}{\omega^{5/2}} \right) \\[10pt]
&= \frac{3}{2} \frac{\hbar}{m\omega}
\end{aligned}
$$
Calculando el producto de las incertidumbres
$$
\begin{aligned}
\Delta x \Delta p &= \sqrt{\langle \hat{x}^2 \rangle - \langle \hat{x} \rangle^2} \cdot \sqrt{\langle \hat{p}^2 \rangle - \langle \hat{p} \rangle^2} \\[10pt]
&= \sqrt{\langle \hat{x}^2 \rangle} \cdot \sqrt{\langle \hat{p}^2 \rangle} \\[10pt]
&= \sqrt{ \left( \frac{3\hbar}{2m\omega} \right) } \cdot \sqrt{ \left( \frac{3}{2}m\hbar\omega \right) } \\[10pt]
&= \sqrt{ \frac{9\hbar^2}{4} } \\[10pt]
&= \frac{3}{2}\hbar
\end{aligned}
$$
Verificando el principio de incertidumbre para este estado del oscilador armónico
$$
\frac{3}{2}\hbar \geq \frac{\hbar}{2}  
$$
como $\frac{3}{2}$ es mayor que $\frac{1}{2}$ entonces se cumple el principio de incertidumbre para este estado.
### Problema 4
![[Pasted image 20260723144352.png]]

Usando la energía del oscilador armónico clásico
$$
\begin{aligned}
E&=\frac{1}{2}m\dot{x}^{2} + \frac{1}{2}kx^{2} \\[10pt]
&=\frac{1}{2} m \dot{x}^{2} + \frac{1}{2} m \omega^{2} x^{2}
\end{aligned}
$$
tomamos el caso de $E_{0}$ donde tenemos amplitud máxima $x=A$ 
$$
\begin{align}
E_{0}&=\frac{1}{2} m\omega^{2}A^{2} = \frac{h\omega}{2}\\[10pt]  \\
A &= \sqrt{ \frac{\hbar}{m\omega} }
\end{align}
$$
Ahora, para determinar la probabilidad de encontrar la partícula en la región clásicamente prohibida. Recordemos que la ec. de onda para el estado fundamental de esta partícula es:
$$
\psi_{0} = \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} e^{-m\omega x^{2}/2\hbar}
$$
la probabilidad de encontrar la partícula es
$$
\begin{aligned}
P(|x|>A)&= \int_{-\infty}^{-A} \left(\frac{m\omega}{\pi \hbar}\right)^{1/2} e^{-m\omega x^{2}/\hbar} dx \, + \int_{A}^{\infty} \left(\frac{m\omega}{\pi \hbar}\right)^{1/2} e^{-m\omega x^{2}/\hbar} dx \\[10pt]
&= 2 \left(\frac{m\omega}{\pi \hbar}\right)^{1/2} \int_{A}^{\infty} e^{-m\omega x^{2}/\hbar} \,dx \\[10pt]
&=\frac{2}{\sqrt{ \pi }} \left( \frac{m\omega}{ \hbar} \right)^{1/2} \int_{1}^{\infty} \sqrt{ \frac{\hbar}{m\omega} }e^{-u^{2}} du\\[10pt]
&= \frac{2}{\pi} \int_{1}^\infty e^{-u^{2}} du \\[10pt]
&= \text{erfc(1)}
\end{aligned}
$$
Nota: $\frac{2}{\pi} \int_{A}^\infty e^{-u^{2}} du = \text{erfc(A)}$ esa es la función error que se calcula numéricamente y en este caso es approx. $0.1573$.

### Problema 5
![[Pasted image 20260723153821.png]]
Comenzamos planteando la ec. de onda. Sabemos que la ec. de onda independiente del tiempo se define como: $\hat{H}\psi=E\psi$ tal que
$$
\begin{cases} 
-\frac{\hbar^{2}}{2m} \frac{d^{2}}{dx^{2}} \psi(x) + \frac{1}{2} m\omega^{2}x^{2} \psi(x) = E \psi(x) & \text{si } x \geq 0 \\[10pt]
-\frac{\hbar^{2}}{2m} \frac{d^{2}}{dx^{2}} \psi(x) + V(x)\psi(x) = E\psi(x) & \text{si } x < 0 
\end{cases}
$$
Cuando nos ubicamos en $x=0$, la función de onda se enfrenta a un potencial infinitamente grande, por lo tanto la partícula no puede atravesar y eso nos dice que $\psi(0) =0$.
Si hacemos el análisis en el infinito tenemos que el potencial $\lim_{ x \to \infty }\frac{1}{2}m\omega^{2}x^{2} = \infty$, lo que nos dice que la función de onda tiene que ser cero $\psi(x\rightarrow \infty) = 0$. Finalmente, esto nos dice que la partícula está en un estado ligado (confinada). 
Con esto podemos definir las condiciones de contorno
$$
\begin{cases}
\psi(0) = 0\\ \\
\psi(x\rightarrow \infty) = 0
\end{cases}
$$
Para determinar el subconjunto de soluciones que satisfacen las condiciones de contorno impuestas por la pared infinita primero debemos plantear la ec. de onda:
$$
\psi_{n}(x) \propto H_{n}(\alpha x) e^{-\alpha^{2}x^{2}/2}
$$
Si evaluamos en cero
$$
\psi_{n}(0) \propto H_{n}(0)e^{0} =0
$$
por la recurrencia y paridad de los polinomios de Hermite donde todos los términos pares dependen del primer término par $H_{0}$, donde ninguno de los polinomios de Hermite pares $H_{2k}$ son cero en el origen, así incumpliendo nuestra condición de contorno. Por lo tanto, podemos concluir que todos los estados pares de la función de onda **se descartan**. Asimismo, el subconjunto de soluciones es $n = 1, 3, 5, 7 \dots$ con $n = 2k + 1, \forall k = 0, 1, 2, 3 \dots$

Ahora, para escribir los niveles de energía usamos la ec. de la energía del oscilador armónico cuántico $E=\hbar \omega\left( n+\frac{1}{2} \right)$:
$$
E_{k} = \hbar \omega\left( k+\frac{3}{2} \right),\, k=0, 1,2,3,\dots
$$
si tomamos $E_0$, obtenemos 
$$
E_{0} = \frac{3}{2}\hbar \omega
$$
donde el nivel fundamental del oscilador está un "paso" más arriba que el oscilador armónico simétrico ya que el potencial "destruye" el estado fundamental simétrico $n=0$ y esto causa que todos los estados pares ya no sean posibles.

### Problema 6
![[Pasted image 20260723162658.png]]
Nuestra nueva ecuación de onda $\hat{H}\psi=E\psi$ es:
$$
\begin{aligned}
-\frac{\hbar^{2}}{2m} \frac{d^{2}}{dx^{2}} \psi + \left(\frac{1}{2}m\omega^{2}x^{2} - qE_{0}x\right) \psi &=E\psi \\[10pt]
\end{aligned}
$$
Analizamos el potencial
$$
\begin{aligned}
V(x) &= \frac{1}{2} m\omega^{2}x^{2} - qE_{0}x \\[10pt]
&\text{completando cuadrados. NO HACERLO ASÍ, esto fue pura obstinación de mi parte.}\\[10pt]

&=\frac{1}{2} m\omega^{2}x^{2} - \frac{2qE_{0}x \sqrt{ m }\omega}{2\sqrt{ m }\omega} + \frac{q^{2}E_{0}^{2}}{2m\omega^{2}} - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}} \\[10pt]

&= \left(\frac{1}{\sqrt{2}}\sqrt{ m }\omega x-\frac{qE_{0}}{\sqrt{ 2m }\omega}\right)^{2} - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}} \\[10pt]
&\text{Hacerlo de la siguiente manera: Completando cuadrados y factorizando}\\[10pt]
&= \frac{1}{2} m\omega^{2} \left( x^{2}-\frac{2qE_{0}x}{m\omega^{2}} \right)\\[10pt]
&=\frac{1}{2}m\omega^{2} \left( x^{2}-\frac{2qE_{0}x}{m\omega^{2}} +\frac{q^{2}E_{0}^{2}}{m^{2}\omega^{4}} - \frac{q^{2}E_{0}^{2}}{m^{2}\omega^{4}} \right) \\[10pt]
&=\frac{1}{2} m\omega^{2} \left( x-\frac{qE_{0}}{m\omega^{2}}   \right)^{2} - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}}

\end{aligned}
$$
Con este cambio algebraico, el Hamiltoniano nos queda de la siguiente forma:
$$
\hat{H} = \frac{\hat{p}^{2}}{2m} + \frac{1}{2} m\omega^{2} \left( \hat{x}-\frac{qE_{0}}{m\omega^{2}}   \right)^{2} - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}}
$$
esto directamente nos dice que tenemos el "cero" del potencial desplazado en $\frac{qE_{0}}{m\omega^{2}}$ ya que tenemos la forma de $(x-x_{0})^{2}$. Haciendo un análisis de autovalores:
Definimos nuestro Hamiltoniano:
$$
\hat{H}_{o} = \frac{\hat{p}^{2}}{2m} + \frac{1}{2}m\omega^{2}(\hat{x}-x_{0})^{2}
$$
donde podemos definir $\hat{x}-x_{0} \equiv \hat{X}$. Donde $x_{0}$ al ser una constante, se mantienen las relaciones de conmutatividad de $[\hat{X},\hat{p}]=i\hbar$. Entonces, los autovalores del hamiltoniano $\hat{H}_{o}=\frac{\hat{p}^{2}}{2m} + \frac{1}{2}m\omega^{2}\hat{X}^{2}$ son los mismos autovalores que los del hamiltoniano del oscilador armónico:
$$
\begin{align}
\hat{H}_{o}\psi &=E\psi \\[10pt]
\hat{H}_{o}\psi &=\left( \hbar \omega\left( n+\frac{1}{2} \right) \right) \psi
\end{align}
$$
Asimismo, podemos definir nuestro hamiltoniano original como: 
$$
\hat{H} = \hat{H}_{o} -\frac{q^{2}E_{0}^{2}}{2m\omega^{2}}
$$
Si ponemos esto en una ecuación de autovalores
$$
\begin{align}
\hat{H} \psi &= (\hat{H}_{o}-\frac{q^{2}E_{0}^{2}}{2m\omega^{2}}) \psi \\[10pt]
\hat{H}\psi &=(\hat{H}_{o}\psi - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}}\psi) \\[10pt]
\hat{H}\psi &= \left( \hbar \omega\left( n+\frac{1}{2} \right) \right) \psi- \frac{q^{2}E_{0}^{2}}{2m\omega^{2}} \psi \\[10pt] \\

\hat{H}\psi &= \left( \hbar \omega\left( n+\frac{1}{2} \right) - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}}\right) \ \psi 
\end{align}
$$
con esto podemos ver que la energía es:
$$
E_{n} =  \left( \hbar \omega\left( n+\frac{1}{2} \right) - \frac{q^{2}E_{0}^{2}}{2m\omega^{2}}\right)
$$
la cual es prácticamente la misma energía del oscilador armónico cuántico, pero con un desplazamiento.