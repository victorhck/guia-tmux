 # Guía de tmux [WIP]
## _Una guía visual de los comandos de tmux_
![tmux logo](/img/tmux-logo-medium.png)

## Atajos de teclado predeterminados en tmux

[tmux](https://github.com/tmux/tmux/wiki) puede ser controlado desde un cliente asociado usando una combinación de teclas de unas teclas ya predeterminadas.

Para ejecutar los comandos de tmux, pulsa `C-b` (la tecla `Control` y la letra `b`) de manera predeterminada, seguido de algunos de estos comandos.

_Ya que algunas personas prefieren cambiar esa combinación predeterminada por otra (por ejemplo `C-a` que es más cómoda) me referiré de manera genérica a esa combinación como <Prefix>._

## Los atajos de teclado predeterminados son:

### Paneles
* `"`           Divide el panel actual en dos, uno superior y otro inferior.
![](/img/1.gif)
* `%`           Divide el panel actual en dos, uno a izquierda y otro a derecha.
![](/img/2.gif)
* `x`           Cierra el panel actual.
![](/img/3.gif)
* `o`           Selecciona el panel siguiente en la ventana actual.
![](/img/4.gif)
* `Up, Down, Left, Right`    Cambia el foco al panel superior, inferior, de la izquierda o derecha
![](/img/5.gif)
* `C-Up, C-Down, C-Left, C-Right`  Redimensiona el panel actual en pasos de una celda.
![](/img/6.gif)
* `M-Up, M-Down, M-Left, M-Right`  Redimensiona el panel actual en pasos de cinco celdas.
![](/img/7.gif)
* `;`           Se mueve al panel activo previo. Para alternar entre dos paneles.
![](/img/8.gif)
* `{`           Intercambia el panel actual con el panel previo.
* `}`           Intercambia el panel actual con el panel siguiente.
* `M-o`         Rota los paneles en en la ventana actual hacia adelante.
* `z`           Cambia el estado del zoom del panel actual.
* `q`           Muestra el número de índice brevemente en los paneles.
* `m`           Marca el panel actual (ver select-pane -m).
* `M`           Limpia el panel marcado.

### Ventanas
* `c`           Crea una nueva ventana.
* `n`           Cambia a la ventana siguiente.
* `p`           Cambia a la ventana previa.
* `0 a 9`       Selecciona la ventana especificada de la 0 a la 9.
* `l`           Se mueve a la ventana seleccionada previa.
* `w`           Escoge de manera interactiva la ventana actual.
* `i`           Muestra alguna información sobre la ventana actual.
* `.`           Pregunta un índice al que mover la ventana actual.
* `'`           Pregunta por el índice de una ventana para seleccionarla.
* `C-o`         Rota los paneles en la ventana actual hacia adelante.
