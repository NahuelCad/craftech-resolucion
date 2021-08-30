<img src="https://i.ibb.co/VM5MzBT/craftech-logo3.png=150x" width="250" height="250">

#### Prueba 1 - Diagrama de Red

Produzca un diagrama de red (puede utilizar lucidchart) de una aplicación web en GCP o AWS y escriba una descripción de texto de 1/2 a 1 página de sus elecciones y arquitectura.

El diseño debe soportar:

Cargas variables
Contar con HA (alta disponibilidad)
Frontend en Js
Backend con una base de datos relacional y una no relacional
La aplicación backend consume 2 microservicios externos
El diagrama debe hacer un mejor uso de las soluciones distribuidas.


Resolucion:


<img src="https://i.ibb.co/CQs6SZR/infra.jpg" width="250" height="250">

Para la resolucion del diseño propuesto utilice la plataforma en la nube de google (GCP)
Debido a la necesidad de soportar cargas variables y tener alta disponibilidad base el diseño en la utulizacion de kubernetes para el frontend y el backend. De esa manera se podra tener gran cantidad de nodos y en caso de que alguno falle se recreara de inmediato. Tambien debido a la gran cantidad de carga que en teoria va a sufrir la aplicacion se necesita la utilizacion de un balanceador de carga que distribuya las llamadas de manera correcta.
 Para la necesidad de tener una bse de datos relacional elegi cloud spanner ya que es una base de datos relacional que proporcional gran escabilidad horizontal y una disponibilidad de un 99,99% cumpliendo con el pedido de la alta disponibilidad. Para el caso de la base de datos no relacional seleccione BigTable ya que por lo mencionado se supongo que va se va a necesitar una gran capacidad de procesamiento de informacion y una gran escalabilidad, y ya que no se menciona que datos se van a tener que guardar en la base de datos no relacional (lo que a veces puede generar restricciones en las elecciones) creo que es la mas adecuada



