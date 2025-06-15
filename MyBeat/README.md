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
Cada obra tiene un nombre, un género, un año de lanzamiento y uno o mas autores, cada uno con diferente rol: Letrista (el que escribe la letra) o Compositor ( de la música). Estos autores son los que tienen los derechos de autor de la obra.

Un **intérprete** puede realizar una **versión** de una obra.

Un intérprete puede ser un solista o un grupo de artistas. 

Cada versión tiene una letra y un archivo de audio asociado que es lo que llamaremos **canción** y como versión puede haber cambios a la obra original (tono, género, arreglos o partes de la letra ) es importante gardar la duración, género, año de lanzamiento y una foto de portada.



### Los artistas
Cada artista tiene un nombre, una biografía, una foto de perfil y un género musical principal. También necesito saber cuántas canciones ha subido, cuántas reproducciones tienen en total y cuántos seguidores tienen. Los artistas pueden seguir a otros artistas.

Un artista puede ser cantante, compositor, productor, etc. y necesito saber cuál es su rol en cada canción. 

### Las listas de reproducción
Cada lista de reproducción tiene un nombre, una descripción y un usuario creador. También necesito saber cuántas canciones tiene y cuántas veces se ha reproducido. Las listas de reproducción pueden ser públicas o privadas, y los usuarios pueden seguir las listas de otros usuarios.

### Los álbumes
Cada álbum tiene un nombre, un año de lanzamiento y un artista. También necesito saber cuántas y cuales canciones tiene y cuántas veces se ha reproducido. Los álbumes pueden tener un género musical y una portada. Los álbumes pueden ser de un solo artista o de varios artistas.
Las canciones tienen un orden en el álbum.
Un álbum puede ser un álbum de estudio, un álbum en vivo, un EP, etc.
Un album pertenece a un sello discográfico, que es la empresa que lo produce y distribuye.

### Los sellos discográficos   
Cada sello discográfico tiene un nombre, una dirección y un número de teléfono.


### Los usuarios 
Cada usuario tiene un nombre, un correo electrónico, una contraseña, una fecha de nacimiento y una foto de perfil. También necesito saber cuántas canciones ha subido, cuántas listas de reproducción ha creado, cuántas canciones ha escuchado y cuántas veces ha escuchado cada canción. Los usuarios pueden seguir a otros usuarios y a artistas.

### Estadísticas de reproducción
Cada vez que un usuario escucha una canción, se registra la fecha y hora de la reproducción, el usuario que la escuchó, la canción que escuchó y la duración de la reproducción. También necesito saber si la reproducción fue completa o no. Opcionalmente puedo saber si adelantó la canción, si la repitió o si la saltó o si repitió una parte. Esto me permitirá calcular las reproducciones completas y las parciales y conocer mas sobre los gustos y del usuario.