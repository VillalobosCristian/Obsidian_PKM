# Electrodinámica

Date Learned: February 13, 2021
1st Rep: No
2nd Rep: No
3rd Rep: No
Next Rep: February 14, 2021
Subject: Electrodinámica
Alarma: February 14, 2021 2:00 PM (GMT-3)

- **E c u a c i o n e s   d e   M a x w e l l**.
    
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
    
- **¿Por qué tengo libertad de elegir los potenciales electromagnéticos?**
    
    Esta invarianza en el cambio de escala de los potenciales es posible principalmente por la forma de las ecuaciones de maxwell y las propiedades vectoriales, pero las consecuencias ayudan a imponer condiciones sobre los potenciales tal que se puedan medir los campos físicos reales.
    
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
    
    
    ![Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png](Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Untitled.png)
    
- **Teorema de Poynting**
    
    El teorema de Ponyting es un teorema de conservación que relaciona la tasa a la cual se realiza trabajo para cambiar la energía mecánica de las partículas.
    $U_{EM}=\frac{1}{2}\epsilon_0 \int_V d^3 [\bold{E}\cdot \bold{E}+c^2 \bold{B}]$ 
    
- **¿Cómo se interpreta el vector de Poyting?**
    
    Se interpreta como la densidad de energía por unidad de área por unidad de tiempo. Como una corriente de densidad de energía. 
    
- 
- **¿Cuáles son las condiciones de borde para campos eléctricos en la materia**?
    
    
- 

[Formulario](Electrodina%CC%81mica%209f3ffcf6e857484cb26f297f291971ef/Formulario%204aa07f367ed44785b04fcd89b808f6c4.md)