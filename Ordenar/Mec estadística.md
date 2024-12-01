# Mec.estadística

- $\colorbox{Lavender}{Formulario}$
    
     
    
    - 10/03/2021 12:00 AM $\texttt{\text{Numéro de microestados}.}$
        
        $\Omega(E,N,V)=\frac{1}{h^{3N}}\int_{E\leq H\leq E+\delta E} d^{3N}q d^{3N}p$. Este es el número de microestados con energía entre $E$ y $E+\delta E$. Donde $h=\Delta p \Delta q$ tiene dimensiones de acción y aparece por la reticulación del espacio de fases de las variables canónicas el cual es continuo.
        
    - March 31, 2021 $\texttt{\text{Probabilidad de los micro estados}.}$
        
        $p_i=\frac{e^{-B \epsilon_r}}{\sum_r e^{-\beta \epsilon_r}}$. La probabilidad de que un sistema esté en un microestado con energía $\epsilon_r$. Cuando se quiere encontrar la probabilidad de cierta cantidad física, se multiplica por esa variable.
        
    - $\texttt{\text{Función de partición canónica.}}$
        
        March 21, 2021 9:00 AM 
        
        La función de partición es la constante de normalización de la probabilidad de encontrar el sistema en cierto estado de energía $E$.
        
        $Z = \sum_r e^{-\beta \epsilon_r}$, para sistemas con energía discreta.
        
        $Z  = \frac{1}{h^{3N}}\int d^{3N}q d^{3N}p \ e^{-\beta H}$.
        
    - $\texttt{\text{Energía de libre de Helmholtz}.}$
        
        April 3, 2021 9:15 PM 
        
        De termodinámica se sabe que $F(T,V,N)=U-TS$
        
        $F=-kT \ln Z(T,V,N)$. Mide el trabajo obtenible en un sistema a temperatura constante.
        
    - $\texttt{\text{Potenciales térmodinámicos}.}$
        
        $\frac{P}{T}=(\frac{\partial S}{\partial V})_{E,N}$. 
        
        $-\frac{\mu}{T}=(\frac{\partial S}{\partial N})_{E,V}$
        
        $-P=(\frac{\partial E}{\partial V})_{S,N}$
        
        $\mu=(\frac{\partial E}{\partial N})_{S,V}$
        
        April 2, 2021 3:40 PM 
        
        @remind 04
        
    - $\texttt{\text{Fluctuaciones}.}$
        
        April 6, 2021 9:23 PM 
        
        El valor medio de la energía $E$ es:
        
        $\langle E \rangle = \sum_{E_r} E_r P(E_r)$=
        
        $\langle E \rangle =\frac{1}{Z}\sum E_r \Omega(E_r)e^{-\beta E_r}=-(\frac{\partial}{\partial \beta}\ln Z)_{N,V}$.
        
        $(\Delta E)^2=k_B T^2 C_v$.
        
    - $\texttt{\text{Numéro medio de partículas F-D}.}$
        
        March 12, 2021 4:34 PM 
        
        $\langle n_j \rangle = \frac{1}{e^{\beta(\epsilon_j -\mu)}+1}$. Cuando $T$ y $\mu$ son dados, es decir, está en contacto con un reservorio térmico y de partículas, esta ecuación da el número medio de cada partícula individual en cada estado. 
        
    - $\texttt{\text{Energía total F-D}.}$
        
        April 7, 2021 3:23 PM 
        
        Si la energía total esla suma de las energías individuales, entonces la energía total será $E=\sum_j \epsilon_j \langle n_j \rangle$. 
        
    - $\texttt{\text{Numéro total de partículas F-D}.}$
        
        March 28, 2021 8:49 PM 
        
        El número total de partículas será $N=\sum_j \langle n_j \rangle$ y para cuando nos den $T$ y $N$ se puede utilizar esta ecuación para determinar el potencial químico del sistema como función de la temperatura. Luego se calcula la energía total y el número de ocupación medio.
        
        Cuando nos dan $E,N$ se usa la ecuación  de energía total y $N$ para encontrar el número de ocupación medio del sistema.
        
    - $\texttt{\text{Densidad de estados F-D}.}$
        
        @remind 03/11/2021 05:15 PM
        
        Cuando el volumen es suficientemente grande el número de estados con energía $\epsilon$ y $\epsilon + \delta \epsilon$ puede ser escrito como $g(\epsilon)\delta \epsilon$. 
        
        En términos de la energía y número total de partículas:$E = \int \epsilon f(\epsilon) g(\epsilon)d\epsilon$, $N=f(\epsilon)g(\epsilon)d\epsilon$, donde $f(\epsilon)$ es la distribución de Fermi-Dirac.
        
    - $\texttt{\text{Número medio de partículas B-E}.}$
    - $\texttt{\text{Energía partícula ultra relativista}.}$
    - $\texttt{\text{Densidad de estados}.}$
    - $\texttt{\text{Función Gamma }.}$
    - $\texttt{\text{Función zetta Riemman}.}$
    - $\texttt{\text{Función de Bose}.}$
    - $\texttt{\text{Función de partición Grand canónica.}.}$
    - $-\texttt{\text{Logaritmo función de partición Grand-Canónica}.}$
        
        $\ln{\mathscr{Z}}=-\int \ln(1-ze^{-\beta \epsilon})\frac{d^3q d^3p}{h^3}$. 
        
        March 17, 2021 4:34 PM 
        
    - $\texttt{\text{Temperatura en equilibrio}.}$
        
        La temperatura en equilibrio, asumiendo volumen constante y número de partículas constante se define tal que las variaciones de entropía de dos subsistemas respecto a sus energía son iguales. $\frac{1}{T}=(\frac{\partial S}{\partial E})_{V,N}$. El inverso de la temperatura es el costo de comprarle energía al universo.
        
