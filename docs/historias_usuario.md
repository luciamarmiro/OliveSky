# Historias de usuario
En este documento se explicarán con más detalle las historias de usuario HU001 y HU002.

## Historia de usuario 1 - No saber si posponer o no la aplicación del plaguicida
### ¿A quién afecta y por qué?
Afecta a [Paco](personas.md#paco-70-años-prejubilado), porque él en la campaña pasada decidió no posponer el uso del producto y lo aplicó una semana en la cual las condiciones meteorológicas no eran las recomendadas por las buenas prácticas. Dando lugar a la evaporación del plaguicida en sus plantaciones de almendro, afectando a su cosecha tanto de almendro como de olivo.

### ¿Cuál es el problema?
Cada día Paco debe consultar manualmente el tiempo durante la semana, lo cuál requiere tiempo, ya que puede que necesite consultar más de una página web.
Del mismo modo, Paco debe retener dichos días y horas que él cree que pueden ser los más adecuados y hacer otra comprobación de si los valores más relevantes para la correcta uniformidad del producto están dentro de los límites; esto también requiere tiempo y supone una carga mental. 
Decidiendo la aplicación o no del producto con cierto riesgo de ser al azar o subjetiva por miedo a la no existencia de condiciones meteorológicas válidas en el futuro.

### Datos que intervienen
- [Fuente 2 - Límites establecidos por las buenas prácticas de aplicación de productos fitosanitarios](../README.md#cuáles-son-las-fuentes-de-datos)
- [Fuente 1 - Condiciones meteorológicas de Baza](../README.md#cuáles-son-las-fuentes-de-datos)
Esta fuente de datos del SiAR proporciona un histórico de las condiciones meteorológicas de semanas y campañas anteriores, por lo que para poder proporcionarle una respuesta a  Paco es necesario que se trabaje con las semanas anteriores a dicha semana por la que pregunta (por ejemplo, dos semanas anteriores).
Así, sabríamos cuáles son las condiciones meteorológicas más características de dichas semanas (si predominan las altas temperaturas, la velocidad del viento es nula, etc) y se compararán con las semanas de las campañas anteriores para ver cuál o cuáles se le asemejan. Así se usaría eficazmente el histórico, ya que se buscarán ventanas válidas en la semana de la campaña anterior más parecida a nivel meteorológico y no se estaría comparando con una campaña anterior cualquiera. 


### ¿Cómo saber si es correcto lo que devuelve OliveSky?
Si devuelve su aplicación, verificando la existencia de una ventana válida en la cuál se cumplan las condiciones meteorológicas dentro de los límites de las buenas prácticas en la semana más parecida de anteriores campañas.
Si devuelve su aplazamiento, verificando la no existencia de dicha ventana válida.


## Historia de usuario 2 - Existe de verdad ventana válida dado un fin de semana
### ¿A quién afecta y por qué?
Afecta a [Carla](personas.md#carla-37-años-madre-de-familia), porque quiere evitar desplazamientos innecesarios a Baza, ya que se debe organizar durante la semana para ello.


### ¿Cuál es el problema?
Carla no sabe qué fines de semana es más adecuado echar el plaguicida según las condiciones meteorológicas. 
Planificarse con antelación durante la semana para poder ir un fin de semana a echar el plaguicida requiere consultar las condiciones meteorológicas continuamente para esas fechas específicas por si ha habido algún cambio desde la última vez que lo consultó, esto también le supone a Carla tiempo continuamente.
Además, necesita saber si en esos días, además de las condiciones adecuadas, dispondría de las horas suficientes que le supone echar el plaguicida, para no empezar una dosis y dejarla a medias, ya que si vuelve a tardar mucho en ir, la exposición al aire puede hacer que pierda parte de su eficacia.

### Datos que intervienen
- [Fuente 1 - Condiciones meteorológicas a nivel semanal de Baza](../README.md#cuáles-son-las-fuentes-de-datos)
- [Fuente 2 - Límites establecidos por las buenas prácticas de aplicación de productos fitosanitarios](../README.md#cuáles-son-las-fuentes-de-datos)

### ¿Cómo saber si es correcto lo que devuelve OliveSky?
Si el resultado es el de aplicar esa semana el plaguicida, la ventana válida cumple con el requisito de los 6 intervalos de media hora continuos en los cuáles las condiciones meteorológicas están dentro de los límites, y dicha ventana válida debe aparece más de una vez durante el fin de semana para garantizar el margen de aplicación.