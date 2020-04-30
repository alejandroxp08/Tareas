
## Diferencia entre git merge y git merge --no -ff

### git merge

El `git merge` sirve para fusionar una o mas ramas dentro de la rama
que tengas  activa o abierta.A continuacion ira donde se encuentre la
rama donde se encuentre el resultado de la fusion
[ejemplo](https://i.stack.imgur.com/GGkZc.png),esta 
fusion se realiza de manera plana tal como se ve en la imagen.

### git merge --no --ff
Se puede ver claramente en el [ejemplo](https://i.stack.imgur.com/GGkZc.png).Esta es una opcion que se le aumenta, el `--no --ff` lo que hace es
evitar un fast forward, esto si se detecta que el **HEAD** es una 
version anterior de la confirmacion que se esta intentando fusionar.Esto permite revisar el historial(log),de la rama que  la que hiciste `checkout`

### ¿Que es un fast forward?
Es cuando, en lugar de de hacer fusionar un commit, solo se 
mueve el **HEAD** de la rama para apuntar al commit entrante.