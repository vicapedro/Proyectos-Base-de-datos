## Pokémon Go

Es un juego que usted quiere diseñar. La idea es que va recolectando pokemones que se encuentra en el camino. 

Cada pokémon puede ser de una especie, por ejemplo: Pika, Chorrito, Rocacho, Dormilón, etc. 
Cada especie es de 1 o 2 tipos, por ejemplo: Agua, fuego, planta, psiquico, etc. 

Cada especie de pokemon tiene valores diferentes para algunas características: Poder de Combate máximo, puntos de salud, poder de defensa, poder de Ataque. 

Cada especie puede aprender un conjunto de diferentes ataques de diferente tipo: Trueno tipo eléctrico, Chorro tipo Agua, etc. 

Los ataques pueden ser o rápidos o cargados. Los ataques rápidos se pueden realizar rápidamente uno tras otro y cada vez van acumulando energía para poder realizar el ataque cargado.

Cada bicho puede aprender un ataque rápido y un ataque cargado.

Cada especie es mas o menos resistente a ataques de cierto tipo de pokémon: Los tipo Planta resisten los ataques tipo agua, pero no los tipo Fuego. 

Ejemplo:

**Anihilape**

| **Debilidades** | **Factor** |
|-------------|--------|
| Hada | 160% |
| Volador| 160% |
| Fantasma| 160% |
| Psíquico| 160% |
| **Resistencias** |**Factor** |
|Bicho|39%|
|Lucha|39%|
|Normal| 39% |
|Veneno| 62% |
|Roca| 62% |


Cada especie puede evolucionar en otra especie de bicho, teniendo un árbol de evoluciones posibles. En la evolución algunos atributos pueden variar, incluidos los ataques que sabe.

Los usuarios pueden recolectar varios bichos, incluso de la misma especie, cada uno con sus propios valores de los diferentes atributos. Los bichos pueden intercambiarse entre los usuarios. El usuario puede deshacerse de cualquier bicho. El bicho puede ser transferido (se pierde) o liberado en la ubicación actual del usuario(disponible durante 10 minutos para que otro usuario lo encuentre y trate de capturarlo). Un bicho tiene un UUID con el cual se le puede dar seguimiento durante su tiempo de vida. 

Un usuario puede capturar cualquier bicho que aparezca en un radio de 50m.

El sistema genera los bichos en un radio de 50m de la ubicación de un usuario. El *spawn* está influenciado por: tiempo climático, si hay nido, región, hora del dia, estado del clima. Un mismo bicho no puede ser capturado por dos usuarios, aunque si pueden intentar hacerlo al mismo tiempo (*transacciones y bloqueo de recursos*). Un bicho permanece en el mismo lugar de su *spawn* por 10 minutos.

Por lo pronto, el sistema cambia el tiempo climático por zonas cada hora.

Una región abarca una gran área geográfica: Norteamérica, Sudamérica, Europa, Asia, Norte de África, etc.

Un usuario puede organizar combates contra otro para lo cual escoge a 3 de sus bichos. Los bichos se enfrentan uno a uno contra los del contrincante realizando un serie de ataques entre si hasta que uno de los dos queda sin puntos de salud. Luego pueden enfrentarse cualesquiera otros dos bichos de los equipos en combate.

Cuando un pokémon es capturado proporciona cierta cantidad de caramelos de la especie base de la cadena evolutiva.

Cada especie requiere cierta cantidad de caramelos para llegar a ella de la especie anterior en la cadena evolutiva. 

Los caramelos se utilizan para aumentar el Poder de Combate de un pokémon.
Se debe llevar el registro de cuantos caramelos de cada especie tiene un entrenador. 

El sistema debe llevar registro de la ubicación donde se recolectó cada bicho y la propiedad de los usuarios, así como las estadísticas de combate. 


Amplíe este escenario para hacer mas completo el juego, de tal forma que cambie la estructura de la base de datos: Pokeparadas, Gimnasios, Nidos, etc. 

## Pendientes
- Como se calcula el daño en combate
