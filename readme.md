¿Qué comando utilizaste en el paso 11? ¿Por qué?
    git reset --hard HEAD~1.
    Porque reset HEAD~1 retrasa el puntero HEAD y el puntero de rama al commit anterior, y con el modificador --hard, perdemos los cambios en el working copy 

-¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
	git reflog
	git reset --hard 44ba8c2
	
	git reflog para conocer el hash del commit al que quiero ir.
	git reset --hard 44ba8c2. Para que lleve el puntero HEAD y la rama al commit seleccionado, y con modificador --hard para recuperar los cambios perdidos en el working copy
	
-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
	No causa ningun conflicto porque se necesita un cambio en la misma linea de DOS ramas diferentes para generar conflictos.
	Ni siquiera se produce un merge porque la rama esta actualizada.
	
-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
	Si porque tenemos cambios en la rama STYLED y en la rama HTMLIFY
	
-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
	No porque solo hay cambios en la rama STYLED, asi que realiza un MERGE fast forward.
	
-¿Qué comando o comandos utilizaste en el paso 25?
	git log --graph
	
-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
	Si porque la rama MASTER ya puede llegar a los commit de HTMLIFY y STYLED, solo añadiemos el hecho dsde TITLE
	
-¿Qué comando o comandos utilizaste en el paso 27?
	git reset HEAD~1, aunque vengamos de un merge no FF GIT sabe de que commit proviene y vuelve al commit antes del merge.
	
-¿Qué comando o comandos utilizaste en el paso 28?
	git checkout git-nuestro.md
	
-¿Qué comando o comandos utilizaste en el paso 29?
	git branch -D title
	
-¿Qué comando o comandos utilizaste en el paso 30?
	git merge 04305a6
	
-¿Qué comando o comandos usaste en el paso 32?
	git reset --hard HEAD@{21}

-¿Qué comando o comandos usaste en el punto 33?
	git reset --hard HEAD@{5}