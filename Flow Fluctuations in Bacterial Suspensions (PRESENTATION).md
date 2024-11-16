


```tikz
\usetikzlibrary{arrows.meta,backgrounds,positioning,shapes}
\usepackage{tikz}

\begin{document}
\begin{tikzpicture}[scale=1]
    % Style definitions
    \tikzset{
        box/.style={
            draw=none,
            fill=#1!10,
            rounded corners=3pt,
            minimum height=2cm,
            minimum width=2.8cm,
            text width=2.6cm,
            align=center,
            inner sep=8pt
        },
        conn/.style={
            -Stealth,
            thick,
            opacity=0.7
        }
    }
    

    % Main scale line
    \draw[thick] (0,0) -- (15,0);
    
    % Scale marks
    \foreach \x in {0,3,6,9,12,15} {
        \draw[thick] (\x,0.1) -- (\x,-0.1);
    }
    
    % Scale labels
    \foreach \x/\xtext/\unit in {
        0/1/\si{\nano\meter},
        3/1/\si{\micro\meter},
        6/100/\si{\micro\meter},
        9/1/\si{\milli\meter},
        12/1/\si{\centi\meter},
        15/1/\si{\meter}
    } {
        \node[below=3pt, font=\small] at (\x,-0.1) {\xtext~\unit};
    }
    
    % Example systems with boxes
    \node[box=blue] (motors) at (1.5,1) {
        \textbf{Molecular\\Motors}\\[3pt]
        \small ATP-driven\\proteins
    };
    
    \node[box=green] (bacteria) at (4.5,1) {
        \textbf{Bacteria}\\[3pt]
        \small E. coli\\B. subtilis
    };
    
    \node[box=green] (cells) at (7.5,1) {
        \textbf{Cellular\\Tissues}\\[3pt]
        \small Epithelial\\sheets
    };
    
    \node[box=orange] (insects) at (10.5,1) {
        \textbf{Swarming\\Insects}\\[3pt]
        \small Locusts\\ants
    };
    
    \node[box=orange] (birds) at (13.5,1) {
        \textbf{Bird\\Flocks}\\[3pt]
        \small Starlings\\pigeons
    };
    
    % Connectors
    \foreach \node in {motors,bacteria,cells,insects,birds} {
        \draw[conn] (\node) -- (\node |- {0,0});
    }
    
    % Log scale indicator
    \draw[|-|] (0,-1.2) -- (15,-1.2);
    \node[below, font=\small] at (7.5,-1.2) {Logarithmic scale};


\end{tikzpicture}
```
