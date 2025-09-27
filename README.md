# Proyectos de Base de datos

Este repositorio contiene una colección de **casos de estudio de diseño de bases de datos** para cursos de Ingeniería en Sistemas. Cada proyecto representa un dominio de negocio completo con requerimientos reales escritos en lenguaje del dominio empresarial.

## 📚 Estructura del Repositorio

Cada directorio representa un caso de negocio completo con:
- **Especificación principal**: `{Proyecto}.md` con requerimientos completos del negocio
- **Consultas SQL**: `Consultas.md` organizadas por niveles de dificultad (Básico/Intermedio/Avanzado/Analítica)
- **Historias de validación**: Escenarios complejos para probar el diseño
- **Recursos adicionales**: Documentos, plantillas y ejemplos del mundo real

## 🏢 Proyectos Disponibles

### Agroquímicos
**Dominio**: Distribución y manejo de productos agroquímicos
- **Entidades principales**: Productos químicos, distribuidores, agricultores, aplicaciones
- **Complejidad**: Manejo de sustancias reguladas, trazabilidad, inventario especializado
- **Casos de uso**: Control de inventario peligroso, cumplimiento regulatorio, distribución regional

### Bichos de Bolsillo
**Dominio**: Juego de colección y batalla de criaturas digitales
- **Entidades principales**: Criaturas, entrenadores, batallas, evoluciones, movimientos
- **Complejidad**: Sistema de combate, mecánicas de evolución, estadísticas complejas
- **Casos de uso**: Gestión de colecciones, sistema de batallas, progresión de personajes

### Comedor Escolar
**Dominio**: Sistema de alimentación para colegio con kínder y primaria
- **Entidades principales**: Estudiantes, menús, recetas, ingredientes, pagos, alergias
- **Complejidad**: Restricciones alimentarias, control nutricional, facturación familiar
- **Casos de uso**: Planificación de menús, control de alergias, gestión de pagos
- **Consultas**: 80 consultas organizadas en 4 niveles de dificultad

### Conquistadores
**Dominio**: Gestión de club scout con múltiples sedes y especialidades
- **Entidades principales**: Clubes, miembros, clases, especialidades, requisitos, familias
- **Complejidad**: Relaciones familiares multi-generacionales, progresión por edades, voluntarios
- **Casos de uso**: Seguimiento de avances, ceremonias de investidura, gestión de voluntarios
- **Consultas**: 75 consultas con análisis de progresión y relaciones familiares

### Cuatro Cuadras
**Dominio**: Red social de barrio para comercio local
- **Entidades principales**: Vecinos, comercios, productos, reseñas, transacciones locales
- **Complejidad**: Geolocalización, reputación comunitaria, comercio de proximidad
- **Casos de uso**: Promoción de negocios locales, recomendaciones vecinales
- **Estado**: En desarrollo (programado para enero 2026)

### Inmobiliaria Morshu Estates
**Dominio**: Compra, venta y renta de propiedades inmobiliarias
- **Entidades principales**: Propiedades, clientes, agentes, contratos, tasaciones
- **Complejidad**: Valuaciones dinámicas, contratos múltiples, comisiones de agentes
- **Casos de uso**: Gestión de inventario inmobiliario, seguimiento de transacciones

### MasterBall Tournaments
**Dominio**: Organización de torneos de videojuegos competitivos
- **Entidades principales**: Jugadores, torneos, partidas, rankings, premios
- **Complejidad**: Sistemas de eliminación, rankings ELO, distribución de premios
- **Casos de uso**: Gestión de competencias, seguimiento de estadísticas
- **Estado**: En desarrollo (programado para enero 2026)

### MyBeat
**Dominio**: Plataforma de streaming musical con gestión de regalías
- **Entidades principales**: Artistas, canciones, álbumes, usuarios, reproducciones, regalías
- **Complejidad**: Derechos de autor, colaboraciones múltiples, análisis de popularidad
- **Casos de uso**: Distribución de regalías, recomendaciones personalizadas, análisis de tendencias
- **Consultas**: 80 consultas incluyendo análisis de comportamiento musical y predicción de éxitos

### Pawfect Care
**Dominio**: Clínica veterinaria con servicios integrales para mascotas
- **Entidades principales**: Mascotas, dueños, veterinarios, tratamientos, inventario médico
- **Complejidad**: Historiales médicos, inventario farmacéutico, programación de citas
- **Casos de uso**: Gestión de expedientes médicos, control de vacunas, inventario veterinario

