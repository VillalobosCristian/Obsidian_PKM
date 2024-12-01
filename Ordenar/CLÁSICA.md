**C L Á S I C A**


• $\colorbox{Lavender}{Esfera en tubo rotando}$

El problema consiste en una partícula de masa $m$ dentro de un tubo rígido el cual rota con $\phi = \omega t$ en el plano $x-y$.

El sistema tiene un grado de libertad, ya que necesitamos solo una coordenada para describirlo: $r$, la distancia de la esfera al centro de giro. Para este problema $V=0$, y las ecuaciones de movimiento corresponden a un oscilador armónico no amortiguado. Sin embargo, la solución para $t \to \infty$ hará que el radio también se vaya a infinito, debido a que la fuerza centrífuga empujará a la esfera cada vez más lejos del centro de giro, aumentando su energía.

• $\colorbox{orangered}{Péndulo vertical}$

Este problema consiste en una barra rígida que oscila tal que $h(t) = h_0 \cos \omega t$. En el extremo de la barra hay una masa $m$ que hace un ángulo $\theta$ con la vertical.

Para determinar las ecuaciones de movimiento, podemos describir el sistema con el ángulo $\theta$, el cual es el único grado de libertad del sistema. Luego de encontrar las ecuaciones de Euler-Lagrange y hacer una aproximación para ángulos pequeños, obtenemos una ecuación de segundo orden con forzamiento. Si el pistón está en reposo, recuperamos la ecuación del péndulo clásico.

• $\colorbox{orchid}{Frecuencias de vibración de una molécula de tres átomos simétrica}$

Se deben encontrar las frecuencias de vibración de una molécula $ABA$. El potencial solo depende de la distancia entre vecinos.

Para este problema, podemos escribir el lagrangiano en coordenadas normales y así encontrar las ecuaciones de vibración de cada átomo de forma desacoplada:

$$

L = \sum_\alpha \frac{m_\alpha}{2}(\dot{\Theta}_\alpha^2 - \omega_\alpha^2 \Theta_\alpha^2).

$$

Aquí, definimos el desplazamiento del átomo $\alpha$ desde su posición de equilibrio $r_{0\alpha}$ como $x_\alpha$. Se asume que la fuerza que mantiene unidos a los átomos es lineal a primer orden. En este caso, el lagrangiano en términos de $x_\alpha$ es:

$$

L = \frac{m_A}{2}(\dot{x}_1^2 + \dot{x}_3^2) + \frac{m_B}{2}\dot{x}_2^2 - \frac{K}{2}[(x_1 - x_2)^2 + (x_3 - x_2)^2].

$$

Luego, eliminamos $x_2$ del lagrangiano, ya que el movimiento del centro de masa satisface la ecuación $m_A(x_1 + x_3) + m_B x_2 = 0$. Definimos las coordenadas normales para desacoplar las ecuaciones de movimiento.

• $\colorbox{lavender}{Pequeñas oscilaciones}$

Un sistema con $s$ grados de libertad puede generalmente describirse para pequeñas oscilaciones como:

$$

L = \frac{1}{2}\sum\limits_{i,j}(m_{ik}\dot{x}_i\dot{x}_k - k_{ik} x_i x_k).

$$

La ecuación de autofrecuencias del sistema se determina con:

$$

\det|k_{i,k} - \omega^2 m_{i,k}| = 0.

$$

• $\colorbox{teal}{Masas puntuales acopladas en un círculo}$

El problema consiste en tres masas de masa $m$, conectadas por resortes de constante $k$ en un anillo. No hay potencial gravitatorio actuando.

Para resolver el problema, primero observamos que cada masa se mueve en un elemento de arco $s_i$ y la interacción con los vecinos es la interacción del resorte.

El potencial de interacción para desplazamientos desde la posición de equilibrio es:

$$

V = \frac{1}{2}\sum\limits_{i=1}^4(s_{i+1} - s_i)^2.

$$

El elemento de arco es $s_i = R \phi_i$, donde $\phi_i$ es la coordenada generalizada del sistema.

Luego escribimos el lagrangiano y las ecuaciones de movimiento. Estas serán cuatro ecuaciones acopladas. Usamos la ecuación característica para encontrar las autofrecuencias del sistema y los autovectores. Esto permite desacoplar el sistema y escribirlo en sus coordenadas normales.

Nota: Una vez encontradas las ecuaciones de movimiento, probamos el ansatz $\phi_i = A_i \cos{\omega t}$, donde los coeficientes se insertan en la ecuación característica.

• $\colorbox{thistle}{Ecuaciones de Hamilton}$

Conociendo el Hamiltoniano de un sistema, podemos determinar las ecuaciones de Hamilton, las cuales son un conjunto de ecuaciones diferenciales que describen la evolución del sistema.

**Derivada total:** $f(x, y, z) \to df = \partial_x f dx + \partial_y f dy + \partial_z f dz$.

El Hamiltoniano se relaciona con el lagrangiano a través de una transformada de Legendre:

$$

L(\dot{q}, q) \leftrightarrow H(q, p): \quad H = p\dot{q} - L; \quad L = p\dot{q} - H; \quad p = -\partial_{\dot{q}}L.

$$

Para obtener las ecuaciones de Hamilton, tomamos la derivada total de $H(q, p, t)$.