
# Pasos para hacer un Fork en github

##
Que es un fork.

Un fork es una copia exacta, hecha en tu cuenta de github, de un repositorio en github que por lo general no es tuyo. Es decir, en github tu puedes ir a un repositorio y hacer click en el boton Fork y al hacer click en este github te preguntara por tus propias credenciales de github para poder hacer una copia de dicho repositorio en tu propia cuenta.

1.- Ir al repositorio de la cuenta en git en donde quieres contribuir. Si es un repositorio publico pues solo hay que ir alla y dar click sobre este y logearte con tu cuenta y usuario y una copia (fork) se creara en tu cuenta de usuario.

Por otra parte si el repositorio de la cuenta en la cual quieres contribuir es privado, entonces el propietario de ese repositorio debera de agregarte como un usuario colaborador. Y entonces podras tener acceso a dicho repositorio y hacer el fork.

2.- Clonar el repositorio desde tu cuenta github, recuerda que vas a clonar el fork que esta en tu cuenta y no el del repositorio original. Pues solo podras hacer push de un repositorio que radica en tu cuenta y no en la cuenta de otra persona.
  
  Crear un directorio en tu computadora
  $ mkdir nombreProyecto
  $ git clone https://github.com/nombre/nombreProyecto.git // El de tu propio fork.

3.- Instalar las dependencias del proyecto en tu computadora.
    
    ----------------------------------------------------------------
    Si el proyecto es de Javascript o si estas trabajando con laravel/mix entoneces:
    $ npm i
    $ npm audit fix
    $ npm audit fix -force
    $ npm run bundle
    $ npm run build //
    Nota: O npm run build-demo si es que existe y entrar en el directorio del demo.
    $ live-server // corre el servidor de desarrollo.

    ----------------------------------------------------------------
    Si el proyecto esta en php o laravel
    1.- $ composer install

    2.- Hacer copia del archivo env_example y renombrarlo como .env
        Cambiar el DB_DATABASE y el DB_USERNAME y el DB_PASSWD al the Xampp local.
        O en caso de que se use un servidor de desarrollo pedir estos datos.
    3. Crear la base de datos en phpMyAdmin.
    
    4.- $ php artisan key:generate // Genera la llave a usar en APP_KEY del archivo .env

    5.- $ php artisan migrate // Para realizar las migraciones.

Si en tu proyecto utilizas redes sociales para logearte entonces tienes que copiar
las credenciales tambien aqui al final del archivo .env

----------------------------------------------------------------

Esto es la recomendacion de un repositorio.

1.- Fork it!
2.- Create your feature branch: git checkout -b my-new-feature
3.- Commit your changes: git commit -am 'Add some feature'
4.- Push to the branch: git push origin my-new-feature
5.- Submit a pull request :D



    




