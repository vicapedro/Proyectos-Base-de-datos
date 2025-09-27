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

## Historias de Validación

### Historia 1: El éxito viral de "Corazón Digital"
La cantautora independiente Ana López lanza su canción "Corazón Digital" en febrero. Ella escribió tanto la letra como la música, y la grabó en su estudio casero. La canción pertenece al género Pop Alternativo y dura 3:45 minutos. Inicialmente solo la escuchan sus 250 seguidores, pero cuando el influencer musical @CarlosBeats la incluye en su playlist "Nuevos Talentos 2025", todo cambia. En una semana, la canción acumula 50,000 reproducciones, Ana gana 2,000 nuevos seguidores y "Corazón Digital" aparece en más de 500 playlists creadas por usuarios. Las estadísticas muestran que el 70% de las reproducciones son completas, y muchos usuarios repiten la canción inmediatamente después de escucharla. Ana decide crear su primer álbum "Sonidos Urbanos" incluyendo esta canción como track número 3 de 10 canciones totales.

**Pregunta para validar:** ¿Cómo registrarías el crecimiento viral de una canción, el impacto de las playlists en las reproducciones, el incremento de seguidores del artista y la posterior inclusión en un álbum?

### Historia 2: La colaboración compleja de "Ritmo de Medianoche"
El productor Miguel Hernández crea la base musical de "Ritmo de Medianoche" (género Reggaetón, 4:12 min). Luego colabora con tres artistas: la rapera Sofía "MC Storm" como letrista y vocalista principal, el cantante Roberto Díaz en el coro, y el DJ Alexis en efectos adicionales. La canción se lanza bajo el sello discográfico "Urban Sound Records" como parte del álbum colaborativo "Noches de Ciudad". Durante el primer mes, acumula 120,000 reproducciones, pero las estadísticas revelan que el 40% de los usuarios saltan la canción después del primer minuto, mientras que un 25% la repite inmediatamente. Los cuatro artistas involucrados deben recibir regalías según su contribución: Miguel 40% (productor), Sofía 30% (letrista y voz principal), Roberto 20% (coros) y Alexis 10% (efectos).

**Pregunta para validar:** ¿Cómo manejarías una canción con múltiples artistas en diferentes roles, la distribución de regalías, las estadísticas detalladas de reproducción y la pertenencia a un álbum colaborativo?

### Historia 3: El usuario obsesivo y sus listas temáticas
El usuario @MelomanoMax es un coleccionista musical extremo. Ha creado 47 playlists diferentes, cada una con temas específicos: "Lunes Motivacional" (35 canciones), "Nostalgia 90s" (127 canciones), "Workout Hardcore" (89 canciones), "Lluvias Románticas" (56 canciones), entre otras. Su playlist más popular "Clásicos Redescubiertos" tiene 2,500 seguidores y ha sido reproducida 15,000 veces en total. Max escucha música 6-8 horas diarias, tiene más de 80,000 reproducciones registradas y sigue a 340 artistas diferentes. Sus estadísticas muestran que prefiere géneros Rock (35%), Jazz (25%), Blues (20%) y Clásica (20%). Frecuentemente adelanta canciones después de 30-45 segundos si no le convencen, pero cuando una canción le gusta, la repite entre 3-5 veces seguidas.

**Pregunta para validar:** ¿Cómo registrarías el comportamiento de un usuario super-activo, sus múltiples playlists con diferentes niveles de popularidad, sus patrones de escucha detallados y las preferencias musicales calculadas?

### Historia 4: El artista que reinventa clásicos
El músico indie Javier Torres se especializa en crear versiones acústicas de canciones famosas. Toma "Bohemian Rhapsody" de Queen (obra original de 1975, compositores: Freddie Mercury) y crea su propia versión acústica de 5:20 minutos, cambiando el género de Rock Progresivo a Folk Acústico. Luego hace lo mismo con "Billie Jean" de Michael Jackson (obra original de 1982, compositor: Michael Jackson), creando una versión de 4:05 minutos en género Acoustic Pop. Ambas versiones las incluye en su álbum "Clásicos Despojados" bajo el sello independiente "Indie Collective Records". Sus versiones acumulan 25,000 y 18,000 reproducciones respectivamente, y varios usuarios comentan comparándolas con las versiones originales. Los titulares de los derechos de las obras originales reciben regalías por las nuevas versiones.

**Pregunta para validar:** ¿Cómo distinguirías entre las obras originales y las versiones, manejarías los diferentes géneros y duraciones de una misma obra, y calcularías las regalías tanto para intérpretes como para compositores originales?

### Historia 5: El fenómeno del álbum conceptual multiplataforma
La banda "Eco Digital" lanza el álbum conceptual "Historias de la Red" bajo "Future Sound Records". El álbum tiene 12 canciones que narran una historia continua, cada una con diferente duración (desde 2:30 hasta 7:45 minutos) y géneros que van evolucionando (Electronic, Synthpop, Ambient, Techno). La banda está formada por 4 miembros: Luis (voz y letras), Carmen (sintetizadores y composición), David (programación y producción) y Sara (violín y arreglos). Cada canción tiene diferentes combinaciones de estos artistas como autores. El álbum se vuelve viral cuando los usuarios descubren que debe escucharse en orden específico, generando 200,000 reproducciones en la primera semana. Las estadísticas muestran que el 60% de las reproducciones son del álbum completo en orden, y se crean más de 1,200 playlists que incluyen todas las canciones secuencialmente.

**Pregunta para validar:** ¿Cómo registrarías un álbum con orden específico, múltiples géneros evolutivos, diferentes autores por canción, y el patrón de escucha secuencial de los usuarios?

### Historia 6: La crisis de los derechos de autor
Una controversia surge cuando el usuario @VintageFinder descubre que la canción "Ecos del Pasado" del artista emergente Tomás Ruiz es muy similar a "Memories Lost" de la banda británica "Lost Echo" de 1987. La investigación revela que Tomás usó una muestra (sample) de 15 segundos de la canción original sin autorización. "Ecos del Pasado" ya había acumulado 85,000 reproducciones y estaba incluida en 450 playlists de usuarios. El sello "Lost Echo Records" (dueño de los derechos de "Memories Lost") exige que se retire la canción, pero Tomás negocia un acuerdo: reconoce a los compositores originales (James Smith y Robert Wilson) como co-autores, acepta compartir el 60% de las regalías y modifica la información de la canción. La canción permanece disponible pero con los créditos actualizados, y las reproducciones futuras generan regalías para ambas partes.

**Pregunta para validar:** ¿Cómo manejarías un conflicto de derechos de autor con cambios retroactivos en la autoría, redistribución de regalías, y el mantenimiento del historial de reproducciones previo al acuerdo?


