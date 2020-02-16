# Manual

pwd : indica cual es la carpeta actual donde estoy.

cd.. : sale de la carpeta

cd carpeta: entra en la carpeta

rm: borra un archivo

rm-rf carpeta: borrar una carpeta y todo su contenido

code . : abre visual studio

---------------------------------------------------------------
$ es el intermediario que recibe los comandos

cd ~ // 

mkdir susana2 : Creo un directorio

cd susana2 : Ingreso a mi directorio

ls: Lista archivo

git init : Inicializa un repositorio, se creará una carpeta llamada .git

touch   lala.txt : Crear un archivo "lala.txt"

git status : Verificar el estado de nuestro repositorio

git add lala.txt : Busca el archivo (si fuese . buscaria todos los archivos) y  agrega todos los archivos nuevos en preparación (staging)

git commit : Realiza los cambios 

git diff : Muestra las diferencias 

git checkout : Actualiza las modificaciones 

git remote show origin : Indica a cuál rama enviarás información automáticamente cada vez que ejecutas git push

git push origin master : Empuja el repositorio / lleva los últimos cambios a github

git fetch  : Actualiza el repostorio local

git pull origin master  : Actualiza directorio

git remote rm origin : Remueve url de github

git clone : Clona un repositorio de github a tu directorio de trabajo local

-------------------------------------------------------------------------
  //Procedimiento 1: Entrar a un reposotorio git

  git clone https://github.com/susana9396/manual.git //En el ejemplo ingreso al repositorio manual

  cd .. //salgo de la carpeta

  cd manual // ingreso a la carpeta manual
 
-------------------------------------------------------------------------
  //Procedimiento 2: Subir un archivo a un repositorio git

  cd manual // Ingreso al repositorio en que quiero cargar archivo

  touch "archivo.txt" // Creo Archivo 

  git add archivo.txt // busco el archivo

  git commit -m "Comentario" // Envío archivo al área de preparación

  git status // verifico que el archivo esté en verde

  git push origin master // Subo archivo al repositorio manual

-------------------------------------------------------------------------
  //Ejemplo 1: Para verificar el estado de una actualización del archivo.
  
  $ git status
  On branch master 

  No commits yet

  Changes to be committed:
    (use "git rm --cached <file>..." to unstage)
      new file:   lala.txt 
      
  * verde indica que esta area staging(area de preparación)
  
  Untracked files:
   (use "git add <file>..." to include in what will be committed)
      lolo.txt (rojo)

-------------------------------------------------------------------------
  //Ejemplo 2: Antes de hacer commit a un archivo se debe configurar usuario y correo
  
  $ git commit -m "primer commit"

  *** Please tell me who you are.

  Run

    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"

  to set your account's default identity.
  Omit --global to set the identity only in this repository.

  fatal: unable to auto-detect email address (got 'alumnos@MININT-ECUT0NC.(none)')

  * debemos configurar, se agrega correo y nombre

  git config --global user.email "susanavlr@live.cl"
  git config --global user.name "SL"

-------------------------------------------------------------------------
 // Ejemplo 3: Al hacer un cambio se puede ver el código de esta modificación
  
  $ git log
  commit fea3f370863e681efe9de680d1172bf9bce8999e (HEAD -> master) 

  * codigo que aparece es la clave del cambio que realicé se ve con  git show

  Author: SL <susanavlr@live.cl>
  Date:   Fri Feb 7 19:57:40 2020 -0300

      jscjndscjdjdcn
