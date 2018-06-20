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

