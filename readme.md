####¿Qué comando utilizaste en el paso 11? 
git reset --hard HEAD~1
####¿Por qué?
La acción era volver a la versión anterior después de realizar un commit. Para ello, simplemente habia que mover el puntero HEAD un nodo atras del que me encontraba en ese momento. Para mover el puntero HEAD se utiliza la instrucción reset de git. Para indicar que solamente quiero moverme un nodo atras del actual se utiliza la nomenclatura HEAD~1. La opción --hard es para que me actualize el work area.
####¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Al moverme al nodo anterior he perdido de vista el nodo donde habia realizado los cambios de los colores a hexadecimal, así que, con la instrucción "git reflog" liste los commits realizados en el repositorio. Se que el nodo que contiene la version del poema que busco es el nodo anterior a la instruccion del reset. En mi caso, dicho nodo es el "d686153". Sabiendo esto, solo tengo que realizar un reset a dicho nodo: "git reset --hard d686153"
####El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
####El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
####El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
####¿Qué comando o comandos utilizaste en el paso 25?
####El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
####¿Qué comando o comandos utilizaste en el paso 27?
####¿Qué comando o comandos utilizaste en el paso 28?
####¿Qué comando o comandos utilizaste en el paso 29?
####¿Qué comando o comandos utilizaste en el paso 30?
####¿Qué comando o comandos usaste en el paso 32?
####¿Qué comando o comandos usaste en el punto 33?