- $\colorbox{aquamarine}{Aplicación}$
    - $\colorbox{aquamarine}{Polarización de un Gas ideal}$
        
        April 4, 2021 5:50 PM 
        
        En este problema piden calcular la polarización $\vec{P}$ de un gas ideal. Que tiene campo eléctrico dipolar constante $\bold{p}$, en un campo eléctrico homogéneo $\bold{E}$ a temperatura $\tau$. Calcular también la constante dieléctrica para campos pequeños. 
        
        Primero debemos conocer el Hamiltoniano de interacción. Este corresponde a la energía potencial del dipolo eléctrico $U=-\bold{p}\cdot\bold{E}$. Definiendo el eje z como eje de giro del dipolo, tenemos el hamiltoniano/función de partición de un rotor rígido. 
        
        El momento dipolar eléctrico total por unidad de volumen del gas es la polarización $\bold{P}$. La cual es la probabilidad de que  el dipolo esté apuntando en alguna dirección dentro del ángulo sólido $d\Omega$. Entonces debemos calcular el número medio $\langle p_z \rangle$. En coordenadas esféricas se introduce la variable $x=\cos{\theta}$ y se encuentra luego de resolver la integral que la polarización es proporcional a la función de Langevin.
        
        Para campos pequeños se expande la ecuación para $\bold{P}$ y se usa la definición del vector desplazamiento eléctrico para calcular la constante dieléctrica.
        
         
        
- $\colorbox{orange}{Interesantes}$
    - $\colorbox{orange}{Gases cuánticos en dimensión dos}$
        
        March 26, 2021 12:07 AM 
        
        Los gases ideales cuánticos son el sistema más simple que evidencia la naturaleza cuántica. Para bosones tenemos el $He^4$ y para fermiones los electrones libres en un metal.
        
        El valor medio del número de partículas en el sistema puede expresarse en el continuo como
        
        $\langle N \rangle = \sum_j \langle n_j \rangle = \int^{\infty}_{0} \frac{1}{z^{-1}e^{\beta \epsilon}+a}g(\epsilon)d\epsilon+\frac{z}{1+az}$, donde $a=-1$ es para bosones y $a=1$ para fermiones.
        
        El sumando extra que aparece hace referencia a la contribución del estado fundamental. El cual toma relevancia en dimensión 3.
        
        1. Como es usual cuando se trabaja con tratamiento cuántico, primero debemos encontrar la densidad de estados, en este caso, densidad de estado con energía ($\epsilon,\epsilon+d\epsilon)$.
        2. La energía $\epsilon = \frac{\hbar^2 k^2}{2m}$, de aquí se encuentra que $g(\epsilon)$ es constante para dos dimensiones.
        3. El gas de Bose-Einstein tiene solución exacta para dimensión 2.
            1. Para el gas de bosones calculamos $\langle N \rangle$ y despejamos $z$ y estudiamos su comportamientos límites.
            2. Para la energía quedamos con una función llamada dilogaritmo el cual tiene solución exacta.
            3. 4. Para el gas de Fermiones se hace el mismo procedimiento, donde se encuentra que a temperaturas bajas el potencial químico tiende a $\mu(0)$ el cual corresponde a la energía del nivel de fermi.
            4.  A temperaturas altas $\beta$ es pequeño y el comportamiento coincide con el gas clásico.
        
           
        
        1. En $T=0$ la distribución de Fermi-Dirac es una función escalon $\theta(\mu(0)-\epsilon)$, que vale 1 para energía por debajo de $\mu(0)$ y cero para energías mayores. A $T=0$ todos los estados por debajo la energía de fermi están ocupados y todos los estados por encima están desocupados. Para $T$ finitas el escalon se suaviza, para $T$ altas recuperamos el resultado clásico.
    - **Oscilador armónico 1-D, puede tener entropía negativa?**
        
        Primero, el hecho que exista entropía negativa para el caso clásico o cuántico  implicaría que existe menos de un estado accesible para alguna temperatura $T$.
        
        Como la entropía en el caso clásico está definida por un logaritmo, está definida positiva. Por lo que para $T\to 0$ diverge. Solo puede existir un oscilador armónico clásico si $k_B T>\hbar \omega$.
        
        Para el caso cuántico es lo mismo, salvo que $S>0$ para todo $T$.
        
