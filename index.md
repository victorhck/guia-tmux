# Guía de tmux [WIP]
## _Una guía visual de los comandos de tmux_
![tmux logo](/img/tmux-logo-medium.png)

## Atajos de teclado predeterminados en tmux

[tmux](https://github.com/tmux/tmux/wiki) puede ser controlado desde un cliente asociado usando una combinación de teclas de unas teclas ya predeterminadas.

Para ejecutar los comandos de tmux, pulsa `C-b` (la tecla `Control` y la letra `b`) de manera predeterminada, seguido de algunos de estos comandos.

_Ya que algunas personas prefieren cambiar esa combinación predeterminada por otra (por ejemplo `C-a` que es más cómoda) me referiré de manera genérica a esa combinación como `<Prefix>`._

_Pincha sobre la imagen para ampliar_

## Los atajos de teclado predeterminados son:

### Paneles
* `"`           Divide el panel actual en dos, uno superior y otro inferior.
<a href="https://victorhck.github.io/guia-tmux/img/1.gif"><img src="https://victorhck.github.io/guia-tmux/img/1.gif"></a>
* `%`           Divide el panel actual en dos, uno a izquierda y otro a derecha.
<a href="https://victorhck.github.io/guia-tmux/img/2.gif"><img src="https://victorhck.github.io/guia-tmux/img/2.gif"></a>
* `x`           Cierra el panel actual.
<a href="https://victorhck.github.io/guia-tmux/img/3.gif"><img src="https://victorhck.github.io/guia-tmux/img/3.gif"></a>
* `o`           Selecciona el panel siguiente en la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/4.gif"><img src="https://victorhck.github.io/guia-tmux/img/4.gif"></a>
* `Up, Down, Left, Right`    Cambia el foco al panel superior, inferior, de la izquierda o derecha
<a href="https://victorhck.github.io/guia-tmux/img/5.gif"><img src="https://victorhck.github.io/guia-tmux/img/5.gif"></a>
* `C-Up, C-Down, C-Left, C-Right`  Redimensiona el panel actual en pasos de una celda.
<a href="https://victorhck.github.io/guia-tmux/img/6.gif"><img src="https://victorhck.github.io/guia-tmux/img/6.gif"></a>
* `M-Up, M-Down, M-Left, M-Right`  Redimensiona el panel actual en pasos de cinco celdas.
<a href="https://victorhck.github.io/guia-tmux/img/7.gif"><img src="https://victorhck.github.io/guia-tmux/img/7.gif"></a>
* `;`           Se mueve al panel activo previo. Para alternar entre dos paneles.
<a href="https://victorhck.github.io/guia-tmux/img/8.gif"><img src="https://victorhck.github.io/guia-tmux/img/8.gif"></a>
* `{`           Intercambia el panel actual con el panel previo.
* `}`           Intercambia el panel actual con el panel siguiente.
<a href="https://victorhck.github.io/guia-tmux/img/9.gif"><img src="https://victorhck.github.io/guia-tmux/img/9.gif"></a>
* `M-o`         Rota los paneles en en la ventana actual hacia adelante.
<a href="https://victorhck.github.io/guia-tmux/img/10.gif"><img src="https://victorhck.github.io/guia-tmux/img/10.gif"></a>
* `z`           Cambia el estado del zoom del panel actual.
<a href="https://victorhck.github.io/guia-tmux/img/11.gif"><img src="https://victorhck.github.io/guia-tmux/img/11.gif"></a>
* `q`           Muestra el número de índice brevemente en los paneles.
<a href="https://victorhck.github.io/guia-tmux/img/12.gif"><img src="https://victorhck.github.io/guia-tmux/img/12.gif"></a>
* `m`           Marca el panel actual (ver select-pane -m).
* `M`           Limpia el panel marcado.
<a href="https://victorhck.github.io/guia-tmux/img/13.gif"><img src="https://victorhck.github.io/guia-tmux/img/13.gif"></a>

### Ventanas
* `c`           Crea una nueva ventana.
<a href="https://victorhck.github.io/guia-tmux/img/14.gif"><img src="https://victorhck.github.io/guia-tmux/img/14.gif"></a>
* `n`           Cambia a la ventana siguiente.
* `p`           Cambia a la ventana previa.
<a href="https://victorhck.github.io/guia-tmux/img/15.gif"><img src="https://victorhck.github.io/guia-tmux/img/15.gif"></a>
* `0 a 9`       Selecciona la ventana especificada de la 0 a la 9.
<a href="https://victorhck.github.io/guia-tmux/img/16.gif"><img src="https://victorhck.github.io/guia-tmux/img/16.gif"></a>
* `l`           Se mueve a la ventana seleccionada previa. Para alternar entre dos ventanas.
* `w`           Escoge de manera interactiva la ventana actual.
* `i`           Muestra alguna información sobre la ventana actual.
* `.`           Pregunta un índice al que mover la ventana actual.
* `'`           Pregunta por el índice de una ventana para seleccionarla.
* `C-o`         Rota los paneles en la ventana actual hacia adelante.
* `M-n`         Se mueve a la siguiente ventana con una señal o marcador de actividad.
* `M-p`         Se mueve a la ventana previa con una señal o marcador de actividad.
* `!`           Manda el panel actual fuera de la ventana actual.
* `Espacio`     Organiza la ventana actual en el siguiente esquema.
* `M-1 a M-5`   Organiza los paneles en uno de los cinco esquemas preconfigurados: iguales-horizontal, iguales-vertical, principal-horizontal, principal-vertical, o tiling
* `f`           Pregunta para buscar un texto en las ventanas abiertas.
* `&`           Cierra la ventana actual.

### Miscelánea
* `?`           Muestra un listado de todos los atajos de teclado.
* `t`           Muestra la hora.
* `$`           Renombra la sesión actual.
* `,`           Renombra la ventana actual.
* `[`           Entra en el modo de copiar para copiar texto o ver el historial.
* `]`           Pega el buffer de texto más reciente.
* `(`           Cambia el cliente seleccionado a la sesión previa.
* `)`           Cambia el cliente seleccionado a la sesión siguiente.
* `D`           Escoge un cliente para desconectarse.
* `L`           Cambia el cliente conectado de vuelta a la última sesión.
* `s`           Selecciona una nueva sesión de manera interactiva para el cliente conectado.
* `d`           Desconecta el cliente actual.                                  
* `~`           Muestra los mensajes previos de tmux, si hubiera alguno.
* `#`           Lista todos los buffers pegados.
* `-`           Elimina el buffer copiado más reciente de texto.
* `=`           Escoge qué buffer pegar de manera interactiva desde una lista.
* `:`           Entra en el modo de comandos de tmux.
* `r`           Fuerza el redibujar el cliente conectado.
* `Page Up`     Entra en el modo de copiar y hace scroll de una página.

`C` Se refiere a la tecla Control. `M` Se refiere a la tecla Meta, que es la tecla Alt.
Los atajos de teclado pueden ser cambiados con los comandos bind-key y unbind-key.

