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