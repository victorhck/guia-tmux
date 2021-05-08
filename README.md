# Guía de tmux
## _Una guía visual de los comandos de tmux_
![tmux logo](/img/tmux-logo-medium.png)

## Atajos de teclado predeterminados en tmux

tmux puede ser controlado desde un cliente asociado usando una combinación de teclas de unas teclas ya predeterminadas.
Para ejecutar los comandos de tmux, pulsa `C-b` (Ctrl-b) de manera predeterminada, seguido de algunos de estos comandos.

## Los atajos de teclado predeterminados son:

* `?`           Muestra un listado de todos los atajos de teclado.
* `t`           Muestra la hora.
* `$`           Renombra la sesión actual.
* `,`           Renombra la ventana actual.
* `"`           Divide el panel actual en dos, uno superior y otro inferior.
* `%`           Divide el panel actual en dos, uno a izquierda y otro a derecha.
* `x`           Cierra el panel actual.
* `o`           Selecciona el panel siguiente en la ventana actual.
* `Up, Down, Left, Right`    Cambia el foco al panel superior, inferior, de la izquierda o derecha
* `;`           Se mueve al panel activo previo.
* `c`           Crea una nueva ventana.
* `n`           Cambia a la ventana siguiente.
* `p`           Cambia a la ventana previa.
* `0 a 9`       Selecciona la ventana especificada de la 0 a la 9.
* `w`           Escoge de manera interactiva la ventana actual.
* `i`           Muestra alguna información sobre la ventana actual.
* `.`           Pregunta un índice al que mover la ventana actual.
* `C-o`         Rota los paneles en la ventana actual hacia adelante.
* `!`           Manda el panel actual fuera de la ventana actual.

           #           Lista todos los buffers pegados.

           &           Cierra la ventana actual.
           '           Pregunta por el índice de una ventana para seleccionarla.
           (           Cambia el cliente seleccionado a la sesión previa.
           )           Cambia el cliente seleccionado a la sesión siguiente.
           -           Elimina el buffer copiado más reciente de texto.
           :           Entra en el modo de comandos de tmux.
           =           Escoge qué buffer pegar de manera interactiva desde una lista.
           D           Escoge un cliente para desconectarse.
           L           Cambia el cliente conectado de vuelta a la última sesión.
           [           Entra en el modo de copiar para copiar texto o ver el historial.
           ]           Pega el buffer de texto más reciente.
           d           Desconecta el cliente actual.                                  
           f           Pregunta para buscar un texto en las ventanas abiertas.
           l           Se mueve a la ventana seleccionada previa.
           m           Marca el panel actual (ver select-pane -m).
           M           Limpia el panel marcado.
           q           Muestra el número de índice brevemente en los paneles.
           r           Fuerza el redibujar el cliente conectado.
           s           Selecciona una nueva sesión de manera interactiva para el cliente conectado.
           z           Cambia el estado del zoom del panel actual.
           {           Intercambia el panel actual con el panel previo.
           }           Intercambia el panel actual con el panel siguiente.
           ~           Muestra los mensajes previos de tmux, si hubiera alguno.
           Page Up     Entra en el modo de copiar y hace scroll de una página.
           M-1 a M-5   Organiza los paneles en uno de los cinco esquemas preconfigurados: iguales-horizontal, iguales-vertical, 
                       principal-horizontal, principal-vertical, o tiling
           Espacio     Organiza la ventana actual en el siguiente esquema.
           M-n         Se mueve a la siguiente ventana con una señal o marcador de actividad.
           M-o         Rota los paneles en en la ventana actual hacia adelante.
           M-p         Se mueve a la ventana previa con una señal o marcador de actividad.
           C-Up, C-Down
           C-Left, C-Right
                       Redimensiona el panel actual en pasos de una celda.
           M-Up, M-Down
           M-Left, M-Right
                       Redimensiona el panl actual en pasos de cinco celdas.

`C` Se refiere a la tecla Control. `M` Se refiere a la tecla Meta, que es el Alt.
Los atajos de teclado pueden ser cambiados con los comandos bind-key y unbind-key.