- $\colorbox{thistle}{Importante/general}$
    
    
    - $\colorbox{thistle}{Función de distribución de Fermi}$
        
        April 6, 2021 9:23 PM 
        
        La función de distribución de fermi $f(\epsilon)=\frac{1}{e^{\beta(\epsilon-\mu)}+1}$. En el límite de $T \to 0$ esta función  parece una función escalon que se suaviza a medida que aumenta la temperatura. A $T=T_c=0$, Las partículas están en el nivel más bajo de energía y el número total de partículas está dado por $N=\int_{\epsilon_0}^{\mu_0}g(\epsilon)d\epsilon$, que es el área bajo la curva de $f(\epsilon)/\epsilon$. pd: La curva se suaviza en factores $kT$.
        
        - Gráfico distro-fermi.
            
            
            ![../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/Mec%20estadi%CC%81stica%20319cfa078b3745f2ac98707cca85870c/Untitled.png](../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/Mec%20estadi%CC%81stica%20319cfa078b3745f2ac98707cca85870c/Untitled.png)
            
            a $\epsilon_0=0$.
            
            ![../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/Mec%20estadi%CC%81stica%20319cfa078b3745f2ac98707cca85870c/Untitled%201.png](../Revisio%CC%81n%20problemas%20779e2f4a39154b849187090fd0bdbbf2/Mec%20estadi%CC%81stica%20319cfa078b3745f2ac98707cca85870c/Untitled%201.png)
            
        
        $\mu_0$ es el nivel de Fermi, (Fermi potential) a $T=0$. $E_0=\int_{\epsilon_0}^{\mu_0}\epsilon g(\epsilon)d\epsilon$ es la energía total del sistem a en el nivel más bajo de energía.
        
        A temperaturas altas $\mu$ es menor que $\epsilon_0$ y en este caso la distribución de Fermi se puede reemplazar por la de Maxwell-Boltzmann.
        
        En este caso la fugacidad puede tomar cualquier valor de cero a infinito. $\mu$ debe aumentar cada vez que se agrega una partícula al sistema a volumen fijo debido a que los fermiones cada vez ocupan un nivel energético más alto.
        
    - $\colorbox{Thistle}{Vibraciones en sólidos}$
        
        April 7, 2021 3:23 PM 
        
        Estudio de las contribuciones debidas a las vibraciones de los átomos en los sólidos cristalinos. El modelo consiste en un cristal perfecto en el cual los átomos se situan en los vértices de una red periódica e interactúan solamente con los primeros vecinos. En la aprox de sólido ideal el potencial es $\textbf{armónico}$.
        
        Se puede estudiar de dos puntos de vista con mismos resultados. 
        
        1. $\textbf{Osciladores armónicos distinguibles unidimensionales (modos normales)}$
        2. $\textbf{Gas ideal de Fonones}$.
        
        Los sólidos cristalínos siguen la ley de Dulong y Petit la cual dice que $C_{v }\approx 3Nk_B$ y que a muy bajas temperaturas $C_{v}\approx \alpha T^{d}$.
        
        $\colorbox{lightblue}{Coordenadas normales}$
        
        La interacción de las partículas en la red con sus primeros vecinos se puede escribir a través de un cambio de coordenadas a sus coordenadas normales, por lo que el hamiltoniano queda de la forma.
        
        $\mathscr{H({\bold{Q,P})}}= \sum^{3N}_{j=1}(\frac{P_j^2}{2} + \frac{w_j^2 Q_j^2}{2}).$ El cual corresponde a $3N$ osciladores armónicos unidimensionales desacoplados. 
        
        La energía de un modo normal de frecuencia $\omega_j$ es $\epsilon(\omega_j,n)=\hbar \omega_j (n+\frac{1}{2})$, $n=0,1,2,3,...$
        
        Luego podemos escribir la función de partición canónica y su expansión en serie geométrica. 
        
        Como los modos normales se distinguen por su frecuencia podemos escribir la función de partición como $Z(N,V,T)= \prod_{j=1}^{3N}{Z(\omega_j,T)}$.
        
        Calcular el $\ln{Z}$ y suponer que las frecuencias son tan cercanas que la suma se puede reemplazar por una integral. Se introduce la densidad de modos normales $g({\omega})d\omega$ que representa el número máximo de osciladores de frecuencia $\omega$ en el intervalo $(\omega, \omega+d\omega)$.
        
        $\colorbox{cadetblue}{Modelo de Einstein}$
        
        El modelo de Einstein aproxima a que todos los modos normales oscilan con la misma frecuencia $\omega_E$. Por lo que la densidad de frecuencias se puede representar por una delta.
        
        $\colorbox{Forestgreen}{Modelo de Debye}$
        
        En este modelo los modos normales son ondas elásticas continuas dentro del volumen V. Este modelo ignora por completo el carácter discreto de los sólidos.
        
    - $\colorbox{thistle}{Gas de fotones}$
        
        March 28, 2021 8:49 PM 
        
        Estudiaremos el comportamiento de la radiación electromagnética en función de la temperatura en equilibrio térmico.  Consideraremos la radiación como un gas de fotones a temperatura $T$.
        
        Los fotones son bosones de spin $S=1$, masa en reposo nula,y  por lo tanto la relación energía momento es ultrarelativista.
        
        1. Cuando el volumen de la cavidad es suficientemente grande se puede tomar $\bold{k}$ como continuo y calcular la densidad de estados con frecuencia $\omega$.
        2. La densidad de estados es $g(\omega)d\omega=\frac{V}{\pi^2 c^3}\omega^2 d\omega$.
        3. Para calcular la densidad de estados $g(\bold{k})d^3\bold{k} = g(s) \color{red}V(k) \int d^3\bold{k}$ donde $g(s)$ es la degeneración de spin y el término en rojo es el volumen por la cantidad de $k$ en el espacio $k$. 
        4. Haciendo los cambio de variables correspondientes al caso se puede escribir la densidad de estados con cierta frecuencia, energía, etc.
        5. Usando la distribución de bose para el número medio de ocupación de estados de energía $\epsilon=\hbar \omega$. 
        6. Como el potencial químico es cero debido a que los fotones no se conservan la fugacidad es $z=1$.
        7. Para longitudes de onda largas la densidad de estados $u\approx x^2$, con $x=\beta \omega \hbar$.
        8. Para longitudes de onda corta la densidad de estados $u \approx x^3 e^{-x}$.
        9. Existe un máximo para $u$ que corresponde   a frecuencias mayores, longitudes de onda corta.
        10. Integrando $\int^{\infty}_0u(\omega,T)d\omega$ , usando la función zeta de Riemann se encuentra la Ley de Stefan Boltzmann.
        11. $u(T) = \frac{\pi^2}{15}\frac{k_B^4}{c^3 \hbar^3}T^4$.
        12. Con la función de partición podemos calcular la ecuación de estado y la presión de radiación la cual es $p=\frac{1}{3}u(T)$. Es distinto a la de una partícula libre no  relativista, probablemente por  la degeneración y por la forma en que se escribe  la función de densidad de estados.
        13. La energía libre se obtiene directamente $F=N\mu-pV=-\frac{1}{3} V u(T)$.
        14. De la definición de $F$ se obtiene la entropía del gas de fotones y la capacidad calorifica.
        15. $\colorbox{lavender}{Hipótesis de Planck}$
        
        La hipótesis de Planck considera que cada modo normal tiene su energía discretizada en paquetes de $\hbar \omega$. Se usa la estadística de Maxwell-Boltzmann para un sistema clásico discreto.
    - $\colorbox{thistle}{Condesación de Bose-Einstein}$
        
        April 8, 2021 8:11 PM 
        
        La condensación de B-E es un fenómeno macroscópico, debido a la coherencia cuántica entre bosones. El hecho que a temperaturas bajas los bosones tiendan a ocupar el estado fundamental, produce su condensación en el espacio de  momentos. La velocidad de las partículas se reduce enormemente y a la vez se hace imposible localizarlas. 
        
    - $\colorbox{thistle}{Temperatura negativa en sistemas de dos niveles}$
        
        March 20, 2021 5:15 PM 
        
        En este tipo de sistemas, tenemos $N$ partículas capaces de estar en dos estados de energía $\pm \epsilon$. Se define  el número de partículas en el estado $+\epsilon$ como $N_{+}$ y el número de partículas en el estado $-\epsilon$ como $N_{-}$. Por lo tanto $N=N_{+}+N_{-}$ y la energía total del sistema es $E=N\sum_j \epsilon_j= (N_{+}-N_{-})\epsilon.$  Donde $\epsilon$ puede tomar los valores $\pm$.
        
        Luego se resuelve para $N_{\pm}$ y se calcula el número de microestados posibles del sistema a energía $E$ y  número de partículas $N$.
        
        En el ensamble microcanónico usamos la distribución binomial para calcular el número de microestados como todas las combinaciones de posibles configuraciones
        
        $\Omega(E,N)= \frac{N!}{N_{+}!N_{-}!}$, se puede leer como número de partículas repartidas en el estadoe $\pm \epsilon$.
        
        Con el número de microestados se calcula la entropía del sistema y posteriormente el inverso de la temperatura.
        
        En este problema mientras la energía sea $E<0$, es decir, hay más partículas en el nivel más bajo de energía $-\epsilon$, tenemos $T>0$. Si por algún método experimental las partículas se fuerzan a estar en un estado metaestable de energía alta $+\epsilon$ se pueden obtener temperaturas negativas. Se puede ver desde el gráfico $S$ vs $T$. 
        
        $\colorbox{lavender}{Cuando existe un límite superior de energía pueden mostrar temperaturas negativas.}$
        
        nota: A altas temperaturas, la energía media está acotada y resulta ser menor que el máximo de energía, es decir, todos los estados de máxima energía ocupados.
        
    - $\colorbox{thistle}{Gases con grados de libertad internos}$
        
        March 17, 2021 4:34 PM 
        
        Cuando consideramos un sistema de átomos más realista, debemos considerar sus grados de libertad internos. Ya sea rotación, vibración, electrónico, etc. Estos grados de libertad como sabemos pueden contribuir a la energía del sistema y por lo tanto a la temperatura. 
        
        El Hamiltoniano para este  sistema será: 
        
          $H=H_{\text{trans}}(\vec{R},\vec{P})+H_{\text{rot}}(\phi_i+p_{\phi_i})+H_{\text{vib}(q_j,p_j)}$. El primer término describe la traslación de las moléculas del gas. El segundo las rotaciones  correspondientes al momento angular y tercer término las vibraciones de las coordenadas normales.
        
        Para partículas no interactuantes sabemos que la función partición del sistema puede ser descrita por la multiplicación de las funciones partición partículares de las partículas.  También cada grado de libertad es independiente del otro y $Z(T,V,1)=Z_{\text{trans}}+Z_{\text{rot}}+Z_{\text{vib}}$. 
        
        Donde cada función de partición es:
        
        $Z_{trans}= \frac{1}{h^3}\int d^3R \int d^3P e^{-\beta H_{trans}}$
        
        $Z_{rot}= \frac{1}{h^3}\int d^3\phi \int d^3p_{\phi} e^{-\beta H_{rot}}$
        
        $Z_{vib}= \frac{1}{h^3}\int d^3R \int d^3P e^{-\beta H_{vib}}$.
        
        Para calcular las propiedades termodinámicas debemos conocer los Hamiltonianos respectivos para cada uno de los grados de libertad. 
        
        El hamiltoniano de traslación corresponde al de una partícula libre $H =\frac{P^2}{2m}$. 
        
        Para el grado de libertad rotacional podemos considerar la molecula como un rotor rígido cuyo lagrangiano es $L= \frac{I_1}{2}(\dot{\theta}^2+\dot{\phi}^2 \sin^2\theta)+\frac{I_3}{2}(\dot{\psi}+\dot{\phi}\cos \theta)^2$ Representado por los ángulos de Euler. Luego usando las ecuaciones de Hamilton, el Hamiltoniano del grado de libertad rotacional es. $H_{\text{rot}}=\frac{p^2_{\theta}}{2I_1}+\frac{p^2_{\psi}}{2I_3}+\frac{(p_{\phi}-p_{\psi} \cos\theta)^2}{2I1 \sin^2\theta}$. Al integrar, la integral de $p_{\phi}$ es una integral gaussiana con el origen  corrido, pero como las integrales gaussianas no dependen de la posición, tenemos el resultado típico de una integral gaussiana.
        
        El grado de libertad vibracional por su parte corresponde a un Hamiltoniano de un oscilador armónico $H_{\text{vib}}=\sum (\frac{p^2}{2m}+\frac{1}{2}m\omega^2 q^2)$.
        
        Nota: A temperaturas bajas, los grados de libertad vibracionales están congelados y la contribución a la energía interna viene únicamente de la energía del nivel fundamental del oscilador armónico cuántico.
        
    - $\colorbox{thistle}{Gas de electrones ultrarelativista}$
        
        March 26, 2021 1:07 PM 
        
        Encontrar la ecuación de un gas de electrones ultrarelativista.
        
