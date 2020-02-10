# manual

pwd : indica cual es la carpeta actual donde estoy.

cd.. : sale de la carpeta

cd carpeta: entra en la carpeta

rm: borra un archivo

rm-rf carpeta: borrar una carpeta y todo su contenido

code . : abre visual studio

---------------------------------------------------------------
cd ~ // 

mkdir susana2 :creo un directorio

cd susana2 : ingreso a mi directorio

git init : inicializa un repositorio, se creará una carpeta llamada .git

touch   lala.txt : crear un archivo "lala.txt"

git status :verificar el estado de nuestro repositorio

* $ es el intermediario que recibe los comando

git add lala.txt : busca el archivo (si fuese . buscaria todos los archivos)

git commit : ahora el archivo lala.txt pasa de stageing al repositorio 

git diff : muestra las diferencias 

git checkout : actualiza las modificaciones 

git remote show origin : 

git push origin master : empuja el repositorio 

git fetch  : actualiza el repostorio local

git pull origin master  : actualiza directorio

git remote rm origin : remueve url de gitcd
 
-------------------------------------------------------------------------
  //Ejemplo 1
  
  $ git status
  On branch master 

  No commits yet

  Changes to be committed:
    (use "git rm --cached <file>..." to unstage)
          new file:   lala.txt *(verde indica que esta area stageing(area de preparación)
  
    *tomo el archivo de mi directory a esta zona

  Untracked files:
   (use "git add <file>..." to include in what will be committed)
          lolo.txt (rojo)

-------------------------------------------------------------------------
  //Ejemplo 2
  
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
 // Ejemplo 3
  
  $ git log
  commit fea3f370863e681efe9de680d1172bf9bce8999e (HEAD -> master) // codigo que aparece es la clave del cambio que realicé se ve con     git show
  Author: SL <susanavlr@live.cl>
  Date:   Fri Feb 7 19:57:40 2020 -0300

      jscjndscjdjdcn
