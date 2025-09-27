# Consultas - Sistema MyBeat

## Consultas Básico

### 1. Mostrar todos los artistas registrados en la plataforma
Obtener la lista completa de artistas incluyendo nombre, biografía, género principal y foto de perfil.

### 2. Listar todas las canciones disponibles
Mostrar todas las canciones en la plataforma con su título, duración, género y año de lanzamiento.

### 3. Obtener información de todos los usuarios activos
Visualizar datos de usuarios como nombre, correo electrónico, fecha de nacimiento y foto de perfil.

### 4. Consultar todas las obras musicales registradas
Mostrar las obras originales con sus títulos, géneros, años de lanzamiento y autores.

### 5. Listar todos los álbumes con su información básica
Obtener nombre del álbum, año de lanzamiento, artista y tipo de álbum (estudio, en vivo, EP).

### 6. Mostrar todas las listas de reproducción públicas
Ver las playlists públicas con nombre, descripción, usuario creador y número de canciones.

### 7. Consultar los sellos discográficos registrados
Listar todos los sellos con nombre, dirección y teléfono de contacto.

### 8. Obtener las reproducciones del día actual
Mostrar todas las reproducciones que se han registrado en las últimas 24 horas.

### 9. Listar los géneros musicales disponibles
Ver todos los géneros musicales que están siendo utilizados en la plataforma.

### 10. Consultar los intérpretes con más seguidores
Mostrar los artistas ordenados por número de seguidores de mayor a menor.

### 11. Obtener las canciones más recientes subidas
Listar las últimas canciones agregadas a la plataforma ordenadas por fecha de subida.

### 12. Mostrar los usuarios que crearon cuenta esta semana
Identificar los nuevos usuarios registrados en los últimos 7 días.

### 13. Consultar las versiones de una obra específica
Ver todas las diferentes versiones/interpretaciones que existen de una obra musical particular.

### 14. Listar los artistas por género musical principal
Agrupar y mostrar artistas según su género musical predominante.

### 15. Obtener las listas de reproducción de un usuario específico
Mostrar todas las playlists creadas por un usuario determinado, tanto públicas como privadas.

### 16. Consultar la duración promedio de las canciones por género
Calcular y mostrar la duración media de las canciones agrupadas por género musical.

### 17. Mostrar las canciones de un álbum en orden
Listar todas las canciones de un álbum específico respetando su orden de pista.

### 18. Obtener los compositores más prolíficos
Identificar qué compositores tienen mayor número de obras registradas.

### 19. Listar las reproducciones completas vs parciales
Mostrar estadísticas de reproducciones distinguiendo entre completas y parciales.

### 20. Consultar los artistas que también son productores
Identificar artistas que tienen múltiples roles (intérprete, compositor, productor).

## Consultas Intermedio

### 1. Calcular las regalías mensuales por artista considerando todos sus roles
Determinar los ingresos de cada artista sumando sus participaciones como compositor, intérprete y productor en todas las reproducciones del mes.

### 2. Identificar las canciones más populares por rango de edad de usuarios
Analizar qué canciones prefieren diferentes grupos etarios (menores de 18, 18-25, 26-35, etc.) basándose en sus reproducciones.

### 3. Generar ranking de álbumes por total de reproducciones de sus canciones
Calcular la popularidad de cada álbum sumando todas las reproducciones de las canciones que contiene.

### 4. Obtener estadísticas de comportamiento de escucha por usuario
Para cada usuario, calcular promedio de canciones escuchadas por día, géneros favoritos y patrones de repetición.

### 5. Calcular la distribución de regalías entre múltiples autores de una obra
Determinar cómo se reparten los ingresos cuando una canción tiene varios compositores, letristas e intérpretes.

### 6. Identificar las listas de reproducción más influyentes
Encontrar playlists que han generado mayor número de reproducciones para las canciones que incluyen.

### 7. Analizar el rendimiento de un sello discográfico
Calcular total de reproducciones, artistas activos y ingresos generados por álbumes de un sello específico.

### 8. Obtener el historial completo de versiones de una obra
Mostrar todas las interpretaciones de una obra original con sus diferencias en género, duración y popularidad.

### 9. Calcular la tasa de retención de usuarios por mes
Determinar qué porcentaje de usuarios siguen activos después de su primer, segundo y tercer mes de actividad.

### 10. Identificar colaboraciones frecuentes entre artistas
Encontrar pares o grupos de artistas que han trabajado juntos en múltiples canciones o álbumes.

### 11. Analizar patrones de abandono en reproducciones por género
Determinar en qué punto promedio los usuarios saltan canciones de diferentes géneros musicales.

### 12. Generar reporte de crecimiento de seguidores por artista
Calcular la evolución mensual del número de seguidores para cada artista en la plataforma.

