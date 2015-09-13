####¿Qué comando utilizaste en el paso 11? 
git reset --hard HEAD~1
####¿Por qué?
La acción era volver a la versión anterior después de realizar un commit. Para ello, simplemente habia que mover el puntero HEAD un nodo atras del que me encontraba en ese momento. Para mover el puntero HEAD se utiliza la instrucción reset de git. Para indicar que solamente quiero moverme un nodo atras del actual se utiliza la nomenclatura HEAD~1. La opción --hard es para que me actualize el work area.

####¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Al moverme al nodo anterior he perdido de vista el nodo donde habia realizado los cambios de los colores a hexadecimal, así que, con la instrucción "git reflog" liste los commits realizados en el repositorio. Se que el nodo que contiene la version del poema que busco es el nodo anterior a la instruccion del reset. En mi caso, dicho nodo es el "d686153". Sabiendo esto, solo tengo que realizar un reset a dicho nodo: "git reset --hard d686153"

####El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No causo ningún conflicto porque el fichero poem.md de la rama master no habia sido modificado en ningún momento

####El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si que hubo conflictos en este caso. El problema reside en que, mientras en la rama matrix, las palabras red y violet se habian cambiado por las frases "red pills" y "blue pills" respectivamente, en la rama htmlify, estas mismas palabras tenian dos valores en hexadecimal.

####El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No, no causo ningun conflicto porque en la rama master no se habia modificado el poema en las mismas lineas en que se habia modificado la rama htmlify

####¿Qué comando o comandos utilizaste en el paso 25?
Bueno... yo uso el alias de sg (super graph) que contiene la siguiente instruccion "log --graph --all --decorate"

####El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si porque no se habia evolucionado la rama master en ningun sentido despues de la creación de title. En otras palabras: La rama title contenia el trabajo de la rama master

####¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1

####¿Qué comando o comandos utilizaste en el paso 28?
git checkout -- poem.md

####¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title

####¿Qué comando o comandos utilizaste en el paso 30?
git checkout 6693affb0ea7bb4b253a7d3d55694a19cae73a2d
git branch title
git checkout master
git merge title --no-ff

####¿Qué comando o comandos usaste en el paso 32?
git sg
git reset --hard 75d2069406df19fccc8f0b09985cd6644124c01b

####¿Qué comando o comandos usaste en el punto 33?
git reflog
git reset --hard bcf02d2

