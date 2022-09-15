# Guía de tmux
## _Una guía visual de los comandos de tmux_
![tmux logo](/img/tmux-logo-medium.png)

## Atajos de teclado predeterminados en tmux

[tmux](https://github.com/tmux/tmux/wiki) puede ser controlado desde un cliente asociado usando una combinación de teclas de unas teclas ya predeterminadas.

Para ejecutar los comandos de tmux, pulsa `C-b` (la tecla `Control` y la letra `b`) de manera predeterminada, seguido de algunos de estos comandos.

En tmux existen las sesiones, las ventanas y los paneles.

* **Las sesiones** son tareas realizadas en tmux que pueden quedar trabajando en segundo plano aunque cerremos la consola, mientras el equipo siga encendido. Podemos más tarde volver a conectarnos a esas sesiones para ver cómose están desarrollando las tareas, para finalizarlas, comenzar otras, etc.
* **Las ventanas** son los espacios de trabajo de tmux. Estas ventanas asociadas a las sesiones, son donde realizaremos las tareas que deseemos en la consola. Podemos abrir muchas ventanas distintas en cada sesión.
* **Los paneles** son divisiones de las ventanas. Podemos tener una vista dividida de cada ventana en múltiples paneles y en cada uno estar realizando una tarea distinta.

En esta guía veremos estas tres herramientas de tmux de manera inversa, es decir, primero los paneles, después las ventanas y por último las sesiones. Más una parte anexa de miscelánea con diversos comandos.

_Ya que algunas personas prefieren cambiar esa combinación predeterminada por otra (por ejemplo `C-a` que es más cómoda) me referiré de manera genérica a esa combinación como `<Prefix>`._

_Pincha sobre la imagen para ampliar_

## Paneles

* `<Prefix>` + `"`           Divide el panel actual en dos, uno superior y otro inferior.
<a href="https://victorhck.github.io/guia-tmux/img/1.gif"><img src="https://victorhck.github.io/guia-tmux/img/1.gif"></a>
* `<Prefix>` + `%`           Divide el panel actual en dos, uno a izquierda y otro a derecha.
<a href="https://victorhck.github.io/guia-tmux/img/2.gif"><img src="https://victorhck.github.io/guia-tmux/img/2.gif"></a>
* `<Prefix>` + `x`           Cierra el panel actual.
<a href="https://victorhck.github.io/guia-tmux/img/3.gif"><img src="https://victorhck.github.io/guia-tmux/img/3.gif"></a>
* `<Prefix>` + `o`           Selecciona el panel siguiente en la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/4.gif"><img src="https://victorhck.github.io/guia-tmux/img/4.gif"></a>
* `<Prefix>` + `Up, Down, Left, Right`    Cambia el foco al panel superior, inferior, de la izquierda o derecha
<a href="https://victorhck.github.io/guia-tmux/img/5.gif"><img src="https://victorhck.github.io/guia-tmux/img/5.gif"></a>
* `<Prefix>` + `C-Up, C-Down, C-Left, C-Right`  Redimensiona el panel actual en pasos de una celda.
<a href="https://victorhck.github.io/guia-tmux/img/6.gif"><img src="https://victorhck.github.io/guia-tmux/img/6.gif"></a>
* `<Prefix>` + `M-Up, M-Down, M-Left, M-Right`  Redimensiona el panel actual en pasos de cinco celdas.
<a href="https://victorhck.github.io/guia-tmux/img/7.gif"><img src="https://victorhck.github.io/guia-tmux/img/7.gif"></a>
* `<Prefix>` + `;`           Se mueve al panel activo previo. Para alternar entre dos paneles.
<a href="https://victorhck.github.io/guia-tmux/img/8.gif"><img src="https://victorhck.github.io/guia-tmux/img/8.gif"></a>
* `<Prefix>` + `{`           Intercambia el panel actual con el panel previo.
* `<Prefix>` + `}`           Intercambia el panel actual con el panel siguiente.
<a href="https://victorhck.github.io/guia-tmux/img/9.gif"><img src="https://victorhck.github.io/guia-tmux/img/9.gif"></a>
* `<Prefix>` + `M-o`         Rota los paneles en la ventana actual hacia adelante.
<a href="https://victorhck.github.io/guia-tmux/img/10.gif"><img src="https://victorhck.github.io/guia-tmux/img/10.gif"></a>
* `<Prefix>` + `C-o`         Rota los paneles en la ventana actual hacia atrás.
<a href="https://victorhck.github.io/guia-tmux/img/10bis.gif"><img src="https://victorhck.github.io/guia-tmux/img/10bis.gif"></a>
* `<Prefix>` + `z`           Cambia el estado del zoom del panel actual.
<a href="https://victorhck.github.io/guia-tmux/img/11.gif"><img src="https://victorhck.github.io/guia-tmux/img/11.gif"></a>
* `<Prefix>` + `q`           Muestra el número de índice brevemente en los paneles.
<a href="https://victorhck.github.io/guia-tmux/img/12.gif"><img src="https://victorhck.github.io/guia-tmux/img/12.gif"></a>
* `<Prefix>` + `m`           Marca el panel actual (ver select-pane -m).
* `<Prefix>` + `M`           Limpia el panel marcado.
<a href="https://victorhck.github.io/guia-tmux/img/13.gif"><img src="https://victorhck.github.io/guia-tmux/img/13.gif"></a>

## Ventanas

* `<Prefix>` + `c`           Crea una nueva ventana.
<a href="https://victorhck.github.io/guia-tmux/img/14.gif"><img src="https://victorhck.github.io/guia-tmux/img/14.gif"></a>
* `<Prefix>` + `n`           Cambia a la ventana siguiente.
* `<Prefix>` + `p`           Cambia a la ventana previa.
<a href="https://victorhck.github.io/guia-tmux/img/15.gif"><img src="https://victorhck.github.io/guia-tmux/img/15.gif"></a>
* `<Prefix>` + `,`           Renombra la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/28.gif"><img src="https://victorhck.github.io/guia-tmux/img/28.gif"></a>
* `<Prefix>` + `0 a 9`       Selecciona la ventana especificada de la 0 a la 9.
<a href="https://victorhck.github.io/guia-tmux/img/16.gif"><img src="https://victorhck.github.io/guia-tmux/img/16.gif"></a>
* `<Prefix>` + `w`           Escoge de manera interactiva la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/17.gif"><img src="https://victorhck.github.io/guia-tmux/img/17.gif"></a>
* `<Prefix>` + `i`           Muestra brevemente información sobre la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/18.gif"><img src="https://victorhck.github.io/guia-tmux/img/18.gif"></a>
* `<Prefix>` + `.`           Pregunta un índice al que mover la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/19.gif"><img src="https://victorhck.github.io/guia-tmux/img/19.gif"></a>
* `<Prefix>` + `'`           Pregunta por el índice de una ventana para seleccionarla.
<a href="https://victorhck.github.io/guia-tmux/img/20.gif"><img src="https://victorhck.github.io/guia-tmux/img/20.gif"></a>
* `<Prefix>` + `!`           Manda el panel actual fuera de la ventana actual creando una nueva ventana del panel.
<a href="https://victorhck.github.io/guia-tmux/img/21.gif"><img src="https://victorhck.github.io/guia-tmux/img/21.gif"></a>
* `<Prefix>` + `Espacio`     Organiza la ventana actual en el siguiente diseño de paneles preconfigurado.
* `<Prefix>` + `M-1 a M-5`   Organiza los paneles en uno de los cinco diseños preconfigurados: iguales-horizontal, iguales-vertical, principal-horizontal, principal-vertical, o tiling
<a href="https://victorhck.github.io/guia-tmux/img/22.gif"><img src="https://victorhck.github.io/guia-tmux/img/22.gif"></a>
* `<Prefix>` + `f`           Busca un texto en las ventanas y muestra la ruta donde se encuentra.
<a href="https://victorhck.github.io/guia-tmux/img/23.gif"><img src="https://victorhck.github.io/guia-tmux/img/23.gif"></a>
* `<Prefix>` + `&`           Cierra la ventana actual.
<a href="https://victorhck.github.io/guia-tmux/img/24.gif"><img src="https://victorhck.github.io/guia-tmux/img/24.gif"></a>

## Sesiones

* `<Prefix>` + `d`           Desconecta el cliente actual.                                  
* `<Prefix>` + `s`           Selecciona una nueva sesión de manera interactiva para el cliente conectado.
<a href="https://victorhck.github.io/guia-tmux/img/29.gif"><img src="https://victorhck.github.io/guia-tmux/img/29.gif"></a>
* `<Prefix>` + `(`           Cambia el cliente seleccionado a la sesión previa.
* `<Prefix>` + `)`           Cambia el cliente seleccionado a la sesión siguiente.
<a href="https://victorhck.github.io/guia-tmux/img/30.gif"><img src="https://victorhck.github.io/guia-tmux/img/30.gif"></a>
* `<Prefix>` + `$`           Renombra la sesión actual.
<a href="https://victorhck.github.io/guia-tmux/img/27.gif"><img src="https://victorhck.github.io/guia-tmux/img/27.gif"></a>

## Miscelánea

* `<Prefix>` + `?`           Muestra un listado de todos los atajos de teclado.
<a href="https://victorhck.github.io/guia-tmux/img/25.gif"><img src="https://victorhck.github.io/guia-tmux/img/25.gif"></a>
* `<Prefix>` + `t`           Muestra la hora.
<a href="https://victorhck.github.io/guia-tmux/img/26.gif"><img src="https://victorhck.github.io/guia-tmux/img/26.gif"></a>
* `<Prefix>` + `[`           Entra en el modo de copiar para copiar texto o ver el historial.
* `<Prefix>` + `]`           Pega el buffer de texto más reciente.
* `<Prefix>` + `~`           Muestra los mensajes previos de tmux, si hubiera alguno.
* `<Prefix>` + `#`           Lista todos los buffers pegados.
* `<Prefix>` + `-`           Elimina el buffer copiado más reciente de texto.
* `<Prefix>` + `=`           Escoge qué buffer pegar de manera interactiva desde una lista.
* `<Prefix>` + `:`           Entra en el modo de comandos de tmux.
* `<Prefix>` + `r`           Fuerza el redibujar el cliente conectado.
* `<Prefix>` + `Page Up`     Entra en el modo de copiar y hace scroll de una página.

`C` Se refiere a la tecla Control. `M` Se refiere a la tecla Meta, que es la tecla Alt.
Los atajos de teclado pueden ser cambiados con los comandos bind-key y unbind-key.