### Salud y Vida
**Dominio**: Sistema hospitalario con múltiples especialidades médicas
- **Entidades principales**: Pacientes, médicos, citas, expedientes, farmacia, laboratorio
- **Complejidad**: Integración de sistemas médicos, privacidad de datos, facturación de seguros
- **Casos de uso**: Gestión de expedientes médicos, programación quirúrgica, control farmacéutico

### Taller Automotriz "El Robe"
**Dominio**: Red nacional de talleres mecánicos con servicios especializados
- **Entidades principales**: Vehículos, clientes, órdenes de trabajo, refacciones, técnicos
- **Complejidad**: Historial vehicular, garantías, inventario multi-sucursal, flotas empresariales
- **Casos de uso**: Mantenimiento preventivo, control de garantías, gestión de flotas
- **Consultas**: 80 consultas con análisis de rentabilidad y optimización operativa

### TrumpetWare
**Dominio**: Sistema MLM (multinivel) de venta de productos por catálogo
- **Entidades principales**: Embajadores, productos, campañas, clientes, CEDIS, comisiones
- **Complejidad**: Estructura multinivel, campañas estacionales, logística de distribución
- **Casos de uso**: Cálculo de comisiones, gestión de inventario, seguimiento de campañas

### Zaboo Mazoo
**Dominio**: Gestión integral de parque zoológico
- **Entidades principales**: Animales, hábitats, cuidadores, visitantes, alimentación, veterinaria
- **Complejidad**: Cuidado especializado por especie, programación de personal, seguridad
- **Casos de uso**: Programas de conservación, gestión de personal, control sanitario
- **Recursos**: Formularios en papel para demostrar problemas pre-digitalización

## 🎯 Metodología Educativa

### Niveles de Consultas SQL
1. **Básico**: SELECT, WHERE, ORDER BY, GROUP BY básico
2. **Intermedio**: JOINs, subconsultas, agregaciones, HAVING
3. **Avanzado**: PIVOT, COALESCE, UNION, INTERSECT, EXCEPT, CASE WHEN
4. **Analítica**: Funciones de ventana, CTEs recursivos, análisis predictivo

### Historias de Validación
Cada proyecto incluye 6 historias complejas que presentan:
- **Escenarios realistas** con múltiples variables simultáneas
- **Casos extremos** que prueban los límites del diseño
- **Situaciones de crisis** que requieren adaptabilidad del sistema
- **Preguntas de validación** para verificar que el diseño maneja la complejidad

### Recursos Adicionales
- **Documentos en papel**: Formularios tradicionales que muestran problemas pre-digitalización
- **Plantillas operativas**: Documentos de trabajo del mundo real
- **Datos de ejemplo**: CSVs y ejemplos concretos para poblar las bases de datos

## 🚀 Cómo Usar Este Repositorio

1. **Selecciona un proyecto** basado en el dominio de interés
2. **Lee la especificación completa** en el archivo principal `.md`
3. **Diseña el modelo de base de datos** considerando todas las entidades y relaciones
4. **Implementa las consultas** progresando por niveles de dificultad
5. **Valida tu diseño** usando las historias complejas de validación
6. **Documenta decisiones** de diseño y justifica la normalización elegida

## 📖 Generación de Documentación

Este repositorio usa **Quarto** para generar documentación en múltiples formatos:

```bash
# Generar libro completo en HTML y PDF
quarto render

# Solo HTML
quarto render --to html

# Solo PDF
quarto render --to pdf
```

## 🎓 Objetivos de Aprendizaje

Los estudiantes desarrollarán habilidades en:
- **Análisis de requerimientos** en lenguaje natural de negocio
- **Diseño conceptual y lógico** de bases de datos relacionales
- **Normalización** y optimización de estructuras
- **Consultas SQL complejas** con múltiples niveles de dificultad
- **Validación de diseños** mediante casos de uso extremos
- **Documentación técnica** y justificación de decisiones de diseño

## 📝 Estado de Desarrollo

- ✅ **Completos**: 10 proyectos con especificaciones, consultas e historias de validación
- 🔄 **En desarrollo**: 3 proyectos programados para enero 2026
- 📚 **Total de consultas**: Más de 500 consultas SQL organizadas por dificultad
- 🎯 **Historias de validación**: 78 escenarios complejos de prueba

---

*Desarrollado para cursos de Bases de Datos en Ingeniería en Sistemas*  
*Autor: Pedro Villa Casas*  
*Última actualización: Septiembre 2025*