### 13. Obtener estadísticas de uso de playlists por popularidad
Analizar cuántas veces se reproducen las playlists según su número de seguidores y canciones incluidas.

### 14. Calcular el impacto de las nuevas versiones en las obras originales
Medir cómo afectan las nuevas interpretaciones a la popularidad de las obras originales.

### 15. Identificar tendencias emergentes por análisis de reproducciones
Detectar géneros, artistas o canciones que están experimentando crecimiento acelerado en reproducciones.

### 16. Generar balance financiero por tipo de contenido
Calcular ingresos separados por canciones originales, versiones, álbumes completos y reproducciones en playlists.

### 17. Analizar la efectividad de las recomendaciones personalizadas
Medir qué porcentaje de las recomendaciones automáticas resultan en reproducciones completas.

### 18. Obtener métricas de engagement por segmento de usuarios
Comparar nivel de actividad entre usuarios freemium, premium, artistas y sellos discográficos.

### 19. Calcular la longevidad promedio de las canciones en playlists
Determinar cuánto tiempo permanecen las canciones en las listas de reproducción antes de ser removidas.

### 20. Identificar oportunidades de cross-promotion entre artistas similares
Encontrar artistas con audiencias compatibles para sugerir colaboraciones o promociones cruzadas.

## Consultas Avanzado

### 1. Comparar artistas emergentes con establecidos usando múltiples métricas
Utilizar UNION para combinar datos de artistas nuevos (menos de 2 años) con veteranos, y CASE WHEN para clasificarlos por crecimiento de seguidores, reproducciones mensuales y colaboraciones.

### 2. Identificar obras originales que no tienen versiones usando operaciones de conjunto
Usar EXCEPT para encontrar obras que nunca han sido versionadas por otros artistas, y INTERSECT para comparar con obras más populares.

### 3. Generar reporte consolidado de ingresos con manejo de valores nulos
Utilizar COALESCE para mostrar información financiera donde, si no hay datos de streaming, se muestre ingresos por descargas, y si tampoco, mostrar "Sin ingresos registrados".

### 4. Crear matriz de popularidad de géneros por rango de edad
Usar PIVOT para mostrar cada género como fila y rangos de edad como columnas, con el promedio de reproducciones por usuario en cada segmento.

### 5. Encontrar usuarios con gustos musicales idénticos usando intersección
Aplicar INTERSECT para identificar usuarios que han reproducido exactamente las mismas canciones en el último mes.

### 6. Clasificar artistas por nivel de actividad con subconsultas correlacionadas
Usar subconsultas para categorizar artistas como "muy activos", "moderadamente activos" o "inactivos" basándose en subidas de contenido y actividad comparada con promedios.

### 7. Analizar rendimiento de canciones con lógica condicional compleja
Utilizar CASE WHEN para clasificar canciones como "hit", "moderado éxito", "nicho" o "sin tracción" según reproducciones, permanencia en playlists and engagement.

### 8. Identificar conflictos de derechos de autor con subconsultas avanzadas
Usar subconsultas EXISTS para encontrar posibles plagios comparando duraciones, géneros y fechas de lanzamiento de canciones sospechosamente similares.

### 9. Consolidar diferentes tipos de colaboraciones musicales
Emplear UNION ALL para combinar compositores, letristas, intérpretes y productores de una obra, mostrando el tipo de contribución de cada uno.

### 10. Crear vista de preferencias musicales con valores por defecto
Usar COALESCE para generar perfiles de usuario donde, si no hay géneros favoritos definidos, se calculen automáticamente basándose en reproducciones históricas.

### 11. Detectar patrones anómalos en reproducciones usando comparaciones
Utilizar subconsultas para identificar canciones con picos de reproducción sospechosos que podrían indicar manipulación artificial.

### 12. Generar tabla cruzada de colaboraciones por período
Aplicar PIVOT para mostrar artistas como filas y meses como columnas, indicando número de colaboraciones realizadas en cada período.

### 13. Comparar estrategias de lanzamiento entre sellos discográficos
Usar INTERSECT y EXCEPT para analizar diferencias en géneros, tipos de álbum y estrategias de marketing entre diferentes sellos.

### 14. Segmentar usuarios por comportamiento de consumo con lógica avanzada
Emplear CASE WHEN con subconsultas para clasificar usuarios en "descubridores", "consumidores habituales", "coleccionistas" según patrones de escucha.

### 15. Identificar obras que comparten elementos musicales similares
Usar INTERSECT para encontrar canciones que tienen los mismos compositores base, géneros relacionados o duraciones similares.

### 16. Sistema de alertas de rendimiento con priorización
Utilizar CASE WHEN para asignar prioridades a alertas: caída dramática en reproducciones (crítico), estancamiento (medio), crecimiento lento (bajo).

### 17. Analizar migración de usuarios entre géneros musicales
Aplicar EXCEPT para identificar usuarios que han dejado de escuchar ciertos géneros y han migrado completamente a otros.

