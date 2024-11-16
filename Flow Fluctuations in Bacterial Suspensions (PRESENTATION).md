


```tikz
\usepackage{tikz}
\usepackage{amsmath}
\usetikzlibrary{decorations.markings,arrows.meta,backgrounds,calc,positioning,fit}

\begin{document}
\begin{tikzpicture}[
    scale=1.2,
    force/.style={-{Latex[length=3mm]}, thick, red},
    flow/.style={blue, ->, thick},
    label/.style={font=\small},
    box/.style={draw, rectangle, fill=white, align=left, inner sep=5pt}
    ]
    
    % Title with better spacing
    \node[font=\Large\bfseries, align=center] (title) at (0,6) 
        {Flow Fields in Low Reynolds Number Regime\\[0.2cm]
         \normalsize\normalfont (Stokes Flow: $\nabla p = \eta\nabla^2\mathbf{u}+\mathbf{f}$)};
    
    % Stokeslet Panel
    \begin{scope}[local bounding box=stokeslet]
        \node[font=\bfseries] at (-5,4) {(a) Stokeslet Solution};
        
        % Background grid
        \draw[help lines,gray!20] (-7,1) grid (-3,3);
        \draw[->] (-7,2) -- (-3,2) node[right] {$x$};
        \draw[->] (-5,1) -- (-5,3) node[above] {$y$};
        
        % Force point and streamlines
        \fill[red] (-5,2) circle (2pt);
        \draw[force] (-5,2) -- (-5,2.7);
        
        \foreach \y in {1.4,1.7,2,2.3,2.6} {
            \draw[flow] (-6.5,\y) .. controls (-5,\y+0.2) .. (-3.5,\y);
        }
        
        % Decay law
        \node[label] at (-3.5,3) {$\mathbf{u} \sim \frac{1}{r}$};
        
        % Mathematical expression
        \node[box] at (-5,0.2) {
            $\mathbf{u}(\mathbf{x}) = \frac{1}{8\pi\eta}\left(\frac{\mathbf{F}}{|\mathbf{x}|} + \frac{(\mathbf{F}\cdot\mathbf{x})\mathbf{x}}{|\mathbf{x}|^3}\right)$
        };
    \end{scope}
    
    % Force Dipole Panel
    \begin{scope}[local bounding box=dipole]
        \node[font=\bfseries] at (2,4) {(b) Force Dipole};
        
        % Background grid
        \draw[help lines,gray!20] (0,1) grid (4,3);
        \draw[->] (0,2) -- (4,2) node[right] {$x$};
        \draw[->] (2,1) -- (2,3) node[above] {$y$};
        
        % Forces
        \fill[red] (1.8,2) circle (2pt);
        \fill[red] (2.2,2) circle (2pt);
        \draw[force] (1.8,2) -- (1.8,1.5);
        \draw[force] (2.2,2) -- (2.2,2.5);
        
        % Streamlines
        \draw[flow] plot [smooth] coordinates {(0.5,2.7) (1.5,2.2) (2,2) (2.5,1.8) (3.5,1.3)};
        \draw[flow] plot [smooth] coordinates {(0.5,1.3) (1.5,1.8) (2,2) (2.5,2.2) (3.5,2.7)};
        
        % Decay law
        \node[label] at (3.5,3) {$\mathbf{u} \sim \frac{1}{r^2}$};
        
        % Mathematical expression
        \node[box] at (2,0.2) {
            $\mathbf{u}_d(\mathbf{r}) = \frac{P}{8\pi\eta r^2} \left[ 3 (\mathbf{e} \cdot \hat{\mathbf{r}})^2 - 1 \right] \hat{\mathbf{r}}$
        };
    \end{scope}
    
    % Combined Legend
    \node[box] (legend) at (0,-1.5) {
        \begin{tabular}{ll}
            \textcolor{red}{$\rightarrow$} Force & \textcolor{blue}{$\rightarrow$} Flow field streamlines\\
            $r$: Distance from source & $P$: Dipole strength\\
            $\eta$: Fluid viscosity & $\mathbf{e}$: Orientation vector
        \end{tabular}
    };
    
    % Key Points Box
    \node[box, right=1cm of legend] {
        \begin{tabular}{l}
            Key Properties:\\
            • Low Reynolds number: $\text{Re} \ll 1$\\
            • Time-independent\\
            • Linear superposition applies
        \end{tabular}
    };

\end{tikzpicture}
```