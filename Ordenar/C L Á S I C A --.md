# C L Á S I C A

- $\substack{ \Huge \textsf{\textbf{\color{thistle}Lagrange}}\\[-1.23em] \frac{\ \ \ \ \ \ \ \ }{}\ L\ a\ g\ r\ a\ n\ g\ e\frac{\ \ \ \ \ \ \ \ }{} }$


# $\colorbox{Lavender}{Esfera en tubo rotando}$
        

        
        El problema consiste en una partícula de masa $m$ dentro de un tubo rígido el cual rota con $\phi = \omega t$ en el plano $x-y$. 
        
        El sistema tiene un grado de libertad ya que necesitamos solo una coordenada para describirlo, $r$ la distancia de la esfera al centro de giro.  Para este  problema $V=0$ y las ecuaciones de movimiento de un oscilador armónico no amortiguado. Sin embargo la solución para $t\to \infty$ hará que el radio también se vaya a infinito, esto debido a que la fuerza  centrifuga empujará a la esfera cada vez más fuera del radio de giro aumentando su energía.
        
		 
# $\colorbox{orangered}{Péndulo vertical}$
        

        
        Este problema consiste en una barra rigida que oscila en tal que $h(t)=h_0 \cos \omega t$. En el extremo de la barra hay una masa $m$ que hace un ángulo $\theta$ con la vertical. 
        
        Para determinar las ecuaciones de movimiento, podemos describir el sistema con el ángulo $\theta$ el cual es el único grado de libertad del sistema. Luego de encontrar las ecuaciones de Euler-Lagrange y hacer aproximación para ángulos pequeños nos queda una ecuación de segundo orden con forzamiento. Si el pistón está en reposo recuperamos la ecuación del péndulo.
        
    - $\colorbox{orchid}{Frecuencias de vibración de una molécula de tres átomos simétrica}$
        

        
        Se debe encontrar las frecuencias de vibración de una molécula $ABA$. El potencial solo dependerá de la distancia entre vecinos. 
        
        Para este problema podemos escribir el lagrangiano en coordenadas normales y así encontrar las ecuaciones de vibración de cada  átomo de forma desacoplada. 
        
        $L=\sum_\alpha \frac{m_\alpha}{2}(\dot{\Theta_\alpha}^2-\omega^2_\alpha\Theta^2_{\alpha})$.
        
        Acá definimos el desplazamiento del átomo $\alpha$ desde su posición de equilibrio $r_{0\alpha}$ como $x_{\alpha}=x_{\alpha}$. Se asume que la fuerza que mantiene unidos a los átomos es lineal a primer orden. Para este caso el lagrangiano en términos de $x_\alpha$ es:
        
        $L=\frac{m_{A}}{2}(\dot{x}^2_1+\dot{x}^2_3)+\frac{m_B}{2}\dot{x_2}^2-\frac{K}{2}[(x_1-x_2)^2+(x_3-x_2)^2]$. Luego podemos eliminar $x_2$ del lagrangiano ya que el movimiento del centro de masa del sistema satiface la ecuación $m_A(x_1+x_3)m_Bx_2=0$. Luego definimos las coordenadas normales para desacoplar las ecuaciones de movimiento.
        
    - $\colorbox{lavender}{Pequeñas oscilaciones}$
        
        March 18, 2021 1:58 PM 
        
        Un sistema de s grados de libertad se puede generalmente para pequeñas oscilaciones como $L=\frac{1}{2}\sum\limits_{i,j}(m_{ik}\dot{x_i}\dot{x_k}-k_{ik} x_{i}x_{k})$. La ecuación de autofrecuencias del sistema es determinada por. 
        
        $\det|k_{i,k}-\omega^2 m_{i,k}|=0$.
        
    - $\colorbox{teal}{Masas puntuales acopladas en un círculo}$
        
        March 17, 2021 11:30 PM 
        
        El problema consiste en tres masas de masa $m$, conectadas por resortes de constante $k$ en un anillo. No hay potencial gravitatorio actuando.
        
        Para resolver el problema primero observamos que cada masa se mueve en un elemento de arco $s_i$ y la interacción con los vecinos será la interacción del resorte.
        
        El potencial de interacción para desplazamientos de la posición de equilibrio es: 
        
        $V=\frac{1}{2}\sum\limits_{i=1}^4(s_{i+1}-s_{v})^2$. El elemento de arco $s_i=R \phi_i$, donde $\phi_i$ es la coordenada generalizada del sistema.
        
        Luego escribimos el lagrangiano y las ecuaciones de movimiento. 
        
        Las ecuaciones de movimiento serán $4$ ecuaciones acopladas, donde podemos usar la ecuación caracteristica para encontrar las autofrecuencias del sistema y los autovectores para luego poder desacoplar el sistema y escribirlo en sus coordenadas normales.
        
        Nota: Una vez encontradas las ecuaciones de movimiento se  prueba el Ansatz $\phi_i=A_i \cos{\omega t}$ donde luego los coeficientes  van en la ecuación característica.
        
    
# - $\colorbox{thistle}{Ecuaciones de Hamilton}$
    
    Conociendo el Hamiltoniano de un sistema podemos conocer las ecuaciones de Hamilton, las cuales nos entregan un conjunto de ecuaciones diferenciales que describen la evolución de un sistema.
    
    $\texttt{Derivada total:}$ $f(x,y,z) \to df = \partial_x f dx \partial_y f dy +\partial_z dz$.
    
    El Hamiltoniano se relaciona con el Lagrangiado a través de una transformada de Legendre:
    
    $L(\dot{q},q)\leftrightarrow H(q,p)$: $H=p\dot{q}-L$; $L=p\dot{q}-H$; $p=-\partial_{\dot{q}}L$.
    
    Para obtener las ecuaciones de Hamilton, tomamos la derivada total de $H(q,p,t)$.