### 18. Consolidar información de contacto de artistas con múltiples opciones
Usar COALESCE para crear contacto de emergencia priorizando: manager oficial, sello discográfico, contacto directo, redes sociales.

### 19. Matriz de compatibilidad musical para recomendaciones
Emplear PIVOT para crear tabla con usuarios como filas y géneros como columnas, marcando afinidad y usándola para recomendaciones cruzadas.

### 20. Identificar nichos musicales únicos usando análisis de conjuntos
Utilizar subconsultas complejas y operaciones de conjunto para encontrar combinaciones de género-artista-audiencia que no tienen competencia directa.

## Consultas de Analítica

### 1. Modelado predictivo de éxito de canciones basado en patrones históricos
Desarrollar algoritmos que analicen características de canciones exitosas (duración, género, colaboraciones, timing de lanzamiento) para predecir el potencial de nuevos lanzamientos.

### 2. Análisis multidimensional de comportamiento de usuarios con segmentación avanzada
Crear perfiles complejos de usuarios combinando datos demográficos, patrones de escucha, interacciones sociales y preferencias temporales para personalización extrema.

### 3. Optimización dinámica de regalías con machine learning
Implementar sistemas que ajusten automáticamente la distribución de regalías basándose en múltiples factores: popularidad, tipo de audiencia, engagement, y valor de retención de usuarios.

### 4. Sistema de detección de tendencias emergentes con análisis temporal
Utilizar series de tiempo y análisis de clusters para identificar géneros, artistas o estilos musicales que están ganando tracción antes de que se vuelvan mainstream.

### 5. Análisis de network effects en descubrimiento musical
Modelar cómo las decisiones de usuarios influyentes afectan el descubrimiento de música, identificando nodos críticos en la red social de la plataforma.

### 6. Optimización de algoritmos de recomendación con feedback loops
Desarrollar sistemas que aprendan de las interacciones de usuarios (saltos, repeticiones, adiciones a playlists) para mejorar continuamente las sugerencias.

### 7. Análisis predictivo de rotación de usuarios y estrategias de retención
Crear modelos que identifiquen usuarios en riesgo de abandono basándose en patrones de uso, y generar estrategias personalizadas de retención.

### 8. Modelado de valor de lifetime de usuarios por segmento
Calcular el valor económico proyectado de diferentes tipos de usuarios considerando patrones de consumo, probabilidad de conversión premium y influencia social.

### 9. Análisis de sentimiento en interacciones musicales
Procesar datos de comportamiento (repeticiones, saltos, creación de playlists) para inferir satisfacción emocional y preferencias implícitas de usuarios.

### 10. Optimización de catálogo con análisis de portfolio musical
Determinar el mix óptimo de géneros, artistas emergentes vs establecidos, y contenido exclusivo vs licenciado para maximizar engagement y rentabilidad.

### 11. Análisis geoespacial de preferencias musicales con clustering
Identificar patrones regionales de consumo musical y adaptar estrategias de contenido y promoción a mercados geográficos específicos.

### 12. Modelado de ciclos de vida de canciones con análisis de supervivencia
Predecir cuánto tiempo permanecerá popular una canción y cuándo es óptimo promover nuevo contenido del mismo artista.

### 13. Análisis de competencia indirecta con correlación de audiencias
Identificar plataformas, actividades o formas de entretenimiento que compiten por el tiempo de atención de los usuarios de música.

### 14. Optimización de precios dinámicos basada en demanda y valor percibido
Desarrollar modelos que ajusten precios de suscripciones y contenido premium basándose en comportamiento de usuarios y elasticidad de demanda.

### 15. Análisis de impacto de eventos externos en consumo musical
Correlacionar eventos culturales, sociales, estacionales y económicos con cambios en patrones de escucha para anticipar demanda.

### 16. Modelado de ecosistemas musicales colaborativos
Analizar redes de colaboración entre artistas para identificar oportunidades de cross-promotion y predicción de éxito de nuevas colaboraciones.

### 17. Análisis de optimización de playlists con teoría de grafos
Determinar el orden óptimo de canciones en playlists para maximizar tiempo de escucha y satisfacción del usuario usando algoritmos de grafos.

### 18. Predictive analytics para planificación de capacidad de infraestructura
Modelar crecimiento de usuarios, patrones de uso y demanda de bandwidth para optimizar costos de infraestructura tecnológica.

### 19. Análisis de atribución multi-touch en descubrimiento musical
Determinar qué combinación de factores (recomendaciones, playlists, redes sociales, búsquedas) lleva al descubrimiento exitoso de nueva música.

### 20. Modelado de ecosistemas de derechos de autor con blockchain analytics
Implementar sistemas de trazabilidad completa de derechos musicales usando tecnología blockchain para garantizar distribución justa de regalías en tiempo real.