# E l e c t r o

$\colorbox{thistle}{Importante/General}$

$\colorbox{orange}{Interesante}$

$\colorbox{aquamarine}{Aplicación}$

- $\colorbox{thistle}{Importante/General}$
    
    March 13, 2021 2:54 AM 
    
    - $\colorbox{thistle}{Ecuaciones de Maxwell}$
        
        Las ecuaciones de Maxwell rigen la dinámica de los campos electromagnéticos. Unifican la electricidad y el magnetismo en 4 ecuaciones.
        
        $$
        \nabla \cdot \bold{E}=\rho/\epsilon_0   
        $$
        
        La primera ecuación se conoce como ley de Gauss. Nos dice que la cantidad de lineas de campo que sale o entra de un volumen $V$ es proporcional a la carga que está encerrada en ese volumen. En su forma integral se escribe como $\oint \bold{E}\cdot d\bold{S}=Q_{enc}/\epsilon_0$.
        
        La segunda ecuación de Maxwell nos da cuenta de la no existencia de monopolos magnéticos.
        
        $$
        \nabla \cdot \bold{B}=0
        $$
        
        Esta ecuación nos dice que el flujo neto de lineas de campo magnético es cero, debido a que dentro de un volumen $V$ cualquiera hay un dipolo magnético que hace que las lineas se cancelen en total. En su forma integral la ecuación queda como $\oint \bold{B}\cdot d\bold{S}=0$.
        
        La tercera ecuación de Maxwell unifica efecto magnéticos y eléctricos. 
        
        $$
        \nabla \times \bold{E}=-\frac{\partial \bold{B}}{\partial t}.
        $$
        
        Esta ecuación, nos dice que si hay una circulación de campo eléctrico, el campo magnético debe cambiar en el tiempo. En otras palabras, campos magnéticos variables en el tiempo generan campos eléctricos capaces de generar corrientes. En forma integral, es más fácil ver el significado físico. $\oint \bold{E}\cdot d\bold{l}=-\int_s \frac{\partial B}{\partial t}d\bold{S}$. El cambio de flujo magnético sobre una superficie $S$ es igual a la circulación del campo eléctrico.
        
        La cuarta ecuación de Maxwell explica como las cargas eléctricas en movimientos generan campos magnéticos.
        
        $$
        \nabla \times \bold{B}=\mu_0\bold{j}+c^{-2}\frac{\partial \bold{E}}{\partial t}.
        $$
        
        La carga neta del sistema es conservada. Si $\rho$ cambia en el tiempo es porque existe una corriente de cargas entrando o saliendo de esa región.
        
        La ecuación de conservación de la carga es:
        
        $\partial_t \rho + \nabla \bold{J}=0$.
        
        De forma integral puede ser escrita como:
        
        $\frac{dQ}{dt}=\int_V d^3 x \partial_t=-\int_V d^3x \nabla \cdot \bold{J}=-\int_S \bold{J}\cdot d\bold{S}$.
        
    - $\colorbox{thistle}{Carga puntual}$
        
        Una densidad de carga puntual se puede expresar matemáticamente como $\rho(\bold{x})=Q\delta^3(\bold{x})$. Donde $\delta$ es la distribución delta de Dirac. Para una densidad puntual, reemplazando en la ecuación de Poisson tenemos una ecuación tipo Green(ver abajo).
        
        Si miramos lejos del origen, sabemos que el potencial será tipo $\varphi \propto \alpha/r$. Este potencial será solución de la ecuación de Laplace, recordar que $\nabla r = \bold{\hat{r}}$, es el vector unitario en coordenadas esféricas, por lo tanto $\bold{x}=r\bold{\hat{r}}$, usando la regla de la cadena $\nabla(\frac{1}{r})=\bold{\hat{r}}/r^3$.  Esto nos da que $\nabla^2 \varphi = -\alpha(\frac{\nabla\cdot{\bold{x}}}{r^3}-\frac{3\bold{x}  \cdot \bold{x} }{r^5})$. En coordenadas esféricas la divergencia de $\bold{x}$ es 3. Por lo tanto $\nabla^2 \varphi =0$, como se esferaba para una carga puntual en el origen. 
        
        $\texttt{Comentario delta Dirac}$: La delta de Dirac es una distribución, que se puede entender como un límite de funciones y cumple con $\int f(x)\delta{(x-a)} = f(a)$. Para $x\neq 0$ tenemos que $\delta =0$ y para $x=0$, $\delta = \infty$.
        
        Tiene unidades de $1/r^3$ y se debe escribir correctamente según las coordenadas.
        
        **EJ**: $\rho(\bold{x})=Q\delta({\bold{x})}$, integrando $\int_v d^3x \rho = Q$.
        
        Usando la Ley de Gauss, $\int_s \nabla \varphi \cdot d\bold{S}=-\frac{Q}{\epsilon_0}$. Eligiendo una superficie esférica $\bold{E} = -\frac{Q}{4\pi\epsilon_0r^2}\hat{\bold{\hat{r}}}$
        
    - $\colorbox{thistle}{Dipolo}$
        
        El dipolo eléctrico consiste en dos cargas puntuales $Q$ y $-Q$ separadas por una distancia $d$. Ponemos la primera carga en el origen y la segunda en $\bold{r}=-\bold{d}$. Por principio de superposición el potencial será la suma de los potenciales de cada carga.
        
        $\varphi = \frac{1}{4\pi\epsilon_0}(\frac{Q}{r}-\frac{Q}{|\bold{r}-\bold{d}}|)$. Nos interesa saber que ocurre cuando $|\bold{d}|\lll \bold{r}$, es decir, cuando estamos lejos de las cargas. Por qué nos interesa esto? porque cuando medimos campos físicos reales, medimos a distancias lejanas a las fuentes. Ya sean dos electrones o una placa cargada, estamos haciendo una especie de promedio de todos los dipolos que existen en el material. 
        
        Expandimos en Taylor $f(\bold{r+\bold{d}})\approx f(\bold{r})+\bold{d}\cdot{}\nabla f{\bold{(r)}}+\frac{1}{2}(\bold{d}\cdot{\nabla})^2f(\bold{r})+....$
        
        Por lo tanto:
        
        $\frac{1}{|\bold{r}+\bold{d}|}\approx\frac{1}{r}+\bold{d}\cdot{\nabla f(\bold{r})}+\frac{1}{2}(\bold{d}\cdot \nabla)^2\frac{1}{r}= \frac{1}{r}-\frac{\bold{d}\cdot\bold{r}}{r^3}-\frac{1}{2}(\frac{\bold{d}\cdot\bold{d}}{r^3}-\frac{3(\bold{d}\cdot \bold{r})^2}{r^5})+...$
        
        Luego $\varphi \approx \frac{Q}{4\pi\epsilon_0}(\frac{1}{r}-\frac{1}{r}-d_i\partial_i \frac{1}{r_i})=\frac{Q}{4\pi\epsilon_0}\frac{\bold{d}\cdot\bold{r}}{r^3}$.
        
        Vemos que el potencial para el dipolo cae como $1/r^2$ y por lo tanto el campo eléctrico $1/r^3$, lo cual es una potencia más grande que para una carga puntual. 
        
        Se define el momento dipolar como $\bold{p}=Q\bold{d}$. 
        
        Y el campo eléctrico como  $\bold{E}=-\nabla\varphi = \frac{1}{4\pi\epsilon_0}(\frac{3(\bold{p\cdot{\bold{\hat{r}}}})\bold{\hat{r}-\bold{p}}}{r^3})+...$
        
    - $\colorbox{thistle}{Energía  potencial de un sistema de cargas}$
        
        March 17, 2021 11:49 AM 
        
        La energía potencial de un sistema de cargas se puede interpretar como la energía necesaria para armar una  configuración debido a los campos existentes.
        
        Las configuraciones de carga se arman una por una tal que:
        
        $q^{1} \to W=U=0$.
        
        $q^2 \to W=U=U^{21}$.
        
        Para $N$ cargas se  puede escribir de dos formas:
        
        $U=\frac{1}{4\pi\epsilon_0}\sum\limits^{N}_{\alpha,\beta(\alpha>\beta)}  \frac{q^{\alpha}q^{\beta}}{|\bold{x}^{\alpha}-\bold{x}^{\beta}|}$.
        
        O para evitar  el sobre conteo y para $\beta$ distinto de $\alpha$.
        
        $U=\frac{1}{8\pi\epsilon_0}\sum\limits^{N}_{\alpha,\beta(\alpha\neq\beta)} \frac{q^{\alpha}q^{\beta}}{\bold{x}^{\alpha}-\bold{x}^{\beta}}$
        
        La densidad de energía en un volumen $V$ será proporcional al campo electrico al cuadrado. Esto tiene que implicaciones importante sobre las ondas electromagnéticas, ya que al hacer un tratamiento más microscópico de los campos EM debemos  considerar que el efecto macroscópico producido es un promedio sobre los efectos microscópicos y $E^2$ puede ser entendido como una probabilidad total y $E$ como una densidad de probabilidad, la cual satiface las ecuaciones de maxwell.
        
    - $\colorbox{thistle}{Separación de variables}$
        
        March 22, 2021 8:28 AM 
        
        Para campos eléctricos estáticos en el tiempo el campo eléctrico es conservativo y se puede escribir como $\bold{E}=-\nabla \varphi$. Esto en la primera ecuación de Maxwell (Ley de Gauss), nos entrega la ecuación de Poisson $\nabla^2 \varphi = -\rho/\epsilon_0$.
        
        En regiones del espacio donde la densidad de carga es cero, tenemos la ecuación de Laplace $\nabla^2 \varphi =0$.
        
        $\texttt{Sobre el potencial:}$ Si miramos la definición de campo eléctrico $\bold{E}=-\partial_i \varphi$, vemos que el potencial $\varphi$ puede ser definido más una constante aditiva sin cambiar el campo eléctrico físico original. $E=-\partial_i (\varphi + \lambda(t))$. En electroestática asumiremos que esa constante es $\varphi(\infty)=0$, pero será de ayuda cuando dependencias temporales entren en el problema.
        
        Como la ecuación de Laplace es lineal en $\varphi$ y en $\rho$, podemos usar el principio de superposición para encontrar soluciones. Además de los teoremas de unicidad. 
        
         
        
        Para resolver la ecuación de Laplace en un sistema de coordenadas ortogonales, podemos utilizar separación de variables, donde el objetivo es encontrar los coeficientes de de la solución. El proceso de separación de variables crea 3 ecuaciones diferenciales ordinarias de segundo orden para un gran número de sistemas de coordenadas.
        
        Sea $\nabla^2\phi=0$. La solución más general será:
        
        $\phi(u,v,w)=A(u)B(v)C(w)$.
        
        $\phi(u,v,w)= \sum\limits_{\alpha \beta \gamma}[a_{\alpha}A(u)+\tilde{a}_{\alpha}\tilde{A}(u)+b_{\beta}B(v)+\tilde{b}_{\beta}\tilde{B}(v)+ c_{\gamma}C(w)+\tilde{c}_{\gamma}\tilde{C}(w)]$.
        
        Para encontrar estos coeficientes se debe cumplir que:
        
        1. Satifacer las condiciones de borde.
        2. Permanecer finito en todo el volumen de la solución.
        3. Respetar las simetrías del problema físico.
        
        La ecuaciones diferenciales separadas deben tener condiciones de borde las cuales producen un problema de autovalores de Sturm-Lioville, el cual asegura que las autofunciones asociadas  son completas y ortonormales.  
        
        Las condiciones de borde necesarias para esto son:
        
        Dirichlet Homogéneas: $\phi =0$. 
        
        Neumann Homogéneas: 
        
        Periódicas
        
        - **Ortogonalidad en distintas coordenadas.**
            
            Un conjunto de autofunciones $\psi(v)$ es completo si cualquier función $F(v)$ definida en el mismo intervalo puede ser escrita como una combinación lin eal.
            
            $F(v)=\sum_k F_k \psi_k(v)$, con $a \leq v  \leq b$.
            
            La relación de clausura es:
            
            $\sum_k \psi_k (v)\psi_k^*(v')=\delta(v-v')$. Y la condición de ortonormalidad de las funciones:
            
            $\int_a^b dv \psi(v)^*_k \psi^*_j(v)=\delta_{kj}$.
            
            **Coordenadas cartesianas**:
            
            $\nabla^2 \phi = \partial^2_i \phi$, con $i=x,y,z$.
            
            Por separación de variables: $\phi(x,y,z)=X(x)Y(y)Z(z)$, esto nos entrega tres ecuaciones diferenciales para cada coordenada.
            
            - **Caja vacia con 5 paredes a potencial cero y la pared inferior $z=0$ a $V(x,y)$.**
                
                Las soluciones para cada ecuación de la separación de variables viene dada por:
                
                $X_{\alpha}(x)=A_0+ B_0 x$ para $\alpha =0$
                
                $X_\alpha(x)=A_{\alpha}e^{\alpha x}+B_\alpha e^{-\alpha x}$ para $\alpha \neq 0$.
                
                Las ecuaciones para las otras coordenadas tienen la misma forma donde se debe satifacer $\alpha^2+\beta^2+\gamma^2=0$, donde $\beta$ y $\gamma$ son los coeficientes de $Y,Z$ respectivamente.
                
                Como la solución se puede escribir como la multiplicación de las soluciones elementarias, en coordenadas cartesianas tenemos:
                
                $\phi(x,y,z)=\sum\limits_{\alpha \beta \gamma}X_{\alpha}(x)Y_{\beta}(y)Z_{\gamma}(z)\delta(\alpha^2+\beta^2+\gamma^2)$, aquí la delta asegura que que se cumpla la condición para los coeficientes. Los valores de los coeficientes pueden ser reales o imaginarios.
                
                El problema entonces consiste en encontrar los coeficientes. La situación indica que el potencial en $X$ y en $Y$ debe ser cero, por lo que para satifacer esa condición $\alpha$ puede ser escrito como $\alpha' i$, lo mismo para $\beta$.
                
                Tenemos por lo tanto para que se cumplan las condiciones de Dirichlet:
                
                $\phi(a,b,z)=\sum\limits_{\alpha \beta \gamma}(A_{\alpha}e^{i\alpha a}+B_\alpha e^{-i\alpha a})(C_{\beta}e^{i\beta a}+D_\beta e^{-i\beta a})Z_{\gamma}(z)\delta(\alpha^2+\beta^2+\gamma^2)=0=\phi(0,0,0)$, para que se cumpla sabiendo que $Z_{\gamma}\neq 0$, Entonces para $X,Y$ podemos usar funciones sinusoidales... porque $\phi_{x,y}(0,0)=0 \to AC_{\alpha \beta} = -BD_{\alpha \beta}, \to \tilde{AC}\sin(\alpha \beta x) = 2iAC\sin(\alpha \beta x)$, ya que las constantes no tienen por qué ser reales podemos absorver el factor $2i$.
                
                Luego para $\phi(a,b,z)=0$ se cumplirá para $\alpha = \frac{m\pi}{a}$ y $\beta = \frac{n\pi}{b}$.
                
                Por lo tanto:
                
                $\phi(x,y,z)=\sum\limits_{m=1}\sum\limits_{n=1}\sin(\frac{m\pi x}{a})\sin(\frac{n\pi y}{b})[E_{mn}e^{\gamma_{mn}z}+F_{mn}e^{-\gamma_{mn}z}]$, donde $\gamma^2 = (\frac{m\pi}{a})^2+(\frac{n\pi}{b})^2$.
                
                Ahora para determinar los demás coeficientes, exigimos que el potencial sea $0$ en $z=c$.
                
            
    - $\colorbox{thistle}{Ecuación  de Poisson y función de Green}$
        
        March 31, 2021 5:04 PM 
        
        Para resolver la ecuación de Poisson $\nabla^2 \Phi=-\rho/\epsilon_0$, la cual es  una ecuación diferencial inhomogénea de segundo orden podemos emplear el método de funciones de green, donde el resultado a la ecuación en el espacio de ""Green"" estará dado por:
        
        $\nabla^2 G(\bold{r,r'})=-4\pi\delta({\bold{r-r'}})$. cuya solución es 
        
        $G(\bold{r,r'})=\frac{1}{|\bold{r}-\bold{r'}|}+F(\bold{r,r'})$. Donde $F$ satiface la ecuación de Laplace.
        
        **Función de Green para una esfera**
        
        La solución del potencial de una carga puntual cerca de una esfera conductora cargada está dado por la función de Green de la ecuación de Poisson con condiciones de borde de Dirichlet.
        
        $G_D(\bold{r,y})=\frac{1}{|\bold{r}-\bold{y}|}-\frac{a}{y|\frac{a^2}{y^2}\bold{y}-\bold{r}|}$.
        
        - Figura
            
            
            ![../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled.png](../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled.png)
            
    - $\colorbox{thistle}{Ecuación de Laplace coordenadas esféricas}$
        
        $\nabla^2\varphi(r,\theta,\phi)=0$, donde $r$ es la distancia radial desde el origen hasta el punto de observación. $\theta$ es el ángulo polar  y $\phi$ el ángulo azimutal. 
        
        Se prueba separación de variables con $R(r)/r$ en vez de $r$ para facilitar los cálculos. 
        
        Luego de reemplazar el Laplaciano en las coordenadas esféricas, se puede factorizar tal que un lado de la ecuación dependa de $R$ y otro de $\theta$ y $\phi$.
        
        Probando solución en serie de potencias se llega a:
        
        $\varphi(r,\theta,\phi)=\sum\limits_{m,l}(A_l r^l + B_l r^{-l-1})(A_m e^{im\phi}+B_m e^{-im\phi})P^m_l(\cos{\theta})$. Donde $P^m_l$ son los polinomios de Legendre.
        
        Cuando $m=0$, y el ángulo azimutual existe entre $[0,2\pi]$. Se dice que tenemos simetría azimutal. Los polinomios de Legendre no están definidos para $l<0$ por lo que el caso $l=0$ se trata separado al caso $l>0$.
        
        Para encontrar los coeficientes hay que usar la relación de ortogonalidad:
        
        $\int_0^\pi P_{l'}(\cos{\theta})P_{l}(\cos{\theta})\sin{\theta}d\theta=\frac{2}{2l+1}\delta_{l',l}$.
        
        La solución general queda como:
        
        $\varphi(r,\theta,\phi)=\sum\limits_{m,l}(A_l r^l + B_l r^{-l-1})P_l(\cos{\theta})$.
        
        - $\texttt{Ejemplo:}$Esfera conductora a potencial $\varphi(\theta)$ en la superficie. Encontrar potencial dentro de la esfera.
            1. Vemos primero las zonas donde queremos encontrar solución. Como es dentro de la esfera, el potencial no se puede indeterminar en el origen por lo que $B_l=0$ para $r<a$.
            2. El potencial por lo tanto es: $\varphi(r,\theta)=\sum\limits_{l=0}^\infty A_l r^l P_l(\cos{\theta})$.
            3. En la superficie el potencial es $\varphi(a,\theta)=\varphi(\theta)=\sum\limits_{l=0}^\infty A_l a^l P_l(\cos{\theta})$. 
            4. Solo queda determinar el coeficiente $A_l$ para esta condición de borde.
            5. Usando ortogonalidad $\int^\pi_0 \varphi(\theta)P_{l'}(\cos{\theta})\sin{\theta}d\theta = \sum\limits_{l=0}^\infty A_l a^l \int^\pi_0 P_{l}(\cos{\theta})P_{l'}(\cos{\theta})\sin{\theta}d\theta=A_la^l  \frac{2}{2l+1}\delta_{l,l}$.
            6. Con la condiciónde ortonormalidad tal que: $\int_0^\pi P_{l'}(\cos{\theta})P_{l}(\cos{\theta})\sin{\theta}d\theta=\frac{2}{2l+1}\delta_{l',l}$.
            7. El coeficiente es. $A_{l}=\frac{2l+1}{2a^l}\int^{\pi}_0 \varphi(\theta)P_{l}(\cos{\theta})\sin{\theta}d\theta$.
            8. Por lo tanto $\varphi$ dentro de la esfera es: $\varphi(r,\theta)=\sum\limits_{l=0}^\infty A_l(\frac{r}{a})^l P_l(\cos{\theta})$.
            
        
    - $\colorbox{thistle}{Campos en la materia}$
        
        
    - $\colorbox{thistle}{Magnetistmo}$
        - March 16, 2021 12:08 AM Jackson 5.13. Esfera rotando con $\omega$ y con densidad de corriente superficial $\sigma$. Encontrar el vector potencial, y la densidad de flujo magnético. Además el campo magnético dentro  y fuera. $\vec{B} =\nabla\times \vec{A}$.
            1. Cuando la esfera rota genera densidades de corriente $\bold{K}$ en  la superficie de la esfera. 
            2. Esta densidad de corriente genera campo magnético, el cual tiene asociado un vector de campo magnético y un vector potencial magnético
            3. El vector potencial $\bold{A}$ está relacionado con la densidad superficial de carga.
            4. Calculando el vector $\bold{A}$ en coordenadas esféricas con el eje $\hat{z}$ paralelo al vector $\omega \hat{z}$.
            5. Se proyecta a coordenadas esféricas el ángulo $\hat{\phi}$ y se expande $\frac{1}{|\bold{r}-\bold{r'}|}$ en armónicos esféricos.
            6. Se buscan los armónicos correspondientes y se usa ortogonalidad para resolver la integral.
    - $\colorbox{thistle}{Leyes de conservación}$
    - $\colorbox{thistle}{Potenciales}$
        
        March 29, 2021 5:51 AM 
        
        Los potenciales electromagéticos $\phi(\bold{r},t)$ y $A({\bold{r},t})$ satifacen las ecuaciones de Maxwell homogéneas y además reducen el número de funciones necesarias para determinar las cantidades eléctromagnéticas, desde 6 para cada componente de los campos a 4, una para $\phi$ y 3 para las componentes de $\bold{A}$.
        
        El campo eléctrico se puede escribir como $\bold{E}(\bold{r},t)=-\nabla \phi(\bold{r},t)-\partial_t \bold{A}(\bold{r},t)$, esto viene de la posibilidad de escribir el rotor del campo $\bold{E}$ más la derivada temporal de $\bold{A}$ igual a cero.
        
        Reemplazando los campos $\bold{E}$ y $\bold{B}$ en término de los potenciales en las ecuaciones inhomogeneas de Maxwell tenemos dos ecuaciones acopladas para los potenciales.
        
        $\nabla^2\phi +\partial_t (\nabla \cdot \bold{A})=-\rho/\epsilon_0$
        
        $\nabla^2\bold{A}-\frac{1}{c^2}\partial^2_t \bold{A}-\nabla(\nabla\cdot \bold{A}+\frac{1}{c^2}\partial_t \phi)=-\mu_0 \bold{j}$
        
        Estas ecuaciones se pueden desacoplar introduciendo los gauges de Lorentz: $\bold{A}'=\bold{A}+\nabla \lambda$ y $\phi'=\phi-\partial_t \lambda$. Este gauge deja invariante las cantidades $E$ y $B$. El gauge de Coulomb es: $\nabla \cdot \bold{A}=0$.
        
          Las ecuaciones de onda para los potenciales en el gauge de Lorentz son:
        
        $\nabla^2 \phi_L-\frac{1}{c^2}\partial^2_t \phi=-\rho/\epsilon_0$
        
        $\nabla^2 \bold{A}-\frac{1}{c^2}\partial^2\bold{A}=-\mu_0 \bold{j}$.
        
    - $\colorbox{thistle}{Electro y relatividad}$
        
        17/03/2021 9:44 PM 
        
        El postulado básico de la relatividad especial es que las leyes físicas son las mismas en todos los marcos de referencia inerciales. Nos ayuda a entender como miran las cosas observadores que se mueven uno respecto a otro.
        
        Un observador está en un marco incercial $\mathcal{S}$ con coordenadas $(ct,x,y,z)$. El segundo observador está en un marco de referencia inercial $\mathcal{S'}$ con coordenadas $(ct',x',y',z')$.
        
        Se definen las transformaciones de Lorentz para cuando $\mathcal{S'}$ se está moviendo con rapidez $v$ en la dirección $x$ relativa a $\mathcal{S}$, tal que los sistemas de coordenadas estén relacionados por un boost de Lorentz:
        
        $x'=\gamma(x-\frac{v}{c}ct)$ y $ct'=\gamma(ct-\frac{v}{c}x)$, mientras que $y=y'$ y $z=z'$. El factor $\gamma=\sqrt{\frac{1}{1-v^2/c^2}}$. 
        
        Por conveniencia se define el 4-vector con indices $\mu=0$ hasta $\mu=3$. 
        
        $X^{\mu}=(ct,x,y,z)$.
        
        Entonces una transformación de Lorentz lo que hace es mapear linealmente de $X$ hasta $X'$ de la forma: 
        
        $X^{'\mu}=\Lambda^{\mu}_\nu X^{\nu}$, donde $\Lambda$ es una matriz $4\times4$ que obedece las ecuaciones matricales:
        
        $\Lambda^T \eta \Lambda = \eta$, que se puede escribir por componentes como $\Lambda^{\rho}_\mu \eta_{\rho \sigma} \Lambda^{\sigma}_\nu=\eta_{\mu \nu}$, donde $\eta_{\mu \nu}$ es la metrica de Minkowski. Un vector diagonal $\text{diag}(+1,-1,-1,-1)$.
        
        El signo $+$ es convención.  De esta ecuación salen dos tipos de soluciones: 1) Rotaciones, 2) boost.
        
    - $\colorbox{aquamarine}{Ondas Electromagnéticas y Guia de Ondas}$
        
        March 27, 2021 2:36 PM 
        
        La onda electromagnética más general se propaga en el espacio y tiempo sin restricciones más que las impuestas por las ecuaciones de Maxwell. 
        
    - $\colorbox{aquamarine}{Radiación}$
        
        March 29, 2021 10:03 PM 
        
- $\colorbox{orange}{Interesante}$
    - 15/03/2021 8:51 AM **¿Cuál debe ser la velocidad de una carga $q$ que viaja con velocidad $\bold{v}$ paralela a un alambre con  densidad de carga $\lambda$ y corriente $I$ para que la trayectoria de la partícula se mantenga paralela al cable?**
        
        
        La carga se ve afectada por  la fuerza de lorentz debido al campo eléctrico y  al campo magnético producido por la corriente. El campo eléctrico del alambre lo podemos encontrar usando la ley de Gauss y el campo magnético producido por la corriente lo podemos encontrar con la ley de Ampere. La condición para que se mantenga con una trayectoria paralela al cable debe ser que la suma de fuerzas sea cero,tal que no se desvie.
        
    - March 14, 2021 6:50 AM **¿Cual es la mínima carga que se debe dar a una esfera conductora para que carga superficial sea en todos  lados positiva, si a distancia $d$ de la esfera hay una carga positiva $q$.**
        
        Este problema se puede resolver utilizando el método de imágenes. Debemos encontrar una configuración de cargas imágenes tal que el potencial sea constante en $r=a$. Esto es equivalente a resolver el problema de una carga a una distancia $d$ de una esfera conductora descargada + una carga en  el centro de la esfera. Esto por  principio de  superposición. La carga en el centro de la esfera inducirá carga en la parte interior de la  cascara esférica ya que el potencial en $r=a$ será el potencial producido por la carga de adentro. Al ser una esféra conductora, esta escomo un escudo para el campo eléctrico externo. La carga inducida en $r=a$ será $\sigma=-\epsilon_0\frac{\partial \phi}{\partial n}$. Reeemplazando para el potencial y luego se sabe que la carga será uniformemente distribuida en la superficie de la esfera, por lo tanto $\sigma = Q 4\pi a^2$. 
        
    - March 16, 2021 1:09 AM **Vacio esférico en un dieléctrico**
        
        El problema consiste en un dieléctrico el cual tiene un agujero esférico vacio, dentro del agujero hay un dipolo. Encontrar el campo en todos lados.
        
        El dipolo generará un campo dipolar dentro del vacio el cual en los bordes debe satifacer las condiciones de contorno para campos en la materia. El dipolo inducirá cargas en el dieléctrico, lo que hará que aparezca una polarización neta y por lo tanto un campo eléctrico dentro del vacio. El campo  total  dentro del dieléctrico será: Campo del dieléctrico+campo del dipolo y el campo en todo el espacio dieléctrico será el campo de desplazamiento $\bold{D}$. Donde se debe cumplir que  D es continuo en la interfaz.
        
    - March 24, 2021 7:31 AM **Esferas concéntricas llanas con mitad de dieléctrico**
        
        La esfera interior tiene carga $Q$ y la exterior carga $-Q$.  Por simetría puedo usar ley de Gauss para el vector desplazamiento eléctrico $\bold{D}$. En las superficies del conductor no hay diferencia de potencial, por lo que en la parte con dieléctrico y en la parte sin dieléctrico el potencial es continuo. Usamos la ley de Gauss para $\bold{D}$ la cual será la contribución de ambos campos, con y sin dieléctrico.
        
    - April 4, 2021 6:39 AM  **¿Qué pasa con una onda electromagnética si $\sigma$, $\mu$, $\epsilon$ no son constantes?**
        
        Aparece el efecto de dispersión. Esto hace que los electrones se muevan en el medio como una partícula amarrada a un resorte viscoso. El electrón tendrá momento dipolar proporcional a la parte real del campo. La parte imaginaria del campo da cuenta del desfase del movimiento del electrón con la onda incidente.
        
        Para estos materiales $\mathcal{X}$ es compleja.
        
    - March 11, 2021 1:29 PM **¿Que pasa con una esfera cargada que oscila??**
        
        Se podría pensar que la esfera emitirá radiación, ya que el movimiento de la superficie de la esfera se podría interpretar como una corriente, pero a diferencia de una esfera rotando, una esféra oscilante no tiene momento dipolar por lo que $\phi$ y $\bold{A}$ son cero. Por ley de Gauss la carga encerrada dipolar será cero. 
        
    - March 23, 2021 4:33 PM **Carga $Q$ dentro de una esfera hueca conductora**
        
        Calcular el campo dentro de la esfera.
        
        Podemos usar el método de imágenes colocando la carga imagen fuera de  la esfera. Recordar que las cargas imágenes no deben ir dentro de la zona donde queremos medir. 
        
        Asumiendo que $\phi=0$ en la superficie, calculamos la posición y magnitud de la carga imagen. 
        
        Si la esfera estuviera a potencial constante, se agrega otra carga en el origen tal que el potencial en la superficie sea constante. 
        
    - March 19, 2021 8:38 PM **¿Trabajo necesario para llevar un dipolo eléctrico que está a una distancia $h$ de un plano hasta el infinito?**
        
        Usamos el método de imágenes, reemplazando el plano por un dipolo imagen antiparalelo.  El dipolo se atrae el plano/otrodipolo ya que la parte negativa del dipolo está más cerca de la parte positiva del dipolo imágen. El campo que siente el dipolo debido al plano será el campo producido por el dipolo imagen. La energía potencial  de la configuración será $U=\bold{p}\cdot\bold{E}$ y el trabajo estará dado por $W=-\frac{\partial U}{\partial x}dx$. Luego de calcular el trabajo contra la carga imagen, dividimos por dos para dar cuenta el efecto del plano, ya que será la mitad de mover dos dipolos reales.
        
    - March 13, 2021 10:52 AM **Esfera dieléctrica en un medio dieléctrico**
        
        Encontrar el campo fuera y dentro de la esfera. 
        
        Como no hay fuentes de cargas, debemos resolver la ecuación de Laplace en coordenadas esféricas con simetria azimutal. Ponemos el origen en el centro de la esfera y exigimos que el potencial cumpla ser finito en el origen y que en infinito sea proporcional al campo eléctrico exterior que será el campo eléctrico de desplazamiento debido a la  polarización de las moleculas. 
        
        Ademas el potencial debe ser continuo en la superficie. Y el campo eléctrico será el gradiente del potencial.
        
        La carga inducida se puede encontrar escribiendo la polarización del dieléctrico como $\bold{P}=(\epsilon-\epsilon_0)\bold{E}$, luego $\sigma=\bold{n}\cdot \bold{P}$.
        
        Ojo, el vector polarización apunta en la misma dirección que el campo, por lo que rotar la esfera respecto a $z$ no inducirá corrientes de polarización ya que la dirección de $\bold{P}$ no cambia.
        
    - March 14, 2021 7:49 AM **Ley de Lenz**
        
        La ley de Lenz fija el signo de la ley de Faraday, tal que las corrientes inducidas y los campos magnéticos se opongan al cambio de flujo externo.
        
    - March 14, 2021 5:40 PM Is **the electric charge always a conserved quantity?**
        
        Yes, because.... 
        
        Sabemos que la carga siempre se conserva en un proceso físico. La única forma de cambiar la carga neta en un volumen finito es moviendo las partículas cargadas dentro o fuera del volumen. 
        
        La ecuación de conservación de la carga tiene la forma de una  ecuación de conservación $\frac{\partial \rho}{\partial t}+\nabla \cdot \bold{j}=0$, donde $\rho$ es la densidad de carga y $\bold{j}$ es la densidad de corriente. Esta ecuación nos dice que la carga total en cualquier  volumen infinitesimal es constante al menos que exista un flujo neto de cargas pre-existentes  que pasa por dentro o fuera del volumen.
        
    - March 24, 2021 8:08 AM **E c u a c i o n e s   d e   M a x w e l l**.
        
        Las ecuaciones de Maxwell rigen la dinámica de los campos electromagnéticos. Unifican la electricidad y el magnetismo en 4 ecuaciones.
        
        $$
        \nabla \cdot \bold{E}=\rho/\epsilon_0   
        $$
        
        La primera ecuación se conoce como ley de Gauss. Nos dice que la cantidad de lineas de campo que sale o entra de un volumen $V$ es proporcional a la carga que está encerrada en ese volumen. En su forma integral se escribe como $\oint \bold{E}\cdot d\bold{S}=Q_{enc}/\epsilon_0$.
        
        La segunda ecuación de Maxwell nos da cuenta de la no existencia de monopolos magnéticos.
        
        $$
        \nabla \cdot \bold{B}=0
        $$
        
        Esta ecuación nos dice que el flujo neto de lineas de campo magnético es cero, debido a que dentro de un volumen $V$ cualquiera hay un dipolo magnético que hace que las lineas se cancelen en total. En su forma integral la ecuación queda como $\oint \bold{B}\cdot d\bold{S}=0$.
        
        La tercera ecuación de Maxwell unifica efecto magnéticos y eléctricos. 
        
        $$
        \nabla \times \bold{E}=-\frac{\partial \bold{B}}{\partial t}.
        $$
        
        Esta ecuación, nos dice que si hay una circulación de campo eléctrico, el campo magnético debe cambiar en el tiempo. En otras palabras, campos magnéticos variables en el tiempo generan campos eléctricos capaces de generar corrientes. En forma integral, es más fácil ver el significado físico. $\oint \bold{E}\cdot d\bold{l}=-\int_s \frac{\partial B}{\partial t}d\bold{S}$. El cambio de flujo magnético sobre una superficie $S$ es igual a la circulación del campo eléctrico.
        
        La cuarta ecuación de Maxwell explica como las cargas eléctricas en movimientos generan campos magnéticos.
        
        $$
        \nabla \times \bold{B}=\mu_0\bold{j}+c^{-2}\frac{\partial \bold{E}}{\partial t}.
        $$
        
    - March 19, 2021 9:23 PM **¿Cuándo son las ondas electromagnéticas soluciones de las ecuaciones de Maxwell?**
        
        Cuando están en ausencia de fuentes.
        
    - March 17, 2021 9:13 AM **¿Cómo es la solución general de una ecuación de onda?**
        
        La solución general de una ecuación de onda es la suma de ondas viajando en distintas direcciones. $f(z,t)=g(z-vt)+h(z+vt$)
        
    - March 15, 2021 5:07 AM **Fuerzas magnéticas hacen trabajo?**
        
        Una fuerza magnética puede cambiar la dirección de $\bold{v}$ pero no su magnitud.
        
        mejorar
        
        ser conserva momentum?
        
    - April 4, 2021 12:00 PM **¿Qué pasa con el campo electromagnético cuando la densidad de carga y la densidad de corriente dependen del tiempo?**
        
        El campo electromagnético en un punto $P$ refleja el comportamiento de las fuentes en un tiempo anterior/retardado $t-r/c$, donde $\vec{r}$ es el vector desde un origen arbitrario $O$ hasta el punto $P$. Esto refiriendose a las fuentes. En las ecuaciones de Maxwell aparecen los términos variables en el tiempo
        
    - April 7, 2021 6:27 AM **¿Qué es la radiación electromagnética**?
        
        El campo electromagnético tiene una componente que transporta energía lejos de las fuentes al infinito, en un proceso que es irreversible. Esta componente es llamada radiación.
        
    - March 16, 2021 8:40 AM **¿Por qué tengo libertad de elegir los potenciales electromagnéticos?**
        
        Esta invarianza en el cambio de escala de los potenciales es posible principalmente por la forma de las ecuaciones de maxwell y las propiedades vectoriales, pero las consecuencias ayudan a imponer condiciones sobre los potenciales tal que se puedan medir los campos físicos reales.
        
    - April 3, 2021 9:15 PM **¿Cómo transforman los campos electromagnéticos?**
        
        Los campos $E$ y $B$ cambian cuando el sistema de referencia se mueve con velocidad $v$. Las transformaciones de Lorentz dan la relación entre las componentes tranversales y perpendiculares de los campos entre dos marcos de referencia.
        $\vec{E^{`}_{||}}=\vec{E_{||}}$ y $\vec{B^{`}_{||}}=\vec{B_{||}}$. Para la componente perpendicular $E^{'}_{\perp}=\gamma(\vec{E_{\perp}+\vec{v}\times \vec{B_\perp}})$ y $B^{'}_{\perp}=\gamma(\vec{B_{\perp}-\frac{\vec{v}\times \vec{E_\perp}}{c^2}})$.
        
    - April 6, 2021 9:23 PM ç**¿Qué es el efecto Hall**?
        
        El efecto Hall, ocurre cuando un campo magnético externo hace que las cargas se acumulen en un extremo de un cable, generando un  campo electrico tranversal.
        
        estudiaaaaaar
        
    - **¿Qué pasa si lleno un capacitor con un dieléctrico?**
        
        Cuando un material dielectrico(aislante) se pone dentro de un capacitor, hace que se polarizen las moléculas en el dieléctrico y la capacitancia aumenta en un factor $\kappa$.Ya que cerca de las laminas del capacitor se crean capas de carga que cancelan las cargas libres "aumentando la capacidad de almacenar carga"
        
    - March 12, 2021 4:34 PM **¿Que es la expansión multipolar?**
        
        Cuando tenemos una distribución de cargas, esta puede ser escrita como expansión en serie aumentando de $1/r$. Los coeficientes de esos términos se conocen como momentos. Una carga tiene un momento monopolar. Dos cargas opuestan crean un dipolo. Sobre un dipolo se puede generar torque el cual es proporcional al momento y al campo eléctrico
        
    
    Cómo cambia la capacitancia en un marco de referencia móvil
    
    - April 7, 2021 3:23 PM **¿Qué le ocurre a un material dieléctrico al entrar en contacto con un campo externo**?
        
        Los electrones de los átomos individuales salen de su posición de equilibrio por una mínima cantidad, pero no se despegan de sus átomos, debido a esto se crea un campo eléctrico dentro del material. Este proceso se llama polarización
        
    - March 28, 2021 8:49 PM **Por qué la carga en un conductor reside en su superficie, por qué un conductor hueco es un escudo para campos exteriores, pero no para cargas dentro?**
        
        La carga en un conductor reside en la superficie debido a que para cualquier superficie cerrada que se haga sobre la superficie dentro del conductor el campo debe ser cero, si uno hace una superficie infinitesimal en la superficie  y el exterior esta por ley de Gauss la carga encerrada que generará el campo estará en las últimas capas del conductor.
        
    - March 26, 2021 5:15 PM **¿Cómo es la fuerza entre las placas conductoras de un capacitor plano?**
        
        Como el campo es constante, basta con multiplicar  por el valor de la carga total del otro plano. 
        
    - March 17, 2021 4:34 PM **¿Explique el método de imágenes y por qué se puede utilizar?**
        
        El método de imagenes consiste en poder resolver un problema que incluye la interacción de una distribución de cargas y un conductor. El conductor se puede reemplazar por una configuración de cargas imaginarias que satifagan las condiciones a la que está en conductor. Por ejemplo, potencial constante, potencial cero, etc.
        
        Se puede utilizar debido a que la ecuación de Laplace tiene un solución única para esas condiciones de contorno, por lo que resolver un problema distinto con mismas condiciones de borde lleva al mismo resultado.
        
    - March 26, 2021 1:07 PM **Ecuaciones de la electrodinámica**
        
        
        ![../Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png](../Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png)
        
    - April 8, 2021 2:20 PM **Teorema de Poynting**
        
        El teorema de Ponyting es un teorema de conservación que relaciona la tasa a la cual se realiza trabajo para cambiar la energía mecánica de las partículas.
        $U_{EM}=\frac{1}{2}\epsilon_0 \int_V d^3 [\bold{E}\cdot \bold{E}+c^2 \bold{B}]$ 
        
    - April 8, 2021 8:11 PM **¿Cómo se interpreta el vector de Poyting?**
        
        Se interpreta como la densidad de energía por unidad de área por unidad de tiempo. Como una corriente de densidad de energía. 
        
    - March 13, 2021 4:49 PM **Cómo es el comportamiento de las cantidades electromagnéticas bajo operaciones discreta de inversión temporal y espacial?**
        
        La densidad de carga $\rho$ es invariante bajo inversiones espaciales y temporales. 
        
        La densidad de corriente $\bold{j}\to \bold{-j}$ para inversiones temporales y espaciales.
        
        La fuerza de Lorentz $\bold{F}\to-\bold{F}$ para inversiones espaciales y es invariante para inversiones temporales, por consiguiente el campo eléctrico también se comporta igual.
        
        El campo magnético es invariante para inversiones espaciales, pero $\bold{B}\to\bold{-B}$ para inversiones temporales.
        
        El potencial electrico es invariante bajo ambas inversiones
        
        El potencial vectorial $\bold{A}\to-\bold{A}$ para ambas inversiones.
        
    - April 9, 2021 12:42 PM **¿Que es una simetría dual?**
        
        Una simetría dual es dada por la invarianza de la fuente de carga libre $\rho=\bold{j}=0$, tal que si $\bold{E}\to c\bold{B}$ ambas son soluciones de las ecuaciones de Maxwell.
        
    
    - April 8, 2021 2:04 PM **¿Cuáles son las condiciones de borde para campos eléctricos en la materia**?
        
        
    - **¿Siempre se conserva la carga?**
        
        Sabemos que la carga siempre se conserva en un proceso físico. La única forma de cambiar la carga neta en un volumen finito es moviendo las partículas cargadas dentro o fuera del volumen. 
        
        La ecuación de conservación de la carga tiene la forma de una  ecuación de conservación $\frac{\partial \rho}{\partial t}+\nabla \cdot \bold{j}=0$, donde $\rho$ es la densidad de carga y $\bold{j}$ es la densidad de corriente. Esta ecuación nos dice que la carga total en cualquier  volumen infinitesimal es constante al menos que exista un flujo neto de cargas pre-existentes  que pasa por dentro o fuera del volumen.
        
    - **¿Cuándo son las ondas electromagnéticas soluciones de las ecuaciones de Maxwell?**
        
        Cuando están en ausencia de fuentes.
        
    - **¿Cómo es la solución general de una ecuación de onda?**
        
        La solución general de una ecuación de onda es la suma de ondas viajando en distintas direcciones. $f(z,t)=g(z-vt)+h(z+vt$)
        
    - **Fuerzas magnéticas hacen trabajo?**
        
        Una fuerza magnética puede cambiar la dirección de $\bold{v}$ pero no su magnitud.
        
        mejorar
        
        ser conserva momentum?
        
    - **¿Qué pasa con el campo electromagnético cuando la densidad de carga y la densidad de corriente dependen del tiempo?**
        
        El campo electromagnético en un punto $P$ refleja el comportamiento de las fuentes en un tiempo anterior/retardado $t-r/c$, donde $\vec{r}$ es el vector desde un origen arbitrario $O$ hasta el punto $P$. Esto refiriendose a las fuentes. En las ecuaciones de Maxwell aparecen los términos variables en el tiempo
        
    - **¿Qué es la radiación electromagnética**?
        
        El campo electromagnético tiene una componente que transporta energía lejos de las fuentes al infinito, en un proceso que es irreversible. Esta componente es llamada radiación.
        
    - **¿Cómo transforman los campos electromagnéticos?**
        
        Los campos $E$ y $B$ cambian cuando el sistema de referencia se mueve con velocidad $v$. Las transformaciones de Lorentz dan la relación entre las componentes tranversales y perpendiculares de los campos entre dos marcos de referencia.
        $\vec{E^{`}_{||}}=\vec{E_{||}}$ y $\vec{B^{`}_{||}}=\vec{B_{||}}$. Para la componente perpendicular $E^{'}_{\perp}=\gamma(\vec{E_{\perp}+\vec{v}\times \vec{B_\perp}})$ y $B^{'}_{\perp}=\gamma(\vec{B_{\perp}-\frac{\vec{v}\times \vec{E_\perp}}{c^2}})$.
        
    - **¿Qué hace el efecto Hall**?
        
        El efecto Hall, ocurre cuando un campo magnético externo hace que las cargas se acumulen en un extremo de un cable, generando un  campo electrico tranversal.
        
        estudiaaaaaar
        
    - **¿Qué pasa si lleno un capacitor con un dieléctrico?**
        
        Cuando un material dielectrico(aislante) se pone dentro de un capacitor, hace que se polarizen las moléculas en el dieléctrico y la capacitancia aumenta en un factor $\kappa$.Ya que cerca de las laminas del capacitor se crean capas de carga que cancelan las cargas libres "aumentando la capacidad de almacenar carga"
        
    - **¿Que es la expansión multipolar?**
        
        Cuando tenemos una distribución de cargas, esta puede ser escrita como expansión en serie aumentando de $1/r$. Los coeficientes de esos términos se conocen como momentos. Una carga tiene un momento monopolar. Dos cargas opuestan crean un dipolo. Sobre un dipolo se puede generar torque el cual es proporcional al momento y al campo eléctrico
        
    - Cómo cambia la capacitancia en un marco de referencia móvil
    - **¿Qué le ocurre a un material dieléctrico al entrar en contacto con un campo externo**?
        
        Los electrones de los átomos individuales salen de su posición de equilibrio por una mínima cantidad, pero no se despegan de sus átomos, debido a esto se crea un campo eléctrico dentro del material. Este proceso se llama polarización
        
    - **Por qué la carga en un conductor reside en su superficie, por qué un conductor hueco es un escudo para campos exteriores, pero no para cargas dentro?**
        
        La carga en un conductor reside en la superficie debido a que para cualquier superficie cerrada que se haga sobre la superficie dentro del conductor el campo debe ser cero, si uno hace una superficie infinitesimal en la superficie  y el exterior esta por ley de Gauss la carga encerrada que generará el campo estará en las últimas capas del conductor.
        
    - **¿Cómo es la fuerza entre las placas conductoras de un capacitor plano?**
        
        Como el campo es constante, basta con multiplicar  por el valor de la carga total del otro plano. 
        
    - **¿Explique el método de imágenes y por qué se puede utilizar?**
        
        El método de imagenes consiste en poder resolver un problema que incluye la interacción de una distribución de cargas y un conductor. El conductor se puede reemplazar por una configuración de cargas imaginarias que satifagan las condiciones a la que está en conductor. Por ejemplo, potencial constante, potencial cero, etc.
        
        Se puede utilizar debido a que la ecuación de Laplace tiene un solución única para esas condiciones de contorno, por lo que resolver un problema distinto con mismas condiciones de borde lleva al mismo resultado.
        
    - **Ecuaciones de la electrodinámica**
        
        
        ![../Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png](../Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png)
        
    - **Teorema de Poynting**
        
        El teorema de Ponyting es un teorema de conservación que relaciona la tasa a la cual se realiza trabajo para cambiar la energía mecánica de las partículas.
        $U_{EM}=\frac{1}{2}\epsilon_0 \int_V d^3 [\bold{E}\cdot \bold{E}+c^2 \bold{B}]$ 
        
    - **¿Cómo se interpreta el vector de Poyting?**
        
        Se interpreta como la densidad de energía por unidad de área por unidad de tiempo. Como una corriente de densidad de energía. 
        
    - 
    - **¿Cuáles son las condiciones de borde para campos eléctricos en la materia**?
        
        
    - 
    
    [Copy of Formulario](E%20l%20e%20c%20t%20r%20o%20d75ce3aa2d4f48a68221fbb40cf28974/Copy%20of%20Formulario%202b4d60d464804e35abc8292f13835221.md)
    
- $\colorbox{aquamarine}{Aplicación}$
    
    
    - $\colorbox{aquamarine}{Expansión  multipolar}$
        
        
        03/11/2021 12:45 
        
        - Ex 4.1 Jackson. Calcular momentos dipolares de distintas distribuciones puntuales en el plano $x,y,z$.
            
            
            - Dibujo.
                
                
                ![../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled%201.png](../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled%201.png)
                
            1. Como queremos información del potencial lejos de la fuente. Podemos usar la solución de la ecuación de Laplace  en coordenadas esféricas con simetría azimutual para encontrar los distintos momentos.
                1. El potencial es de la forma.$\varphi(r,\phi,\theta)=\sum\limits^{\infty}_{l=0}\sum\limits^{m=-l}_{l}(A_{lm}r^l+B_{lm}r^{-l-1})Y_{l,m}(\theta,\phi)$. Donde
                son los armónicos esféricos. 
                2. Pero queremos que la solución se aproxime a cero en infinito $A_{l}=0$
                3. Y podemos usar $q_{l,m}=\int Y^{*}_{l,m}(\theta,\phi)r^{´l} \rho(\bold{r'})d\bold{r}$  para calcular los momentos multipolares esféricos.
                4. Cada carga vive en el plano $x,y$, por lo que $\theta=\pi/2$ y $\phi = 0,\pi/2,-\pi/2,  3\pi/2$.
                5. Calculamos $Y_{l,m}$ con sus polinomios de legendre asociados y encontramos el valor para distintos $l,m$ si se tiene suerte se puede encontrar una relación de recursión.
                    - Dibujo 2.
                        
                        
                        ![../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled%202.png](../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/E%20l%20e%20c%20t%20r%20o%205c64d285374147bd9e57cafd27575d60/Untitled%202.png)
                        
                    1. En este caso tenemos todas las cargas en el eje $z$. 
                    2. Repetir procedimiento para $\theta =0$ y $\phi =0$.
                    
                
                Luego nos quedamos con los primeros ordendes de la expansión y las agregamos al potencial.
                
        
    - $\colorbox{aquamarine}{Método de las imágenes (carga y esfera)}$
        
        March 19, 2021 5:36 PM 
        
        El método de las imágenes consiste en reemplazar el problema electroestático de la presencia de cargas y un conductor, también se puede extender a problemas de campos en la materias, siempre y cuando se pueda encontrar una ecuación de Laplace análoga, es decir, un sistema sin fuente y que satifaga $\nabla^2 \psi=0$, donde $\psi$ es el potencial de un campo. Si la simetría acompaña se puede reemplazar el conductor por una distribución de cargas que satisfaga las condiciones de frontera en el conductor y de esta forma reemplazar el problema a un problema de interacción entre cargas
        
        1. **Problema:** Carga a una distancia $d$ de una esfera conductora de radio $R$ que se encuentra conectada a tierra. Piden encontrar el potencial fuera de la esfera.
        
        Para resolver este problema, vemos que tenemos. La esfera es conductora, por lo que el campo eléctrico dentro de ella es cero y por consiguiente el potencial en su superficie es constate. Esto nos da una condición de borde para el potencial $\phi (R)$=constante. 
        
        Reemplazamos TODA la esfera por una carga $q'$ alineada con la carga $q$ externa y la colocamos a una distancia $d'$ del origen. Queremos conocer el potencial en un punto $P$ cualquiera fuera de la esfera, entonces lo que debemos resolver ahora es el potencial para dos cargas puntuales separadas por una distancia $d+d'$, la distancia $d'$ la podemos encontrar exigiendo que el potencial en $R$ sea cero/constante y despejamos $d$ de la ecuación para la suma de los potenciales. Esta posición será tal que cumpla esa condición, una vez encontrado ese valor, se puede encontrar la magnitud de la carga imagen. Por teorema de unicidad de las soluciones de la ecuación de Laplace, esta solución es equivalente al problema original.
        
        **PD**  el valor de $q' = \frac{-R q}{y}$ y el de la posición $d'=\frac{R^2}{y}$.
        
        También por el mismo teorema de unicidad de las soluciones, sabemos que la solución encontrada utilizando el método de imagenes será la solución de la ecuación de Poisson, ya que la solución es única, por lo que la función de Green es:
        
        $G(\bold{r,r'})=\frac{1}{|\bold{r}-\bold{r'}|}+F(\bold{r,r'})$
        
        $G_D(\bold{r,y})=\frac{1}{|\bold{r}-\bold{y}|}-\frac{a}{y|\frac{a^2}{y^2}\bold{y}-\bold{r}|}$, la cual satiface las condiciones de borde de Dirichlet. Donde $y$ es la distancia a la carga $r$ la posición donde medimos.
        
        Cuando la esfera metálica no está conectada a tierra, y tiene carga total $Q$, el problema se puede resolver usando susperposición del problema anterior $+$ una carga puntual que haga que el potencial de la esfera sea constante $\phi=q/4\pi r$, esta nueva carga se distribuye en la superficie de la esfera y llega a un estado de equilibrio, por lo que el potencial es la suma de los potenciales. 
        
    - $\colorbox{aquamarine}{Método de las imágenes (esfera en un campo eléctrico)}$
        
        March 22, 2021 11:27 PM 
        
        **Esfera conductora en un campo eléctrico**
        
        Tenemos una esfera conductora en un campo eléctrico $E\hat{z}$, por simetría conviene elegir $z$ como la coordenada donde apunta el campo. La presencia de la esfera conductora hará que las lineas de campo cambien en las cercanías,  'las repele", el campo eléctrico dentro necesariamente es cero debido a que es una esfera conductora. 
        
        **PD:** El potencial será $\phi = -E_0(r-\frac{R^3}{r^2})\cos{\theta}$, donde el término $-E_0 r$ viene del campo externo $\vec{E}=-\nabla \phi$.
        
        - $\texttt{Sol dos métodos:}$
            1. Método de imágenes: Usando el método de las imagenes, podemos pensar este problema como la interacción de dos cargas $\pm Q$, cargas opuestas generarán una componente neta del campo en este caso $z$ la cual debe reemplazar al campo externo. Ahora se exigen las condiciones de borde sobre la esfera, es decir, que el potencial sea constante en el radio y el campo cero dentro. **Ojo:** como las cargas deben estár muy lejos para que el efecto sea un campo constante, se usa la aproximación dipolar para $1/|\vec{r}-\vec{r'}|$.
            2. Como el principio de superposición se cumple para la ecuación de Laplace, potencial y campo eléctrico, podemos construir este problema como la suma de distintos problemas.
            3. El primero es el efecto de una carga cerca de una esfera conductora a potencial cero.
            4. Luego, el efecto de una carga sobre una esfera conductora a potencial fijo.
            5. Finalmente, el efecto de la presencia de dos cargas de distinto signo y una esfera a potencial fijo.
            
            Para el primer caso, tenemos que el potencial es:
            
            $\varphi=\frac{1}{4\pi\epsilon_0}(\frac{q'}{\bold{r^i}}+\frac{q}{\bold{r^q}})$, donde $\bold{r^i}$ es la distancia desde la carga imagen al punto donde queremos medir y $\bold{r^q}$ la distancia entre la carga original y el punto. $\bold{r}$ es la distancia del origen al punto de medición.
            
            Por teorema del coseno:
            
            $\varphi(\bold{r},\theta)=\frac{1}{4\pi\epsilon_0}\left(\frac{q'}{\sqrt{r^2+b^2+2rb\cos{\theta}}}+\frac{q}{\sqrt{r^2+a^2+2ra\cos{\theta}}}\right)$. Donde $a$ es la distancia del origen a la carga $q$ y $b$ a la carga imagen. Se debe cumplir que $\varphi(R,\theta)=0$.
            
            Por lo tanto, factorizando por $a$ y $b$.
            
            $\frac{q}{q'}=\left(\frac{a(R^2/a+a+2R\cos{\theta})}{b(R^2/b+b+2R\cos{\theta}}\right)^{1/2}$, debido a que $q$ no puede depender de $\theta$, pero si debe depender del radio $R$ de la esfera y la distancia de la carga, no puede darse el caso de $a=b$, por lo tanto para todo $\theta$, se cumple que, $b=\frac{R^2}{a}$, por  lo tanto $q'=-\frac{R}{a}q$.  A medida que la carga se acerca a la esfera, la carga imagen crece en magnitud y se aleja del centro de la esfera.
            
            Conociendo la posición de la carga imagen, para el problema de la esfera en el campo eléctrico, se pondrán dos cargas en la región interior de la esfera $\pm  b=\frac{R^2}{a}$.
            
            Por lo que el potencial será $\varphi=$Potencial cargas que generan el campo externo+ potencial de las cargas imágenes dentro de la región de la esfera. Para el caso de que la esfera se mantenga a potencial constante, se puede agregar una carga ficticia en el origen tal que el potencial sea constante en $R$.
            
            El campo eléctrico dentro de la esfera sigue siendo cero debido a que se genera una densidad de carga superficial sobre la superficie interior de la esfera que anula este campo.
            
            $\texttt{Polinomios de Legendre}$: 
            
            Para resolver este problema a través de los polinomios de Legendre. Tenemos que satifacer la condiciones de borde, las cuales son $\varphi_{\to \infty} = -E_0 r \cos{\theta}$. Y que el potencial en la superfice o es cero o es $\varphi(R)$. 
            
            $\varphi(\bold{r},\theta)= \sum\limits_{l=0}^{\infty} (A_l r^l +B^l r^{-l-1})P_{l}(\cos{\theta})$
            
            Para $\varphi(R=0,\theta)=0$, los coeficientes son:
            
            $A_l R^l=-\frac{B_l}{R^{l+1}}$, por lo tanto el potencial para todo $\bold{r}$ en términos de $A_l$ es:
            
            $\varphi(\bold{r}{,\theta})=\sum\limits_{l=0}^{\infty}(A_l r^l -A_l R^{2l+1}r^{-l-1})P_l(\cos{\theta})$.
            
            Para $\bold{r} \to \infty$
            
            $-E_0 r \cos{\theta} = \sum \limits_{l=0}A_l r^lP_l(\cos{\theta})$, usando ortogonalidad para determinar $A_l$
            
            $-E_0 r \int_0^\pi  P_{l'}(\cos{\theta})\cos{\theta}\sin{\theta}d\theta=\sum\limits_{l=0}A_l r^l\int_0^\pi P_l(\cos{\theta})P_{l'}(\cos{\theta})\sin{\theta}d\theta$, donde $P_1({\cos{\theta}})=\cos{\theta}$.
            
            $-E_0 r  \frac{1}{2+1}\delta_{l',1}*2 = 2/3.$Para cualquier $l'$ distinto de $l=1$ el potencial se hace cero.  Y $A_1=E_0$.
            
            Por lo tanto: 
            
            $\varphi(\bold{r},\theta) = -(E_0 r -\frac{E_0R^3}{r^2})P_1(\cos{\theta})=(E_0 r -\frac{E_0R^3}{r^2})\cos{\theta}$. Para $R \ll r$   recuperamos $\varphi \propto -E_0 r$.
            
        
    - $\colorbox{aquamarine}{Semiesferas conductoras a distintos potenciales}$
        
        
    - $\colorbox{aquamarine}{Geometría Cilíndrica}$
    - $\colorbox{aquamarine}{Geometría Cartesiana}$
    - $\colorbox{aquamarine}{Dipolo eléctrico sobre un plano conductor}$
        
        March 24, 2021 7:10 AM 
        
        Se tiene un dipolo eléctrico a una distancia $d$ de un plano conductor a tierra. El dipolo forma un ángulo $\theta$ con la horizontal. Encontrar una expresión para el torque que genera el plano sobre el dipolo.
        
        sol: Para este problema se puede usar el método de imágenes donde el potencial debe ser cero en $z=0$, la expresión para el potencial debe ser la de una expasión dipolar eléctrica .
        
        El dipolo eléctrico imagen estará antiparalelo al dipolo real. Para calcular el torque, debemos considerar solo el efecto del campo eléctrico producido por el dipolo imagen $\bold{\tau}=\bold{p}\times\bold{E'}$.
        
    - $\colorbox{aquamarine}{Ondas electromagnéticas}$
        - March 20, 2021 12:10 PM Jackson 7.4.  Onda electromagnética plana incidiendo perpendicularmente.  Calcular la fase y la amplitud de la onda reflejada respecto a la onda incidente para $\sigma$ y $\epsilon$ arbitrarios.
            1. Cuando se dice que la onda es una onda $\textit{plana polarizada}$ se refiere a que es una onda linealmente polarizada. Por lo que podemos tomar $k\hat{z}$ y sin perdida de generalidad escribir el campo $\vec{E}=E_0\hat{x}e^{i(kz+wt)}$
            2. El campo reflejado será $\vec{E^{''}}=-E^{''}_{0}\hat{x}e^{-i(kz+wt)}$.
            3. Con estas dos expresiones podemos calcular los coeficientes de transmisión y reflexión para encontrar una relación entre las Amplitudes.
            4. $\frac{E_0^{''}}{E_{0}}=\frac{\sqrt{\frac{\mu \epsilon '}{\mu '\epsilon}}-1}{\sqrt{\frac{\mu \epsilon '}{\mu '\epsilon}}+1} \to \frac{n'-n}{n'+n}$ donde el resultado de la derecha es para $\mu'=\mu$
            5. Recordar que para incidencia normal la onda reflejada es paralela al plano de incidencia por lo que si $n' > n$ ocurre un reverso de fase para la onda reflejada.
            6. El indice de refracción es $n_i = \sqrt{\frac{\epsilon_i \mu_i}{\epsilon_0 \mu_0}}$, asumiendo que el medio no es permeable $i=1,2$.
            7. $\epsilon_2 = \epsilon +\frac{i \sigma}{\omega}$. Reemplazar y despejar.
        - March 13, 2021 1:23 PM Jackson 7.6  Una onda electromagnética de frecuencia $\omega$ incide normal desde el vacio sobre un bloque semi infinito de material con un indice de refracción complejo $n(\omega)$.
        Mostrar que $R=|\frac{1-n(\omega)}{1+n(\omega)}|^2$ y que $T=|\frac{4\real{n(\omega)}}{1+n(\omega)}|^2$, donde $n^2(\omega)=\epsilon(\omega)/\epsilon_0$.
            
            Como el indice de refracción es complejo, podemos usar las ecuaciones de Fresnel para campo con incidencia normal. 
            
            La relación entre el campo incidente (amplitudes) y el coeficiente de refracción complejo es: $\frac{E_0^{''}}{E_0}=\pm(\frac{n(\omega)-1}{n(\omega)+1})$. 
            
    - 
- **Problemas importantes revisar**
    - [x]  Jackson 1.1
    - [x]  Jackson 1.9
    - [x]  Jackson 2.3
    - [ ]  Jackson 2.5
    - [ ]  Jackson 2.7
    - [ ]  Jackson 2.9
    - [ ]  Jackson 2.11
    - [ ]  Jackson 2.16
    - [ ]  Jackson 2.26
    - [ ]  Jackson 3.1
    - [ ]  Jackson 3.3
    - [ ]  Jackson 3.5
    - [ ]  Jackson 4.2
    - [ ]  Jackson 4.8
    - [ ]  Jackson 4.9
    - [ ]  Jackson 4.10
    - [ ]  Jackson 5.6
    - [ ]  Jackson 5.8
    - [ ]  Jackson 5.14