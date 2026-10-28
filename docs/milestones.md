# Milestone
A continuación se detalla de los milestones establecidos, qué es lo que se pretende resolver, cómo se sabe que es válido y el soporte concreto que se va tener en cada uno de ellos.

## Milestone 0 - Modelo de dominio
Relacionado con [HU001 - No saber si posponer o no la aplicación del plaguicida](historias_usuario.md#historia-de-usuario-1---no-saber-si-posponer-o-no-la-aplicación-del-plaguicida).

### ¿Qué necesidad hay que resolver?
Es necesario saber cuáles son los elementos del problema que forman parte de la decisión de Paco para llegar a generar una respuesta de si se aplaza o no el uso del producto, es decir, se requiere un modelo de domino; representaciones y relaciones de los componenetes claves de la HU001.
Es un requerimiento conocer las condiciones meteorológicas a seguir para garantizar la sostenibilidad del medio ambiente y la correcta distribución de un producto fitosanitario.
Existe la necesidad de conocer los datos atmosféricos que se dan en una población dada una semana en periodos semihorarios. Dichas lecturas semihorarias serán un intervalo si cumplem los límites atmosféricos establecidos. 

### ¿Cómo se hace la comprobación de que es válido?
Se parte de la HU001 y se crean issues vinculados a dicha historia de usuario para establecer la representación de los elementos del problema, límites, lecturas e intervalos, los requerimientos necesarios para sus relaciones.
Cada vez que se resuelva un issue se actualizará su estado y se cerrará mediante commits. Una vez que dichos issues estén resueltos, se llevará a cabo su revisión mediante la aprobación y fusión de Pull Request.
Una vez que se hayan definidos los límites atmosféricos, estos serán correctos si se ha fusionado el PR que verifica que dichos datos se han obtenido de la normativa del BOE,[Fuente 2 - Uso sostenible de los productos fitosanitarios](../README.md#cuáles-son-las-fuentes-de-datos).
Lo mismo ocurre para las lecturas, estas seran correctas si se ha fusionado el PR que verifica que dichos datos se han obtenido adecuadamente de la población de Baza, [Fuente 1 - Consulta datos SiAR Baza](../README.md#cuáles-son-las-fuentes-de-datos).
Se reconocerá si es válido el entregable de este milestone, o no, dependiendo de si para llevarlo a cabo ha sido necesario un replanteamiento de la HU001. Si no ha sido necesario dicho replanteamiento el entregable será válido.


## Milestone 1 - Especificación y verificación de una ventana válida
Relacionado también con [HU001 - No saber si posponer o no la aplicación del plaguicida](historias_usuario.md#historia-de-usuario-1---no-saber-si-posponer-o-no-la-aplicación-del-plaguicida).

### ¿Qué necesidad hay que resolver?
Con el entregable del milestone 0, y para poder responder a la pregunta de la HU001 que se plantea Paco es necesario establecer que es una ventana válida, ya que de la existencia o no de esta depende la aplicación o no del producto.

### ¿Cómo se hace la comprobación de que es válido?
Se parte del entregable en el milestone 0, y se continua trabajando con el establecimiento de issues, actualización de commits y aprobación mediante PR.
Se establecerá como ventana válida aquella que corresponda a 6 intervalos de media hora continuos (las condiciones meteorológicas ya se encuentran dentro de los límites, por la propia definición de intervalo que se ha tomado en el milestone 0). 
Se sabrá que una ventana válida es correcta mediante tests, y se considerará correcta siempre que pase todos los tests.
Se reconocerá si es válido o no el entregable de este milestone dependiendo de si para llevarlo a cabo ha sido necesario un replanteamiento de la HU001 o del milestone 0. Será válido si no se ha llevado a cabo dicho replanteamiento de la HU001 y se ha podido trabajar a partir del entregable del milestone 0.