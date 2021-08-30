<img src="https://i.ibb.co/VM5MzBT/craftech-logo3.png=150x" width="250" height="250">

#### Prueba 2 - Despliegue de una aplicación Django y React.js

Elaborar el deployment dockerizado de una aplicación en django (backend) con frontend en React.js contenida en el repositorio. Es necesario desplegar todos los servicios en un solo docker-compose.

Se deben entregar los Dockerfiles pertinentes para elaborar el despliegue y justificar la forma en la que elabora el deployment (supervisor, scripts, docker-compose, kubernetes, etc)

Subir todo lo elaborado a un repositorio (github, gitlab, bitbucket, etc). En el repositorio se debe incluir el código de la aplicación y un archivo README.md con instrucciones detalladas para compilar y desplegar la aplicación, tanto en una PC local como en la nube (AWS o GCP).

Resolucion:

Para la resolucion de este ejersicio utilice una imagen base de python y resolvi las dependencias para la parte del back end. Para la parte del front utilice una imagen de node. Para orquestar todo use un docker compose creado los volumenes necesarios y el servidor de nginx.

Para deployar la aplicacion localmente se debe correr el comando de docker-compose up. En caso de querer correr la aplicacion en la nube se podrian tomar 2 caminos. El primero seria deployar la aplicacion en una virtual machine y levantarle de la misma manera con docker-compose y la segunda opcion seria usar kubernetes, en este caso se tomaria se buildea cada imagen y kubernetes la tomaria individualmente para crear los nodos dandole mayor escabilidad 