- March 31, 2021 1:40 PM $\colorbox{aquamarine}{Primeras preguntas}$
    
    
    - March 10, 2021 12:23 AM **¿Qué es un microestado?**
        
        Un microestado es un estado de un sistema de muchas partículas donde todas las variablers microscópicas de interes están especificadas. Por ejemplo: La posición, momentum, etc. Experimentalmente es complicado acceder a los microestados debido a la cantidad de partículas de un sistema.
        
    - March 13, 2021 4:49 AM **¿Qué es un macroestado?**
        
        Es el estado termodinámico del sistema, el estado que observamos experimentalmente y definido por  variables macroscopicas.
        
    - April 9, 2021 12:42 AM**¿Qué cantidad es fundamental en los distintos ensambles?**
        
        En el ensamble microcanónico se mantiene la energía fíja, en este ensable es recalcable el calculo de entropía del sistema, siendo esta la variable utilizada para encontrar los parámetros termodinámicos. 
        
        En el ensamble canónico, el sistema está en contacto con otro sistema a temperatura $T$ y en equilibrio térmico. El número de partículas es constante, y la energía libre de Helmholtz es la variable más importante a encontrar.
        
        En el ensamble grand canónico, el sistema está en contacto con otro con el cual puede intercambiar partículas, por lo que $N$ no es constante y se busca determinar el potencial químico.
        
        Qué es un ensamble 
        
        Micro estado accesible
        
        Poner ecuaciones(las mencionó harto)
        
        Cuál conecta con la termodinámica 
        
    - April 8, 2021 2:04 PM **¿Qué es la función de partición?**
        
        
    - March 24, 2021 12:25 AM **¿Qué es el potencial Químico?**
        
        El potencial químico se puede entender como la energía media necesaria para agregar otra partícula al sistema.
        
    - March 12, 2021 4:22 PM **¿Cuál es el objetivo de la física estadística?**
        
        Determinar las propiedades termodinámicas de los sistemas macroscópicos a través de sus propiedades microscopicas. Siempre asumiremos que trabajamos con un número gigante de copias del sistema, cada una de ella en algún microestado del sistema. Las propiedades de macroscópicas de equilibrio serán entonces los promedios de sobre los microestados.
        
        - ¿Qué otros ensambles hay?
    - March 21, 2021 10:02 PM **¿Qué otros ensambles hay?**
        
        Colectividad isotermica-isobarica. se busca equilibrio mecánico. 
        
        Cuál es la cantidad fundamental 
        
    - April 7, 2021 5:15 PM **¿Cuál es el postulado fundamental del Ensamble microcanónico?**
        
        El postulado de igualdad a priori. El cual establece que todos los microestados compatibles con un macroestado del sistema tienen igual probabilidad.
        
    - April 3, 2021 3:25 PM **¿Cuál es la probabilidad de un determinado microestado?**
        
        $P_r = \frac{1}{\Omega}$
        
    - April 8, 2021 3:55 PM **¿Cómo son los microestados de dos sistemas en equilibrio entre sí y aislados del resto del universo?**
        
        El número de microestados para dos sistemas será máximo si están aislados e igual a $\Omega(E_1,V_1,N_1,E_2,V_2,N_2)$.
        
        Sumar o multiplicar 
        
    - March 31, 2021 9:49 PM **¿Cómo es el número de microestados de un sistema compuesto, $1+2$?**
        
        Para este sistema comopuesto se cumple $E=E_1+E_2$, $V=V_1+V_2$, $N=N_1+N_2$. Por lo que el número de microestado es $\Omega(E,V,N,E_1,V_1,N_1)=\Omega_1 \Omega_2$, debido a que los sistemas son independientes(por eso es la multiplicación)
        
    - April 1, 2021 9:42 PM **Para dos sistemas que se juntan, el equilibrio se alcanza cuando $\Omega$ es máximo.**
    - March 17, 2021 2:36 PM **¿Cuál es la condición de máximo?**
        
        $\frac{d\Omega}{dE_1}=0$, es decir, $\frac{1}{\Omega_1}(\frac{\partial \Omega_1}{\partial E_1})=\frac{1}{\Omega_2}(\frac{\partial \Omega_2}{\partial E_2})$
        
    - March 30, 2021 10:19 PM **¿Cómo evolucionan los sistemas?**
        
        Un sistema aislado evoluciona maximizando su entropía según la termodinámica y maximizando su número de microestados segun la física estadística.
        
    - March 29, 2021 2:50 PM **¿Cuáles son condiciones de equilibrio termodinámico?**
        
        $T_1=T_2$, $p_1=p_2$, $\mu_1=\mu_2$, se expresan mediante derivadas e igualadades de $S$ respecto a sus variables naturales
        
    - March 13, 2021 8:47 PM **¿La entropía es extensiva?**
        
        Sí, la entropía es extensiva $S=S_1+S_2$ de aquí deriva que $\Omega \propto E^{N\phi}$
        
        Por qué se puede sumar las propiedades extensivas 
        
    - March 11, 2021 10:14 PM **¿Qué es la entropía?**
        
        Desde la termodinámica se interpreta como una medida de desorden de un sistema. En concreto, de la falta de disponibilidad en el sistema de energía convertible en trabajo.
        
        Poner o interpretar ecuación 
        
    - March 24, 2021 10:42 PM **Cuándo la entropía es cero?**
        
        La entropía es cero cuando el numéro de microestados es 1, es decir, el estado es totalmente predecible.
        
    - March 19, 2021 5:35 PM **¿Qué es la paradoxa de Gibbs y cómo se corrige?**
    - March 27, 2021 7:31 PM **¿Qué variable se define para distinguir entra la estadística clásica y la estadística cuántica?**
        
        La longitud de onda de  De Broglie $\lambda =(\frac{h^2}{2\pi m k_bT})^{1/2}$ y la longitud de coherencia cuántica de las partículas que componen al sistema $l = (\frac{V}{N})^{1/3}$. A partir de estas dos longitudes podemos definir $\lambda/l \lll 1$ que nos conduce a $\lambda^3 n = (\frac{h^2}{2\pi m k_B T})^{3/2}$ con $n\lll 1$. Si esta condición no se cumple, se estudia el sistema en la estadísitica cuántica
        
        ### 
        
    - $\colorbox{lightblue}{Clasificación de los sistemas estadísticos}$
        - Sistemas estadísticos Cuánticos-Discretos.
        Estos sistemas se caracterizan por tener niveles de energía discreto, pero se debe tomar en cuenta la simetría de la función de onda para ver si las  partículas son bosones o fermiones y tratarlas con la estadística correspondiente.
        - Sistemas estadísticos cuánticos-continuos
        Se toma en cuenta la simetría de la función de onda, pero los niveles de energía están tan cercanos que se consideran continuos. Ej: Gas ideal cuántico
        - Sistemas estadísiticos clásicos-discretos.
        Cuando las partículas están muy separadas entre si se desprecian los efectos de la coherencia cuántica de las partículas y se utiliza estadística clásica para tratarlas.
        - Sistemas estadísticos Clásico-Continuos.
        El espectro de energía se considera continuo, por ejemplo, partículas libres, altas temperaturas en sólidos. 
        Para estos últimos dos casos se utiliza la estadística de Maxwell-Boltzman.
        - 
        
        ![../Mec%20Estadi%CC%81stica%20b9c87674f76b456b8f9eeb0a196aa463/Untitled.png](../Mec%20Estadi%CC%81stica%20b9c87674f76b456b8f9eeb0a196aa463/Untitled.png)
        
    - April 1, 2021 7:00 PM **Teorema de equipartición  de  la energía**
        
        El teorema de equipartición relaciona la energía  cinética de las partículas de un sistema con su temperatura.
        $E=\langle H \rangle  = N' \frac{k_B T}{\eta}$, donde $N'$ son los grados de libertad y $\eta$ la potencia del hamiltoniano.
        
        - $\textbf{Partículas libres}$:tienen un hamiltoniano $H= \sum p_i^2/2m$, tenemos $3N$ momentos y $\eta = 2$, luego $E=\frac{3}{2}k_B T$.
        - $\textbf{Oscilador armónico}$: $E = \frac{3}{2}k_B T + \frac{3}{2}k_B T = 3Nk_B T$.
    - March 16, 2021 10:02 PM $\colorbox{lavender}{Ensamble Macrocanónico- Grand canónico}$
        
        Este Ensamble ayuda a describir los sistemas donde $N$ no es constante, o la exigencia de que $N$ sea fijo hace que la suma en el ensamble canónico sea difícil de realizar, como en los sistemas cuánticos. Acá $E$ y $N$ son variables del sistema y se define como variable termodinámica de conección el potencial químico $\mu$. El sistema está en equilibrio químico y térmico con un resorvorio de partículas cuyo potencial químico es $\mu$. Por lo tanto el sistema está descrito por $\mu$, $V$, $T$.
        
        $\textbf{Fugacidad}$: Se define la fugacidad $z$ como $z = e^{\beta \mu}$, est
        
    - $\colorbox{lightgreen}{Mecánica estadística Cuántica}$
        
        Cuando las funciones de onda se comienzan a solapar, la coherencia cuántica debe tomarse en cuenta desde el comienzo del planteo del problema. También se pueden estudiar usando la estadística clásica algunos problemas tomando en consideración la cuantización de la energía. A pesar de ser efectos microscopicos, la coherencia cuántica tiene efectos incluso a temperatura ambiente (radiación de cuerpo negro, gas de electrones, etc).
        
        - $\textbf{Matriz de densidad}$: La matriz de densidad $\hat{\rho}$ es un  operador autoadjunto, que se puede interpretar como la densidad de  probabilidad en términos de la estadísitica. Debido a que es dificil conocer la función de onda de un sistema de $N$ partículas, se puede calcular su valor medio mediante $\langle \hat{A} \rangle = \sum_i \langle \phi_i |\hat{A}\hat{\rho}|\phi_i \rangle = Tr({\hat{A}\hat{\rho}})$. Para estados estacionarios la matriz de densidad es diagonal en la base donde el Hamiltoniano es diagonal, ya que al no ser una variable dinámica se cumple que $\hat{\rho}=f(\hat{H})$, $[\hat{H},\hat{\rho}]=0$
        - $\textbf{Colectividad microcanónica}$: Además del postulado de igual probabilidad a priori, se debe agregar otro postulado que asegure que los elementos no diagonales de la matriz de densidad se anulen. Esto es que las fases aleatorias tengan igual probabilidad. en cualquier base.
        - $\textbf{Colectividad canónica}$: En este caso la matriz de densidad  en la representación diagonal de energía viene dada por $\hat{\rho}= \frac{1}{Z}\sum_i e^{-\beta E_i}$.
        Y la función de partición viene descrita por $Z = Tr(e^{-\beta\hat{H}})$.
        - $\textbf{Colectividad macrocanónica}$: En este ensamble el hamiltoniano conmuta con el operador numero de partículas $\hat{N}$.
        
        Se define que $N$ partículas son indistinguibles si cuando no existe un observable que las distinga. Para todas las posibles configuraciones $N!$ de funciones de onda,  la densidad de probabilidad queda definida por la paridad de la función de onda.
        
        - $\textbf{Teorema de la conexión Spin-Estadísitca}$: Este teorema  nos dice cuándo la función de onda será simétrica o anti simétrica. Postula que si las partículas tienen spin entero, serán bosones y si tienen spin semi entero serán fermiones. Se utiliza la estadísitica respectiva para cada tipo de partículas. Donde los fermiones no pueden ocupar un mismo lugar energético debido al principio de exclusión de Pauli.
        
        $\textbf{Notación unificada para las tres estadísiticas}$:
        
        Podemos escribir las tres estadísticas utilizando el valor $a$ el cual toma valores $0,1,-1$ para la estadística de Maxwell-Boltzmann, Fermi-Dirac y Bose-Einstein respectivamente.
        
        $q = \ln{\mathscr{Q}}= \frac{1}{a}\sum_j{(1+az e^{-\beta \epsilon_j})}$. La estadística de M-B se obtiene tomando el límite de $q$.
        
    - **Paramagnetismo**
        
        Una sustancia es paramagnética si tiene imantación nula cuando no hay campo externo aplicado. Concentrandonos en el paramagnetismo de Langevin , las variables termodinámicas que describen el sistema son $M, T,H$, donde se busca la ecuación de estado la cual es la ley de Curie. En el caso cuántico se considera la cuantización de $E$ debido a que el momento magnético está cuantizado, pero al estar fijas las partículas se puede asumir sin perdida de generalidad que las funciones de onda no se solapan
        
    - **¿Qué es un cuerpo negro?**
        
        Un cuerpo negro consiste en una cavidad de volumen $V$ que contiene únicamente radiación electromagnética emitida  y absorbida por las paredes de la cavidad, y que se encuentra en eq termodinámico a  temperatura T.Por la cavidad se observa el flujo de radiación electromagnética.
        
