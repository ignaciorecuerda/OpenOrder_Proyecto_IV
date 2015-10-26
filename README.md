# Proyecto OpenOrder IV

#Primer hito
##Integrantes del proyecto
Este repositorio es de **Jose Ignacio Recuerda Cambil**, aunque el grupo esta formado también por:
- Antonio Miguel Pozo Cámara
- Ignacio Romero Cabrerizo

##Breve descripción del proyecto OpenOrder
Este proyecto llevará la gestión de pedidos de una pequeña o mediana empresa mediante una aplicación cliente-servidor. La API del servidor hará de intermediario entre 2 clientes (comercio y usuario) con posibilidad de notificaciones push en ellas. El usuario podrá realizar un pedido directamente a través de la aplicación. La parte del comercio será notificado de los pedidos realizados por los clientes, agilizando el proceso de comunicación entre ambas partes.

##Descripción de este respositorio
Este repositorio se encargará del desarrollo de la app que se comunicará con el servidor mediante peticiones y respuestas en JSON con la API. La aplicación recibirá la respuestas JSON y se encargará de notificar a ambos usuarios del estado del pedido (nombre, descripción del pedido, unidades, precio...). Con esto se llevará a cabo la comunicación cliente-servidor, para asi poder realizar los pedidos en tiempo real.

##Tecnologías a usar
Las principales serán: 
 - Android Studio
 - sqlitebrowser
 - Azure
 - Nodejs
 - y alguna más que se necesite.


#Segundo hito
##Sistema de test
Como sistema de test he usado moncha, ya que lo conocia de haberlo usado para uno de los ejercicios del tema.
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