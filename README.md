Crear un repositorio en vuestro GitHub llamado masteruah.
	Se hace de maner gráfica en github

Clonar vuestro repositio en local.
	git clone <urlProyec>

Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md.
	Se hace manualmente

Añadir al README.md los comanddos utilizados hasta ahora y hacer un coomit inicial con el mensaje commit inicial.
	git status
	git add .
	git status
	git commit -m "commit inicial"

Subir los cambios al repositorio remoto.
	git branch -M main
	git push -u origin main

Crear en el repositorio local un fichero llamado privado.txt.
Crear en el repositorio local una carpeta llamada privada.
	Éstos dos se hacen manualmente

Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.
	Crear arch ".gitignore", escribir dentro los nombres y carpetas a ignorar, separados por un salto de línea

Añadir fichero 1.txt al repositorio local.
	Se hace manual

Crear un tag v0.1.
	git tag v0.1

Subir los cambios al repositorio remoto.
	git push