- $\colorbox{aquamarine}{Segundas preguntas}$
    
    
    - April 6, 2021 9:35 PM **¿Qué es la energía de Fermi?**
        
        March 8, 2021 12:08 AM 
        
        La energía de Fermi es un valor límite del potencial químico a $T=0$. Donde todos los espacios de energía $\epsilon<\epsilon_f$ están ocupados.
        
    - April 8, 2021 3:45 PM **¿Cómo es la distrribución binomial?**
        
        $\binom{p}{q} = \frac{p!}{q!(p-q)!}$, es el número de formas de elergír un subset no ordenado de tamaño $q$ desde un set de tamaño $p$.
        
    - March 26, 2021 1:23 PM **¿Qué es una cantidad extensiva?**
        
        Una cantidad que escala linealmente con el tamaño del sistema.
        
    - March 12, 2021 10:14 PM **¿Qué es una cantidad intesiva?**
        
        Cantidades que se mantienen constantes cuando el sistema crece. $T$, $\mu$, $P$.
        
    - March 16, 2021 11:56 PM **¿La entropía es un máximo o un extremo?**
        
        La entropía al estar definida como un logaritmo, es un máximo en vez de un extremo.
        
    
- 

[Copy of  Formulario](Mec%20estadi%CC%81stica%2022ea3cb1d124482faf5c0a335c9b94a1/Copy%20of%20Formulario%203660670a50834cac883104520573e64c.md)