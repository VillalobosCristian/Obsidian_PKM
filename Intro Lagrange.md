

  

1. Cuántos grados de libertad?

2. Cuántas coordenadas generalizadas?

3. Cuáles son las mejores coordenadas generalizadas?

4. Hay ligaduras?

5. Cantidades conservadas

6. Cuántos potenciales hay?

  

• ${\text{Leyes de Newton y sistema de partículas.}}$

• **Definición fuerza central.**

$$\vec{F}=0 \ \ \text{no implica} \ \ \vec{\tau}=0.$$

Que el torque sea cero, implica que la fuerza es paralela al vector $\mathbf{r}$, esta es la definición de fuerza central.

• **¿Qué es una fuerza conservativa?**

Una fuerza conservativa es una fuerza que depende solo de la posición $\mathbf{r}$ y no de la velocidad $\dot{\mathbf{r}}$. En estas fuerzas el trabajo es independiente del camino que se elige. De aquí deriva que la fuerza puede ser escrita como $\mathbf{F}=-\nabla V$. Cuando tenemos una fuerza conservativa, necesariamente tenemos una ley de conservación para la energía.

$$

T(t_2)-T(t_1)=-\int_{\mathbf{r}_1}^{\mathbf{r}_2} \nabla V \cdot d\mathbf{r} = -V(t_2)+V(t_1).

$$

Luego $T(t_1)+V(t_1)=T(t_2)+V(t_2) \equiv E$, es una constante de movimiento.

• Las fuerzas actúan sobre el centro de masa. Despreciando el roce con el aire, dos cuerpos de igual masa seguirán el mismo camino si se les aplica la misma fuerza.

• **¿Qué es una variable dinámica?**

Las variables dinámicas son cualquier conjunto de variables que pueden describir completamente la configuración de un sistema mecánico, es decir, la posición de sus partes y pueden cambiar bajo la acción de fuerzas.

• **¿Cuántos grados de libertad tiene una masa puntual?**

Una masa puntual tiene 3 grados de libertad, usualmente se usan ángulos o posiciones.

• El número de grados de libertad $N$ de un sistema es una propiedad intrínseca del sistema. Pero la elección de las variables dinámicas depende de uno, mientras el número de coordenadas independientes sea $N$.

• **¿Qué hace un Constraint/ligadura?**

Una ligadura reduce el número de grados de libertad.

Ejemplo: Una caja sobre una mesa tiene 3 grados de libertad: dos de traslación y uno de rotación sobre el eje perpendicular a la mesa.

• **¿Cuántos grados de libertad tiene una colección de $M$ masas puntuales?**

Podemos pensar este sistema como un sistema dinámico con $3M$ grados de libertad. Si hay $j$ ligaduras independientes, el sistema tiene solo $N=3M-j$ grados de libertad.

• **¿Depende el número de grados de libertad del cuadro de referencia?**

¡Sí! Un cuerpo que rota, por ejemplo, sus variables dinámicas dependerán de la elección del origen.

• **¿Qué son las ligaduras holonómicas?**

Las ligaduras holonómicas son aquellas ligaduras que se rigen por la siguiente ecuación:

$$

\vec{r}_i = \vec{r}_i(q_1, \dots, q_k, \dots, q_N, t)

$$

o $\vec{r}_i = \vec{r}_i(q_1, \dots, q_k, \dots, q_N)$

• **¿Qué son las ligaduras escleronómicas?**

Son aquellas donde las variables dinámicas cambian en el tiempo, pero las ligaduras son independientes del tiempo.

• **¿Qué son las ligaduras reonómicas?**

Cuando las ligaduras dependen explícitamente del tiempo. Por ejemplo, una cuenta deslizando sobre un alambre rotando.

• **¿Cuántas ecuaciones de Euler-Lagrange debemos resolver para un problema?**

Se deben resolver $N$ ecuaciones de Euler-Lagrange, que es igual al número de grados de libertad del sistema.

• **¿Se puede usar un marco de referencia no inercial en el Lagrangiano?**

No se puede, se deben escribir las variables de tal forma que queden de forma no inercial.

• **¿Cuándo un sistema conserva la energía?**

Decimos que un sistema conserva la energía si la energía total del sistema es constante $E = T + V = C$.

• **¿Cuándo el Hamiltoniano es conservado?**

El Hamiltoniano $H$ es conservado si el tiempo no aparece explícitamente en el Lagrangiano. Se cumple que $\frac{dH}{dt} = -\frac{\partial L}{\partial t}$.

• **¿Qué es una coordenada cíclica?**

Una coordenada cíclica es una coordenada que no aparece explícitamente en el Lagrangiano y solo aparecen sus derivadas temporales. Por lo tanto, se cumple que $\frac{d}{dt}\left( \frac{\partial L}{\partial \dot{q}} \right) = 0$

