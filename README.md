   --Aquí escribiré mi trabajo para el tema 1 del curso de FullStack de Deusto Formación sobre el control de versiones de "Git"

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
       <img src="Screenshots/Git Config.png" width="400" height="150">

## Empezando con Git

  * Abriremos nuestro editor de codigo:

    ```sh
    code
    ```
 * Empezaremos creando nuestro HTML, al finalizarlo deberemos inicializar nuestro control de versiones de Git (Podremos utilizar la propia terminal de Visual Studio Code <Ctrl + `>):

   ```sh
   git init
    ```
   (Por defecto nos creara la rama principal con el nobre "master")-(Se podra cambiar con el comando):

   ```sh
   git branch -m <nombre-rama>
   ```

 * Podemos ver todos los cambios desde la zona interactiva de Visual Studio Code en el lateral izauierdo llamada source control.

   
 * Una vez creada la rama principal, necesitaremos añadir los archivos que hemos creado utilizando el comando:

   ```sh
   git add <nombre-de-archivo>
   ```
   (En el caso que queramos que se nos añadan todos los nuevos archivos, utilizaremos el comando):

   ```sh
   git add -A
   ```
 * Continuaremos con el comando "commit", sera indispensable comentar el commit para continuar, además, de ser una buena practica para la correcta documentación de nuestro desarrollo sobre el repositorio:

   ```sh
   git commit -m <comentario-sobre-el-commit>
   ```
* Una vez realizado el commit podremos publicar nuestro primer repositorio en GitHub, para ello necesitaremos una cuenta en GitHub y vincularla con Visual Studio Code.
