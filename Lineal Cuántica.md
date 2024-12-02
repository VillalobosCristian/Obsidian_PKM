# Matemática

1st Rep: No
2nd Rep: No
3rd Rep: No
Subject: Mecánica cuántica

- $\colorbox{thistle}{Notación.}$
    
    En cuántica en vez de trabajar/pensar en un espacio de fases de las variables conjugadas, los objetos viven en un espacio vectorial lineal V con objetos $|1 \rangle,...,| v \rangle,|w\rangle$. Estos son los vectores y cumplen con las reglas de la suma, multiplicación por escalar y inverso aditivo.
    
    Un conjunto de vectores es linealmente independiente si cumple con:
    
    $\sum a_i|i\rangle = 0$, (donde si no se escriben los indices en la suma se asumirá que son los que aparecen). Dos vectores paralelos son ejemplo de dos vectores linealmente independientes.
    
    Podemos escribir cualquier vector $|v\rangle$ como una combinación lineal de $n$ vectores independientes llamados base.
    
    $|v\rangle = \sum v_i|i\rangle$.
    
    El producto interno se define como $\langle \text{bra}|\text{ket} \rangle = \sum_i \sum_j v_i^*w_j \langle i |j \rangle$.
    
    Para cada ket existe un bra en otro espacio vactorial "dual", con un bra asociado para cada ket y están relacionados por su relación adjunta.
    
    En una base normal in vector se puede expandir como:
    
    $\langle j | v \rangle  = \sum_i v_i \langle j | i \rangle = \sum_i v_i \delta_{i,j}=v_j$.
    
    Para encontrar una base ortonormal debemos:
    
    1. Convertir a vector unitario, esto entrega el primer vector base.
    2. Restar del segundo su proyección sobre el primero, dejando solo la parte perpendicular al primero.
    3. Rescalar lo que queda para que sea unitario y así para cada vector.
    
    Ej: $|2'\rangle = |II\rangle - |1\rangle \langle 1|II\rangle$, donde $|1\rangle = |I\rangle/|I|$.
    
    $\texttt{Problema de autovalores}$:
    
    Para un sistema físicom se define el observable como el operador (matriz) asociado a la cantidad física que se quiere medir o al aparato, etc. El observable al representar una cantidad física real, debe entregar autovalores reales. Se define como operador Hermitíco/Hermitanio el operador que cumple con $\hat{A}^{\dagger}=\hat{A}$.
    
    El problema de autovalores: $\Omega|v\rangle = \omega|v\rangle$. Donde $\Omega$ es el operador, $\omega$ es el autovalor y $|v\rangle$ es el autovector asociado a $\Omega$.
    
    Conociendo la representación matricial del operador, debemos resolver $\det(\Omega-I\omega)=0$.
    
    El problema de encontrar una base ortogonal es equivalente a resolver el problema de autovalores.
    
    Cuando dos operadores hermiticos conmutan existe una base común de autovectores que diagonaliza a ambos operadores.
    
    Por ejemplo, los modos normales de un sistema masa resorte, al desacoplar las ecuaciones de movimiento estamos encontrando los vectores base que diagonalizan.
    
     
    
    $\langle \text{bra}|\text{ket} \rangle$ =