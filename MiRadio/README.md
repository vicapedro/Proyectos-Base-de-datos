# MyBeat - Música con tu estilo
## Proyecto de Base de datos

### ¿Qué es MyBeat?
MyBeat es una empresa que ofrece servicios de música en línea. Los usuarios pueden escuchar música, crear listas de reproducción, seguir a otros usuarios y artistas, y recibir recomendaciones personalizadas. Los artistas pueden subir su música, crear listas de reproducción y ver estadísticas de reproducción.

### ¿Qué necesito?
Un sistema que me permita:
- Registrar a los usuarios y artistas.
- Guardar la música y las listas de reproducción.
- Llevar un control de las reproducciones.
- Mostrar recomendaciones personalizadas.
- Mostrar estadísticas de reproducción a los artistas.
- Determinar las regalias de los artistas.

### Las canciones
Cada canción tiene un nombre, un género, un año de lanzamiento y uno o mas autores, cada uno con diferente rol: Letrista (el que escribe la letra) o Compositor ( de la música). Estos autores son los que tienen los derechos de autor de la canción.

Un intérprete puede grabar una versión de una canción. Un intérprete puede ser un cantante o un grupo musical.

Cada versión tiene una letra y un archivo de audio asociado.


### Los artistas
Cada artista tiene un nombre, una biografía, una foto de perfil y un género musical principal. También necesito saber cuántas canciones ha subido, cuántas reproducciones tienen en total y cuántos seguidores tienen. Los artistas pueden seguir a otros artistas.

Un artista puede ser cantante, compositor, productor, etc. y necesito saber cuál es su rol en cada canción. 

### Las listas de reproducción
Cada lista de reproducción tiene un nombre, una descripción y un usuario creador. También necesito saber cuántas canciones tiene y cuántas veces se ha reproducido. Las listas de reproducción pueden ser públicas o privadas, y los usuarios pueden seguir las listas de otros usuarios.

### Los álbumes
Cada álbum tiene un nombre, un año de lanzamiento y un artista. También necesito saber cuántas y cuales canciones tiene y cuántas veces se ha reproducido. Los álbumes pueden tener un género musical y una portada. Los álbumes pueden ser de un solo artista o de varios artistas.

### Los usuarios 
Cada usuario tiene un nombre, un correo electrónico, una contraseña, una fecha de nacimiento y una foto de perfil. También necesito saber cuántas canciones ha subido, cuántas listas de reproducción ha creado, cuántas canciones ha escuchado y cuántas veces ha escuchado cada canción. Los usuarios pueden seguir a otros usuarios y a artistas.


# Inconsistencias o imprecisiones
## Derechos de autor y regalías:

No se especifica cómo se gestionan los derechos de autor de las canciones. Por ejemplo, si una canción tiene múltiples autores (letristas y compositores), ¿cómo se dividen las regalías entre ellos?

Falta claridad sobre cómo se calculan las regalías para los artistas. ¿Se basa en las reproducciones, descargas, o ambos? ¿Cómo se manejan las regalías para canciones con múltiples intérpretes o colaboraciones?

## Roles de los artistas:


No se aclara si un artista puede tener múltiples roles en una misma canción (por ejemplo, ser cantante y compositor a la vez).

## Versiones de canciones:

Se menciona que un intérprete puede grabar una versión de una canción, pero no se especifica cómo se relaciona esta versión con la canción original. ¿La versión tiene su propio identificador único? ¿Cómo se manejan los derechos de autor de la versión?

No se aclara si una versión puede tener múltiples intérpretes (por ejemplo, un dúo o un grupo).

## Álbumes:

No se especifica si un álbum puede tener canciones de múltiples artistas (colaboraciones). Si es así, ¿cómo se manejan los créditos y las regalías?

No se menciona si un álbum puede pertenecer a un sello discográfico o si tiene un identificador único (como un código ISRC o UPC).

## Listas de reproducción:

No se especifica si una lista de reproducción puede tener canciones de múltiples artistas o álbumes.

No se aclara si las listas de reproducción pueden tener un orden específico de canciones o si son simplemente una colección sin orden.

## Estadísticas de reproducción:

No se especifica cómo se registran las reproducciones. ¿Se cuentan por usuario, por dispositivo, o por sesión? ¿Se almacena la fecha y hora de cada reproducción?

No se menciona si las estadísticas de reproducción incluyen métricas como la duración de la reproducción o si la canción se escuchó completa.

## Recomendaciones personalizadas:

No se explica cómo se generan las recomendaciones personalizadas. ¿Se basan en el historial de reproducciones, los géneros favoritos, o las listas de reproducción seguidas?

No se menciona si se utilizará un algoritmo de recomendación basado en machine learning o si será algo más simple, como sugerir canciones populares.

## Contratos de artistas:

No se especifica si los contratos tienen cláusulas adicionales, como exclusividad, duración mínima, o condiciones de renovación.

No se aclara cómo se manejan los contratos para grupos musicales. ¿Cada miembro del grupo tiene un contrato individual o hay un contrato grupal?

## Usuarios:

No se menciona si los usuarios pueden tener roles adicionales, como administradores o moderadores, que podrían necesitar permisos especiales en la plataforma.

No se especifica cómo se manejarán las contraseñas (por ejemplo, si se almacenarán encriptadas).

Normalización de la base de datos:

No se menciona cómo se normalizarán las tablas para evitar redundancias. Por ejemplo, ¿habrá una tabla separada para los géneros musicales, o se repetirá el género en cada canción o álbum?

No se especifica cómo se manejarán las relaciones muchos-a-muchos, como artistas que colaboran en múltiples canciones o usuarios que siguen a múltiples artistas.

Sugerencias de mejora
Tablas adicionales:

Crear una tabla para roles de artistas (cantante, compositor, productor, etc.) y relacionarla con las canciones.

Crear una tabla para derechos de autor, donde se registren los porcentajes de regalías para cada autor (letrista, compositor) e intérprete.

Crear una tabla para versiones de canciones, con atributos como el identificador de la versión, los intérpretes y la fecha de grabación.

Atributos adicionales:

Agregar un identificador único para cada canción, álbum y lista de reproducción (por ejemplo, un código ISRC para canciones o un UUID para listas).

Agregar atributos como duración para las canciones y fecha de creación para las listas de reproducción.

Relaciones muchos-a-muchos:

Implementar tablas intermedias para manejar relaciones como:

Artistas que colaboran en canciones.

Canciones que pertenecen a múltiples álbumes (por ejemplo, reediciones o compilaciones).

Usuarios que siguen a múltiples artistas y listas de reproducción.

Estadísticas detalladas:

Registrar métricas adicionales, como la fecha y hora de cada reproducción, la duración escuchada, y el dispositivo utilizado.

Crear una tabla para historial de reproducciones, donde se almacene esta información.

Recomendaciones personalizadas:

Implementar un sistema de recomendación basado en el historial de reproducciones, los géneros favoritos y las listas de reproducción seguidas.

Considerar el uso de algoritmos de machine learning para mejorar la precisión de las recomendaciones.

## Seguridad:

Asegurar que las contraseñas de los usuarios se almacenen encriptadas (por ejemplo, usando hash y salt).

Implementar medidas de seguridad para proteger los datos de los usuarios y artistas.

