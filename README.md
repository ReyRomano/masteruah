## Ejericio: Crear una tabla

- Crear una tabla de este estilo en el fichero README.md con la información de varios de tus compañeros de clase:

|	NOMBRE	|	GITHUB	|
| ------------	|	----------	|
|	Alfredo S.	|	[Enlace a github 1](https://github.com/asalber/libro-git)	|
|	Brais Moure	|	[Enlace  a github 2](https://github.com/mouredev/hello-git)	|
|	Rey R.	|	[Enlace  a github 3](https://github.com/ReyRomano/masteruah)	|

----
----

### -- Pasos para resolver "Ejercicios básicos de Git, GitHub y Markdown - https://github.com/asanzdiego/curso-git-github-markdown-2017/blob/master/ejercicios/git-github-markdown-ejercicios-01-basico.md": --

## Repositorio masteruah

- Crear un repositorio en vuestro GitHub llamado **masteruah**.

		Se hace de maner gráfica en github

- OK. Resp oficial, R=

		En el menú de GitHub > Pulsar en el icono “+” > Pinchar en “New repository”

- Clonar vuestro repositio en local.

		git clone **(urlProyec)**

- OK. Resp oficial, R=

		git clone git@github.com:asanzdiego/masteruah.git

## README

- Crear (si no lo habéis creado ya) en vuestro repositorio local
un documento **README.md**.

> Notas: en este documento tendreís que ir poniendo los **comandos** que habéis tenido que utilizar durante todos los ejercicios y las **explicaciones y capturas de pantalla** que consideréis **necesarias**.

	Se hace manualmente

## Commit inicial

- Añadir al README.md los comanddos utilizados hasta ahora
y hacer un coomit inicial con el mensaje **commit inicial**.

		git status
		git add .
		git status
		git commit -m "commit inicial"

## Push inicial

- Subir los cambios al repositorio remoto.

		git branch -M main
		git push -u origin main

- OK. Resp oficial, R=
		
		git push origin master

## Ignorar archivos

- Crear en el repositorio local un fichero llamado **privado.txt**.
- Crear en el repositorio local una carpeta llamada **privada**.

		Éstos dos se hacen manualmente

- Realizar los cambios oportunos para que tanto el archivo como
la carpeta sean ignorados por git.

		Crear archivo ".gitignore", y meter el siguiente código, es importante respetar los saltos de línea ya que diferencían a un archivo de otro:
		#Ignorando carpeta y archivo "privada" y "privado", sólo deben estar separados por el salto de línea para que los reconozca como diferentes
		privada
		privado.txt

## Añadir fichero 1.txt

- Añadir fichero **1.txt** al repositorio local.

		Crear archivo "1.txt"

- Resp oficial, R=

		touch 1.txt
		git add .
		git commit -m "añadido 1.txt"

## Crear el tag v0.1

- Crear un tag **v0.1**.

		git tag v0.1

## Subir el tag v0.1

- Subir los cambios al repositorio remoto.

		git status
		git add .
		git status
		git commit -m "Subiendo el tag v0.1"
		git push

- Resp oficial, R=

		git push --tag origin master

## Cuenta de GitHub

- Poner una foto en vuestro perfil de GitHub.

		Se hace manualmente

- Poner el doble factor de autentificación en vuestra cuenta de GitHub.

		Actualmente git ya lo maneja como obligatorio. Se puede desactivar pero se pierden ciertas funciones para el manejo de repositorios privados.

- Añadir (si no lo habéis hecho ya) la clave pública que se corresponde a tu ordenador.

		Seguir [Curso de GIT y GITHUB - MoureDev](https://www.youtube.com/watch?v=3GymExBkKjE) , min  **2 : 47 : 30**

- OK. Resp oficial, R=

		[Seguir esta guía](https://help.github.com/articles/generating-ssh-keys/)

## Uso social de GitHub

- Preguntar los nombres de usuario de GitHub de tus compañeros de clase, búscalos, y sigueles.
- Seguir los repositorios **masteruah** del resto de tus compañeros.
- Añadir una estrella a los repositorios **masteruah** del resto de tus compañeros.

		Éstos tres se hacen manualmente

- OK. Resp oficial. R=

		Ir a http://github.com/usuario y pulsar en "Follow"
		Ir a http://github.com/usuario/masteruah y pulsar en "Star"

## Crear una tabla

- Crear una tabla de este estilo en el fichero README.md con la información de varios de tus compañeros de clase:

		Se usa el siguiente código:
		|	NOMBRE	|	GITHUB	|
		| ------------	|	----------	|
		|	Nombre del compañero 1	|	[Enlace a github 1](https://github.com/asalber/libro-git)	|
		|	Nombre del compañero 2	|	[Enlace  a github 2](https://github.com/mouredev/hello-git)	|
		|	Nombre del compañero 3	|	[Enlace  a github 3](https://github.com/ReyRomano/masteruah)	|

##Colaboradores

- Poner a [github.com/asanzdiego](https://github.com/asanzdiego) como colaborador del repositorio **masteruah**

		Se hace manualmente desde repositorio de git

- OK. Resp oficial, R=

		Ir a http://github.com/usuario/masteruah > Pinchar en "Settings" > Pinchar en "Collaborators"

----
----

### -- Pasos para resolver "Ejercicios avanzados de Git, GitHub y Markdown - https://github.com/asanzdiego/curso-git-github-markdown-2017/blob/master/ejercicios/git-github-markdown-ejercicios-02-avanzado.md": --

## Notas

- Este ejercicio es continuación del anterior por lo que tendréis que seguir trabajando en el repositorio **masteruah**.

- También tendreís que ir poniendo los **comandos** que habéis tenido que utilizar durante todos los ejercicios y las **explicaciones y capturas de pantalla** que consideréis **necesarias** al fichero README.md del citado repositorio.

## Crear una rama v0.2

- Crear una rama **v0.2**.

- Posiciona tu carpeta de trabajo en esta rama.

		git checkout -b v0.2	//Este comando crea rama y te posiciona en ella al mismo tiempo

## Añadir fichero 2.txt

- Añadir un fichero **2.txt** en la rama **v0.2**.

		Esto se hace manualmente

## Crear rama remota v0.2

- Subir los cambios al reposiorio remoto.

		git add .
		git commit -m "Creando rama remota v0.2"
		git push -u origin v0.2

## Merge directo

- Posicionarse en la rama **master**.

		git checkout "id de último commit de rama main"

- Hacer un merge de la rama **v0.2** en la rama **master**.

		git merge v0.2

## Merge con conflicto

- En la rama **master** poner **Hola** en el fichero **1.txt** y hacer commit.

		switch main

		Escribir manualmete Hola en fichero.

		git status
		git add 1.txt
		git status
		git commit -m "Iniciando conflicto con -Hola- en 1.txt"
		git status
		git tree

- Posicionarse en la rama **v0.2** y poner **Adios** en el fichero "1.txt" y hacer commit.

		git switch v0.2
		Escribir manualmete Adios en fichero.

		git status
		git add 1.txt
		git status
		git commit -m "Continuando conflicto con -Adiós- en 1.txt"
		git status
		git tree

- Posicionarse de nuevo en la rama **master** y hacer un merge con la rama **v0.2**

		git switch main
		git merge v0.2

## Listado de ramas

- Listar las ramas con merge y las ramas sin merge.

		git branch
		git branch -av

## Arreglar conflicto

- Arreglar el conflicto anterior y hacer un commit.

		En 1.txt, el conflicto resuelto queda:
			Hola y Adiós

		git status
		git add .
		git status
		git commit -m "Resuelto conflicto con Hola y adiós en 1.txt"

		Al resolver  el conflicto y hacer el commit, en automático se mergea lo que marcaba error

		git status
		git tree

## Borrar rama

- Crear un tag v0.2

		git tag		//ver todos los tags
		git tag v0.2

		git tree
		git tag

- Borrar la rama v0.2

		

