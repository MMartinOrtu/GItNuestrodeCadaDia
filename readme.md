# Práctica del curso de git, gitHub y Sourcetreea
### Ejercicio 1: Respuestas a las preguntas planteadas

*Qué comando utlizaste en el paso 11? ¿Por qué?*

```
git reset --hard HEAD~1
```
He utilizado el comando **git reset --hard HEAD~1** ya que con dicho 
comando se consigue deshacer el último commit, es decir, mover la rama 
**styled** al commit inmediatamente anterior y, además, elimina los 
cambios que habíamos hecho anteriormente en el working copy 
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

*¿Qué comando o comandos utilizaste en el paso 25?*

```
git log --graph
```
He usado git --graph, también se pueden añadir modificadores para 
mejorar la visibilidad del grafo como

```
git log --graph --decorate --pretty=online
```

*El merge del paso 26, ¿Podría ser fast foward? ¿Por qué?*

Sí, podría ser un merge fast foward ya que la rama **title** solo está 
un commit por arriba de la rama **master**, es decir, la rama master 
ya se encontraba integrada en la rama **title**.

*¿Qué comando o comandos utilizaste en el paso 27?*

```
git reset HEAD~1
```
Con este comando volvemos al commit anterior de la rama desde la que 
hemos hecho el merge sin perder los cambios del working copy.

*¿Qué comando o comandos utilizaste en el paso 28?*

```
git status
git checkout -- git-nuestro.md
```
He usado primero un *git status* para consultar el estado del 
repositorio y comprobar que el comando necesario para descartar los 
cambios era *git checkout -- <archivo>*.

*Qué comando o comandos utilizaste en el paso 29?*

```
git branch -D title
````

*¿Qué comando o comandos utilizaste en el paso 30?*

```
git reflog
git reset --hard 0f7af3b
```
Primero he hecho un *git reflog* para ver el identificador del commit 
donde habíamos realizado el merge y, después, he hecho un *git reset 
--hard 0f7af3b* para volver a dicho commit.

*¿Qué comando o comando utilizaste el el paso 32?*

```
git reflog
git reset --hard c8b79aa
```
Primero un *git reflog* para ver el identificador del commit donde se 
creó el poema y después un *git reset* a dicho commit, aquí no se 
indicaba si tenía que ser --hard o no, pero yo lo puse --hard.

*¿Qué comando o comando utilizaste en ele paso 33?*

```
git reflog
git reset --hard 07af3b
```
Igual que antes, primero he hecho un *git reflog* y después un *git 
reset --hard 07af3b* para volver al estado final.

