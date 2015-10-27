# Proyecto OpenOrder IV

#Primer hito
##Integrantes del proyecto
Este repositorio es de **Jose Ignacio Recuerda Cambil**, aunque el grupo esta formado también por:
- Antonio Miguel Pozo Cámara
- Ignacio Romero Cabrerizo

##Breve descripción del proyecto OpenOrder
Este proyecto llevará la gestión de pedidos de una pequeña o mediana empresa mediante una aplicación cliente-servidor. La API del servidor se encargará de permitir al usuario hacer pedidos y que todo ellos queden registrados en una Base de datos. 

##Descripción de este repositorio
Este repositorio se encargará de la gestión de los pedidos que los usuarios harán a la empresa. Almacenará en una base de datos todos los datos necesarios tanto del cliente como del producto que se está solicitando.

##Servicios necesarios
En principio será necesario un servicio de base de datos de SQL para poder almacenar y gestionar tanto los pedidos como los datos del usuario que los solicita.

##Este proyecto se ha inscrito en el certamen de proyectos libres de la UGR.

#Segundo hito
##Sistema de test
Como sistema de test he usado moncha, ya que lo conocia de haberlo usado para uno de los ejercicios del tema.
Empiezo instalando moncha con el comando "sudo npm install -g mocha" .Creo un directorio con el nombre "test" y dentro de este el archivo que se encargará de comprobar que la aplicación carga correctamente.
El contenido de test.js es el siguiente:

![test.js](https://www.dropbox.com/s/zyxh53hsaij1pmi/hito2.4.png?dl=1)

Finalmente lo ejecuto con el comando "mocha test/test.js"

Por ahora solo he realizado una comprobación para que no se puede introducir un nombre con menos de 3 caracteres para ser añadido. En un futuro se añadiran más test a la aplicación. Aquí se puede ver el código:

![.travis.yml](https://www.dropbox.com/s/8qtl4jypm9t3vq7/hito2.3.png?dl=1)


##Integración continua
Para la integración continua de mi proyecto he usado [Travis](https://travis-ci.org).

Para empezar tenemos que registrarnos en la página desde el mismo git. Le damos permisos para que pueda acceder a nuestros proyectos de git y así lanzar la aplicación.
Una vez hecho esto creo el fichero llamado ".travis.yml" y lo añado a la carpeta raiz del repositorio.

El fichero contiene lo siguiente:

![.travis.yml](https://www.dropbox.com/s/556agqlr8n9figk/hito2.1.png?dl=1)

Seguidamente inicio el test al repositorio de la aplicación y lo realiza correctamente como podemos ver en la siguiente captura:

![build passing](https://www.dropbox.com/s/swj3hbol024xu7m/hito2.2.png?dl=1)