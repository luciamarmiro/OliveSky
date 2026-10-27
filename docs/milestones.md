# Milestone
A continuación se detalla de los milestrones establecidos, qué es lo que se pretende resolver, cómo se sabe que es válido y el soporte concreto que se va tener en cada uno de ellos.

## Milestone 0 - Establecimiento de límites atmosféricos
Relacionado con [HU001 - No saber si posponer o no la aplicación del plaguicida](historias_usuario.md#historia-de-usuario-1---no-saber-si-posponer-o-no-la-aplicación-del-plaguicida).

### ¿Qué necesidad hay que resolver?
Definición de las condiciones meteorológicas a seguir para garantizar la sostenibilidad del medio ambiente y la correcta distribución de un producto fitosanitario.

### ¿Cómo se hace la comprobación de que es válido?
Se parte de la HU001 y se crean issues vinculados a dicha historia de usuario para establecer los requerimientos necesarios para el establecimiento de los límites.
Cada vez que se resuelva un issue se actualizará su estado y se cerrará mediante commits. Una vez que dichos issues estén resueltos, se llevará a cabo su revisión y mediante la aprobación y fusión de Pull Request.
Una vez que se hayan definidos los límites atmosféricos, estos serán correctos si se ha fusionado el PR que verifica que dichos datos saldrán de la normativa del BOE,[Fuente 2 - Uso sostenible de los productos fitosanitarios](../README.md#cuáles-son-las-fuentes-de-datos).
Se reconocerá si es válido el entregable de este milestone, o no, dependiendo de si para llevarlo a cabo ha sido necesario un replanteamiento de la HU001. Si no ha sido necesario dicho replanteamiento el entregable será válido.


## Milestone 1 - Especificación y verificación de una ventana válida
Relacionado también con [HU001 - No saber si posponer o no la aplicación del plaguicida](historias_usuario.md#historia-de-usuario-1---no-saber-si-posponer-o-no-la-aplicación-del-plaguicida).

### ¿Qué necesidad hay que resolver?
Con el entregable del milestone 0, y para poder abordar a la pregunta de la HU001 que se plantea Paco es necesario establecer que es una ventana válida, ya que de la existencia o no de esta depende la aplicación o no del producto.

### ¿Cómo se hace la comprobación de que es válido?
Se parte del entregable en el milestone 0, y se continua trabajando con el establecimiento de issues, actualización de commits y aprobación mediante PR
Se establecerá como ventana válida aquella que corresponda a 6 intervalos de media hora continuos con condiciones meteorológicas pertenecientes a los límites. Se sabrá que una ventana válida es correcta mediante test, y se considerará correcta siempre que pase todos los test.
Se reconocerá si es válido o no, el entregable de este milestone dependiendo de si para llevarlo a cabo ha sido necesario un replanteamiento de la HU001 o del milestone 0. Será válido si no se ha llevado a cabo dicho replanteamiento de la HU001 y se ha podido trabajar a partir del entregable del milestone 0.