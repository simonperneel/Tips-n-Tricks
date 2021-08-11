# Tips & Tricks
Tips and tricks from my engineering studies that I wish I knew earlier. This is an online draft for myself and everyone who sees this 🙂
## Latex 
### useful packages
- package **`siunitx`** for typesetting values with correct units \
in options: `[per-mode=symbol]`: / instead of $^{-1}$ \
command: `\SI{12}{\meter}`
- package **`mhchem`** for chemical formulas  \
command: `\ce{CO2}`

- package **`pifonts`** for checkmarks \
command: `\checkmark` :heavy_check_mark:


### useful commands
Scaling image to the width of the paper: 
 ```
 \begin{figure}
        \centerline{\includegraphics[width=\paperwidth]{figure.pdf}}
 \end{figure}
 ```
 Two figures side-by-side:
  ```
\begin{figure}[H]
    \begin{subfigure}{0.5\columnwidth}
      \centering
      \includegraphics[width=\columnwidth]{img/xxx.pdf}
      \caption{comment}
      \label{fig:label}
    \end{subfigure}
    \begin{subfigure}{0.5\columnwidth}
      \centering
      \includegraphics[width=\columnwidth]{img/xxx.pdf}
      \caption{comment}
      \label{fig:label}
    \end{subfigure}
    \caption{comment}
    \label{fig:label}
  \end{figure}
```

## PCB design with Kicad
- Add 3D model to footprint:
1. Select component and press `E`
2. Select 3D settings tab
3. Add .step model of the component

- Use mounting holes for mounting the PCB: \
`MountingHole_4.3mm_M4_Pad_Via` footprint looks cool. Use this with rounded edges of the PCB: select `edge cut` layer, select `add graphic arc` in PCBNew, click the center of the MountingHole footprint, drag it out to the edge of the bord, click again and go anti-clockwise to the other edge of the board. 

- When placing a sensor on PCB: check the breakout boards from Sparkfun for the correct wiring. You can also download the schematics from their website

- When drawing a schematic: making comments with the `Place Text` button is a good idea!
## Python plots
template for a latex-style plot from a csv dataset
[here](https://github.com/simonperneel/Tips-n-Tricks/tree/master/Python%20plot)


## Sublime text
To put cursor at same place in everly line:
1. Select all text: `CTRL+A`
2. Activate multi-cursors: `CTRL+SHIFT+L`
3. Left/Right arrow keys to position cursor


