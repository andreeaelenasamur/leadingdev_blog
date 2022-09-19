# Antes de arrancar el proyecto

Esta guía contempla la preparación del entorno en un sistema operativo Linux. Para la instalación en otros sistemas operativos consulte la siguiente guía: https://guides.rubyonrails.org/getting_started.html#creating-a-new-rails-project

### Preparación del entorno

1. Instalación de Ruby: ejecutar el comando `sudo apt install ruby-full`. Una vez finalizado, comprobar que se ha instalado correctamente usando el comando `ruby --version`.

2. Instalación de sqlite3: ejecutar el comando `sudo apt install sqlite3`. Una vez finalizado, comprobar que se ha instalado correctamente usando el comando `sqlite3 --version`.

3. Instalación de rails: ejecutar el comando `sudo gem install rails`. Una vez finalizado, comprobar que se ha instalado correctamente usando el comando `rails --version`.

Si todo ha funcionado correctamente, podemos seguir al siguiente paso.

### ¿En que consiste el proyecto?

Este proyecto consiste en la creación de un blog básico el cual tiene distintas vistas que nos permiten crear artículos y comentarios dentro de los mismos. También permite la edición de artículo así como el borrado de artículos y comentarios.

Incorpora, para poder realizar estas tareas, un sistema de autenticación básico. Las credenciales de prueba son: 

* usuario: admin
* contraseña: 123456

### Arrancar el proyecto

1. Abrimos una nueva terminal y vamos al directorio raíz de este proyecto.

2. Para instalar las dependencias del proyecto ejecutamos el comando: `./bin/bundle install`.

3. Ejecutamos las migraciones para inicializar la base de datos con el siguiente comando: `./bin/rails db:migrate RAILS_ENV=development`.

4. Por último, lanzamos la aplicación en el equipo local con el siguiente comando: `./bin/rails server`.

### Base de datos

Para esta prueba técnica hemos usado una base de datos local sqlite3. Tras ejecutar las migraciones (paso 3 del apartado anterior), tendremos el fichero db/development.sqlite3 que almacena la estructura y datos del proyecto.
Para visualizar los datos de una forma intuitiva, podemos subir dicho archivo en la siguiente plataforma: https://inloop.github.io/sqlite-viewer/

### Estilos

Para esta prueba hemos incorporado el framework Boostrap en su versión 5.X.
