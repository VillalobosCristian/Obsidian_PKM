







```tikz
\begin{document}
\begin{tikzpicture}[scale=1]

    % Colors and styles

    \definecolor{perpcolor}{RGB}{0,153,76}       % Green for perpendicular

    \definecolor{parallelcolor}{RGB}{204,0,0}    % Red for parallel

    \definecolor{parallelcolor2}{RGB}{1,1,1}    % Red for parallel

  

    \tikzset{

        arrowstyle/.style={-stealth, thick},

        point/.style={circle, draw=blue, thick, inner sep=1.5pt, fill=white},

        connection/.style={dashed, gray, thin}

    }

  

    % Title for perpendicular correlation with proper math spacing

    \node[parallelcolor2, align=left] at (0,5) 

        {\Large $C_\perp(r)$: correlation perpendicular to separation $\bigl\langle u_i^\perp u_j^\perp \bigr\rangle$};

  

    % Negative correlation case

    \begin{scope}[xshift=-4cm, yshift=2.5cm]

        \node[point] (i1) at (0,0) {};

        \node[point] (j1) at (3,0) {};

        \draw[connection] (i1) -- (j1);

        \draw[arrowstyle, perpcolor, thick] (i1) -- ++(0,1.2) node[above] {$u_i^\perp$};

        \draw[arrowstyle, perpcolor, thick] (j1) -- ++(0,-1.2) node[below] {$u_j^\perp$};

        \node[align=center] at (1.5,-1) {$C_\perp < 0$ \\ anti-aligned};

    \end{scope}

  

    % Positive correlation case

    \begin{scope}[xshift=4cm, yshift=2.5cm]

        \node[point] (i2) at (0,0) {};

        \node[point] (j2) at (3,0) {};

        \draw[connection] (i2) -- (j2);

        \draw[arrowstyle, perpcolor, thick] (i2) -- ++(0,1.2) node[above] {$u_i^\perp$};

        \draw[arrowstyle, perpcolor, thick] (j2) -- ++(0,1.2) node[above] {$u_j^\perp$};

        \node[align=center] at (1.5,-1) {$C_\perp > 0$ \\ aligned};

    \end{scope}

  

    % Title for parallel correlation with proper math spacing

    \node[parallelcolor2, align=left] at (0,0) 

        {\Large $C_\|(r)$: correlation along separation $\bigl\langle u_i^\| u_j^\| \bigr\rangle$};

  

    % Strong correlation case

    \begin{scope}[xshift=-4cm, yshift=-2.5cm]

        \node[point] (i3) at (0,0) {};

        \node[point] (j3) at (3,0) {};

        \draw[connection] (i3) -- (j3);

        \draw[arrowstyle, parallelcolor, thick] (i3) -- ++(1.5,0) node[above] {$u_i^\|$};

        \draw[arrowstyle, parallelcolor, thick] (j3) -- ++(1.5,0) node[above] {$u_j^\|$};

        \node[align=center] at (1.5,-1) {$C_\| \approx 1$ \\ strong correlation};

    \end{scope}

  

    % Weak correlation case

    \begin{scope}[xshift=4cm, yshift=-2.5cm]

        \node[point] (i4) at (0,0) {};

        \node[point] (j4) at (3,0) {};

        \draw[connection] (i4) -- (j4);

        \draw[arrowstyle, parallelcolor, thick, opacity=0.7] (i4) -- ++(1.2,0) node[above] {$u_i^\|$};

        \draw[arrowstyle, parallelcolor, thick, opacity=0.7] (j4) -- ++(0.3,0) node[above] {$u_j^\|$};

        \node[align=center] at (1.5,-1) {$C_\| \approx 0$ \\ weak correlation};

    \end{scope}

  

\end{tikzpicture}
\end{document}
```
