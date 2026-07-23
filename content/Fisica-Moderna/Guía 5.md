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
