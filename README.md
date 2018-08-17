# Notes js
Es un mini proyecto basado en los tutoriales de MitoCode.

La aplicación guarda/modifica/elimina y visualiza las notas que hayan sido agregadas.

## Tecnologías utilizadas
MongoDB, Node JS (Express), Bootstrap.

## Servidores para app y la DB
Heroku y mLab

## Como instalar
Primero debes contar con Node JS y Mongo DB Community Server instalados en tu computadora.

Ubícate en la carpeta raíz del proyecto y ejecuta el siguiente comando:
```
npm install
```
Una vez instaladas las dependencias crea una carpeta en el disco C llamada data y dentro que contenga otra carpeta llamada db.

Para estos pasos deberás tener las variables de entorno de Mongo DB.
Ejecuta en cmd:
```
mongod --dbpath C:/data/db
```

Luego de esto sin cerrar la terminal abre otra y ejecuta:
```
mongo
```

Listo, el motor de base de datos está listo, ahora solo necesitas ejecutar la aplicacion.
Ubícate en la carpeta del proyecto y ejecuta:
```
set DEBUG=myapp:* & npm start
```

## Heroku
[App en heroku](https://brayannotes.herokuapp.com/)

# Como subir una app a Heroku
Para poder subir a heroku una app se hace la ejecucion de los siguientes comandos:

1.- Entra en tu cuenta
```
heroku login
```

2.- Ubicate en la carpeta de tu proyecto y ejecuta:
```
git add .
```

3.- Agregas un commit a los cambios
```
git commit -m 'mLab'
```

4.- Crear la aplicacion en heroku con:
```
heroku apps:create [nombreDeLaApp]
```

5.- Subirlo a la rama
```
git push heroku master
```

6.- Para abrir la app ejecuta:
```
heroku open
```