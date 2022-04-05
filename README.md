# AprendiendoGitHub
Este es un repositorio que destine para aprender Git y Gitbub


### MIS NOTAS ###

# Para ver la lista configuraciones 
	git config --list

# Configuración de usuario en Git
	git config --global user.name "Luis Arrieta"
	git config --global user.email "luisarrieta796@gmail.com"

## GIT

# Dentro de la carpeta raíz del proyecto, empezar un repositorio
	git init

# Para ver el estado de cambios del proyecto
	git status

# añadir archivo a una memoria temporal (al staging)
	git add historia.txt

# añadir todos los archivos modificados (al staging)
	git add .

# Realizar un commit para guardar cambios
	git commit -m "Este es el primer commit de este proyecto"

# Ver historia de todos los commits de un archivo
	git log historia.txt

# Para ver los cambios de cada linea
	git show historia.txt

# Para comparar los cambios de commit a commit (indicadores o id del commits) 
	git diff 12a3d7g1j2hf 9t8dfgdf4gdswwe
`			 (ID Actual / Otro ID Version)

# Ver los cambios entre el directorio actual y el staging
	git diff

# Reiniciar a una versión borrando todos los commits a su paso 
	git reset 1a2sds3rfgdd12fdg3 --hard

# Ver una versión anterior, reemplazando el archivo actual
	git checkout 12asd3asd1as historia.txt

# Volver a la versión inicial que se tenia antes de ver la version anterior
	git checkout master historia.txt

# Si el cambio se quiere permanente se hace el commit
	git commit -m "Reemplazo de ..."

# Hacer un add y commit al mismo tiempo, pero estos previamente ya han sido additionados xd
	git commit -am "Este es un comentario"


# Crear rama o Branch
	git branch nombre-de-branch

# Renombrar nombrre de Branch
	git branch -m nuevo-nombre

# Mover historial de un Branch a otro
	git branch -M nombre-de-branch

# Ver todos los Branchs
	git branch

# Cambiar entre branchs
	git checkout nombre-de-branch

# Fusionar branchs y posteriormente darle un mensaje
	git merge nombre-de-branch


## GITHUB

# Una vez creado el repositorio en Github.com, se conecta de la siguiente manera
	git remote add origin https://github.com/username/namerepository

# Para ver a qué repositorio esta conectado remotamente
	git remote -v

# Enviar al repositorio remoto un Branch
	git push origin master

# Obtener el repositorio de github
	git pull origin master

# Forzar a obtener el repositorio de github para fusionar el proyecto con el repositorio de github
	git pull origin master --allow-unrelated-histories

# Para traer el proyecto del repositorio remoto
	git clone url
