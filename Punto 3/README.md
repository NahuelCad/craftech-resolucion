<img src="https://i.ibb.co/VM5MzBT/craftech-logo3.png=150x" width="250" height="250">

#### Prueba 3 - CI/CD

Dockerizar un nginx con el index.html default.
Elaborar un pipeline que ante cada cambio realizado sobre el index.html buildee la nueva imagen y la actualize en la plataforma elegida. (docker-compose, swarm, kuberenetes, etc.)
Para la creacion del CI/CD se puede utilizar cualquier plataforma (CircleCI, Gitlab, Github, Bitbucket.)

Resolucion:

Para la resolucion de esta prueba utilice una imagen de nginx como base y para el ci/cd utilice Github actions, el pipeline al ver un nuevo cambio en el codigo buildea la imagen y 
la sube a docker hub para que desde ahi se pueda deployar por ejemplo a en la plataforma de azure a app engine, el cual al detectar una nueva imagen vuelve a deployar.

