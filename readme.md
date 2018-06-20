# Práctica del curso de git, gitHub y Sourcetree
### Ejercicio 1: Respuestas de las preguntas planteadas

*Qué comando utlizaste en el paso 11? ¿Por qué?*

```
git reset --hard HEAD~1
```
He utilizado el comando **git reset --hard HEAD~1** ya que con dicho 
comando se consigue deshacer el último commit, es decir, mover la rama 
**styled** al commit inmediatamente anterior y, además, elimina los 
cambios que habíamos hecho anteriormente el en el working copy 
(gracias al modificador --hard).


*¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?*

```
git reflog
git reset --hard 20b3b82
```
Primero he usado **git reflog** para acceder al hitórico de commits 
realizados y poder ver el identificador del commit deshecho 
anteriormente. A continuación, ejecuto **git reset --hard 20b3b82** 
para llevar la rama **styled** ha dicho commit devolviendo los cambios 
del working copy tal y como estaban antes de deshacer el commit.

*El merge del paso 13, ¿Causó algún conflicto?¿Por qué?*

No, no causó ningún clonflicto, ni siquiera ha llegado a realizarse el 
merge ya que la rama **master** ya se encontraba integrada en la rama 
**styled**, por lo que nos aparece el mensaje *already up-to-date*.

*El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*

Ŝí, en este merge surgió un conflicto ya que tanto en la rama 
**styled** como en la rama **htnlify** habíamos modificados las mismas 
líneas en ambas ramas, por lo que al hacer el merge git nos genera un 
conflicto para que seamos nosotros los que decidamos qué contenido es 
el que debemos dejar en el archivo. En nuestro caso, nos quedamos con 
el contenido de que había en la rama **styled**.

*El merge del paso 21, ¿Causó algún conflicto? ¿Po qué?

No, este merge no causó ningún conflicto ya que ha sido un merge 
Fast-foward, pues la rama **master** ya se encontraba incluída en la 
rama **styled**, por que solamente se ha movido el puntero de la rama 
**master** al último commit donde está el puntero de la rama 
**styled**.


