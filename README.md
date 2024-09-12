<p>Aquí escribiré mi trabajo para el tema 1 del curso de FullStack de Deusto Formación sobre el control de versiones de "Git"</p>

## Empezando con Git

  * Instalar Git Utilizando la terminal de comandos de ubuntu comandos de ubuntu:

    ```sh
    sudo apt-get install git
    ```
  * Empezar la configuración de git:

    ```sh
    git config --global user.email "correp-electronico"
    git config --global user.name "nombre-usuario"
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