• **¿Dónde viven las soluciones de las ecuaciones de Newton?**

Las soluciones viven en el espacio de fases $[q, \dot{q}]$.

• **¿Qué es un sistema integrable?**

Un sistema integrable son aquellos sistemas que tenemos soluciones explícitas con forma integral.

• Cuando el sistema presenta $C$ ligaduras que cumplen con la ecuación $\sum_{\alpha}^n C_{\mu,\alpha} dq_{\alpha} + C_{\mu,t} dt = 0$, ¿cómo se escriben las ecuaciones de Euler-Lagrange?

Las ecuaciones de Euler-Lagrange quedan de la forma:

$$

\frac{d}{dt}\left( \frac{\partial T}{\partial \dot{q}_{\alpha}} \right) - \frac{\partial L}{\partial q_{\alpha}} = \phi_{\alpha} + \sum_{\mu}^c \lambda_{\mu} C_{\mu,\alpha}

$$

donde $\lambda_{\mu}$ son multiplicadores de Lagrange. Si el sistema es conservativo entonces las ecuaciones de Euler-Lagrange se escriben como:

$$

\frac{d}{dt}\left( \frac{\partial T}{\partial \dot{q}_{\alpha}} \right) - \frac{\partial L}{\partial q_{\alpha}} = \sum_{\mu}^c \lambda_{\mu} C_{\mu,\alpha}

$$

• **¿Qué son los multiplicadores de Lagrange?**

Los multiplicadores de Lagrange están asociados con las fuerzas de ligadura actuando en el sistema. Cuando se determinan los multiplicadores de Lagrange, el efecto de las fuerzas de ligadura es esencialmente tomado en cuenta sin necesidad de calcularlos explícitamente.

• **¿Las ecuaciones de Lagrange dependen de las coordenadas?**

No, las ecuaciones de Lagrange funcionan en todo sistema de coordenadas. Esto deriva del principio de mínima acción el cual trata de caminos y no de coordenadas.

• **¿Qué son los grados de libertad?**

Las coordenadas independientes que necesito para describir el sistema.

• **¿Los resortes son ligaduras?**

No, los resortes son interacciones.

  

**¿Cuántas transformaciones linealmente independientes existen para un marco de referencia inercial $S$?**

  

10 transformaciones: 3 rotaciones, 3 traslaciones, 3 boost y una traslación temporal.

  

$$

\vec{r}’ = O\vec{r} \

\vec{r}’ = \vec{r} + \vec{c} \

\vec{r}’ = \vec{r} + \vec{u}t \

t’ = t + c

$$

• ${\text{Fuerzas centrales}}$

Una fuerza central es una fuerza tal que esta solo dependa del vector posición $\mathbf{r}$. El problema de dos cuerpos se puede simplificar utilizando como coordenadas el centro de masa de dos objetos y la masa reducida como masa. Esto reduce el problema, donde al ser un movimiento en un plano conviene utilizar coordenadas polares para describir el problema. El momento angular es una cantidad conservada de movimiento y se define el potencial efectivo, como un potencial que depende de $r$ y una contribución centrífuga debido al movimiento rotacional.

1. El lagrangiano de dos masas interactuando con un potencial central es:

$$

L = \frac{m_1}{2} \dot{\mathbf{r}}_1^2 + \frac{m_2}{2} \dot{\mathbf{r}}_2^2 - U(|\mathbf{r}_1 - \mathbf{r}_2|)

$$

2. El truco está en elegir la coordenada relativa $\mathbf{r}$ como una elección de coordenada astuta para escribir el problema en un Lagrangiano más fácil.

3. Se define $\mathbf{R}$ como la coordenada del centro de masa. La distancia del origen al centro de masa del problema.

4. Reemplazando en las coordenadas en $T$ se llega a $T = \frac{1}{2} M \dot{\mathbf{R}}^2 + \frac{1}{2} \mu \dot{\mathbf{r}}^2$. Este notable resultado dice que la energía cinética del sistema es la misma que la de otro sistema, uno con dos partículas “ficticias”, una de masa $M$ moviéndose con la velocidad del CM, y otra de masa reducida, moviéndose con la velocidad relativa.

5. Por lo tanto $L = L_{\text{CM}} + L_{\text{rel}}$

6. El momento total es constante para el centro de masa y por lo tanto podemos elegir un sistema donde $\mathbf{R}$ esté en reposo.

7. En coordenadas polares y en el sistema en reposo en el CM, el potencial efectivo es

$$

U_{\text{eff}} = U + U_{\text{cf}} = U(r) + \frac{l^2}{2\mu r^2}

$$
