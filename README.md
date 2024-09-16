--Aquí escribiré mi aprendizaje del curso de FullStack de Deusto Formación sobre el control de versiones de "Git"

## Instalación y configuración de Git

 * Instalar Git Utilizando la terminal de comandos de ubuntu:

    ```sh
    sudo apt-get install git
    ```
 * Empezar la configuración de git:

    ```sh
    git config --global user.email <"correp-electronico">
    git config --global user.name <"nombre-usuario">
    ```
 * Podemos abrir el archivo de configuración una vez terminado el paso anterior con el siguiente comando:

    ```sh
    git config --global -e
    ```
 * Podemos tambien establecer nuestro editor de codigo por defecto (en mi caso elegí Visual estudio code) añadiendo la siguiente linea de comando o escribiendo en el documento que acabamos de abrir:

    ```sh
    git config --global core.editor "code"
    ```
    <img src="/Screenshots/Git Config.png" width="400" height="150">

## Empezando con Git

  * Abriremos nuestro editor de codigo:

    ```sh
    code
    ```
    <img src="/Screenshots/Main Visual Studio Code.png" width="1000" height="600">
 * Empezaremos creando nuestro HTML, al finalizarlo deberemos inicializar nuestro control de versiones de Git (Podremos utilizar la propia terminal de Visual Studio Code <Ctrl + `>):

   ```sh
   git init
    ```
   (Por defecto nos creara la rama principal con el nobre "master")-(Se podra cambiar con el comando):

   ```sh
   git branch -m <nombre-rama>
   ```
   <img src="/Screenshots/Git init next.png" width="1000" height="600">
 * Podemos ver todos los cambios desde la zona interactiva de Visual Studio Code en el lateral izquierdo, llamada source control.

   <img src="/Screenshots/Source control Visual Studio Code.png" width="110" height="110">
   
 * Una vez creada la rama principal, necesitaremos añadir los archivos que hemos creado utilizando el comando:

   ```sh
   git add <nombre-de-archivo>
   ```
   (En el caso que queramos que se nos añadan todos los nuevos archivos, utilizaremos el comando):

   ```sh
   git add -A
   ```
   O
   ```sh
   git add --a
   ```
 * Continuaremos con el comando "commit", sera indispensable comentar el commit para continuar, además, de ser una buena practica para la correcta documentación de nuestro desarrollo sobre el repositorio:

   ```sh
   git commit -m <comentario-sobre-el-commit>
   ```
    <img src="/Screenshots/First git add and commit.png" width="720" height="220">
 * Una vez realizado el commit podremos publicar nuestro primer repositorio en GitHub, para ello necesitaremos una cuenta en GitHub y vincularla con Visual Studio Code.

    <img src="/Screenshots/Publish Visual Studio Code.png" width="250" height="45">

## Fetch, Merge y Pull

 * Una vez crado el repositorio de GitHub podremos provar 3 nuevas funciones. Que serán:

    (El comando "fetch" nos permitira descargar los cambios realizados del repositorio remoto al local, dandonos una comparación sobre los cambios).
    ```sh
    git fetch
    ```
      <img src="/Screenshots/Git fetch changes.png" width="1000" height="600">
    
    (El comando "merge" fusionara los cambios descargados por el comando "fetch" al repositorio local).<br>
    !!! El comando "merge" tambien lo veremos en otro caso más adelante !!!
    ```sh
    git merge
    ```
      <img src="/Screenshots/Git merge terminal.png" width="720" height="220">

    (El comando "pull" realizara la función de el comando "fetch y "merge" al mismo tiempo. Esta acción puede llevar a que el repositorio local entre en conflicto con los cambios realizados).
    ```sh
    git pull
    ```
      <img src="/Screenshots/Git push terminal.png" width="720" height="280">
    
    Esta sería la cadena de comandos que deberemos seguir para añadir unas imagenes al repositorio remoto.

## Git Remote

  * Al trabajar con repositorios remotos sera indispensable saber utilizar las funcionalidades del comando git remote.

    ```sh
    git remote
    ```
      <img src="/Screenshots/Git remote terminal.png" width="720" height="100">

    (Al utilizar este comando nos mostrara los nombres de los repositorios remotos creados, por defecto el nombre del repositorio por defecto es el de "origin").
    ```sh
    git remote -v
    ```
      <img src="/Screenshots/Git remote v terminal.png" width="720" height="100">

    (Este comando nos permitira ver las urls asociadas a los repositorios remotos)
    ```sh
    git remote add <nombre-repositorio> <Url>
    ```
      <img src="/Screenshots/Git remote add terminal.png" width="1000" height="220">

    (Este comando nos permitira añadir y nombrar un nuevo repositorio remoto, para ello sera necesario un nomre y una url).
    ```sh
    git remote rename <nombre-repositorio> <nuevo-nombre-repositorio>
    ```
      <img src="/Screenshots/Git remote rename terminal.png" width="1000" height="220">

    (Este comando nos permitira cambiar el nombre del repositorio).
    ```sh
    git remote remove <nombre-repositorio>
    ```
      <img src="/Screenshots/Git remote remove terminal.png" width="1000" height="150">
    
    (Este comando nos permitira eliminar el repositorio remoto).
