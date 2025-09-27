# Consultas - Sistema Taller Automotriz "El Robe"

## Consultas Básico

### 1. Mostrar todos los vehículos registrados en el taller
Obtener la lista completa de vehículos incluyendo marca, modelo, año, placas, VIN y kilometraje actual.

### 2. Listar todos los clientes activos
Mostrar información de clientes como nombre, teléfono, correo electrónico y tipo de cliente (individual o flota).

### 3. Obtener el inventario actual de refacciones
Visualizar todas las piezas disponibles con código, descripción, cantidad en stock y ubicación en almacén.

### 4. Consultar todos los técnicos y sus especialidades
Mostrar el personal técnico con nombre, especialidad principal, certificaciones y sucursal asignada.

### 5. Listar todas las órdenes de trabajo del día
Ver las órdenes programadas para hoy con cliente, vehículo, tipo de servicio y técnico asignado.

### 6. Mostrar todos los proveedores de refacciones
Obtener información de proveedores como nombre, contacto, especialidad y términos de crédito.

### 7. Consultar los servicios más comunes ofrecidos
Listar los tipos de servicio (mantenimiento preventivo, reparaciones) con descripción y tiempo estimado.

### 8. Obtener las facturas pendientes de pago
Mostrar facturas emitidas que aún no han sido pagadas con cliente, monto y fecha de vencimiento.

### 9. Listar las garantías vigentes
Ver garantías activas con cliente, servicio realizado, fecha de inicio y fecha de vencimiento.

### 10. Consultar las compras realizadas esta semana
Mostrar todas las compras de refacciones de los últimos 7 días con proveedor, monto y fecha.

### 11. Obtener el historial básico de un vehículo específico
Mostrar todos los servicios realizados a una unidad particular ordenados por fecha.

### 12. Listar las refacciones que están por agotarse
Identificar piezas con stock menor al mínimo establecido para cada una.

### 13. Consultar las órdenes de trabajo completadas hoy
Ver trabajos terminados en la fecha actual con tiempo empleado y costo total.

### 14. Mostrar los vehículos programados para mantenimiento preventivo
Listar unidades que necesitan servicio basándose en kilometraje o tiempo transcurrido.

### 15. Obtener las sucursales y su información de contacto
Mostrar todas las ubicaciones del taller con dirección, teléfono y personal asignado.

### 16. Consultar los reclamos de garantía activos
Ver casos donde se ha activado garantía por defectos en trabajo realizado o piezas instaladas.

### 17. Listar las órdenes de compra pendientes de recibir
Mostrar compras realizadas a proveedores que aún no han sido entregadas.

### 18. Obtener los clientes de flota con sus vehículos
Ver empresas con múltiples unidades y el número de vehículos registrados por cada una.

### 19. Consultar los técnicos disponibles por turno
Mostrar qué personal está programado para trabajar en cada horario (mañana, tarde, noche).

### 20. Listar las emergencias atendidas fuera de horario
Ver servicios de urgencia realizados en fines de semana o después del horario normal.

## Consultas Intermedio

### 1. Calcular el costo promedio de mantenimiento por tipo de vehículo
Determinar cuánto se gasta en promedio manteniendo diferentes marcas y modelos, considerando mano de obra y refacciones.

### 2. Identificar patrones de fallas recurrentes por vehículo
Analizar qué problemas se repiten frecuentemente en las mismas unidades para sugerir mantenimiento preventivo adicional.

### 3. Generar reporte de rentabilidad por técnico
Calcular ingresos generados vs costos de cada técnico, considerando tiempo empleado, salario y overhead.

### 4. Obtener estadísticas de tiempo de respuesta por tipo de servicio
Medir cuánto tiempo promedio toma completar diferentes tipos de trabajo (cambio de aceite, reparación de motor, etc.).

### 5. Calcular la rotación de inventario por categoría de refacciones
Determinar qué tan rápido se mueven diferentes tipos de piezas (filtros, bandas, líquidos) para optimizar compras.

### 6. Identificar clientes con mayor valor de por vida
Encontrar clientes que han generado más ingresos históricos considerando servicios, frecuencia y años de relación.

### 7. Analizar efectividad de las garantías por proveedor
Medir qué proveedores tienen menor tasa de reclamos y mejor calidad en sus refacciones.

### 8. Obtener análisis de ocupación por bahía de servicio
Calcular qué tan eficientemente se utilizan las diferentes áreas de trabajo del taller.

### 9. Calcular márgenes de ganancia por tipo de servicio
Determinar qué servicios son más rentables comparando costos directos con precios de venta.

### 10. Generar alertas de mantenimiento preventivo por flota
Crear sistema que identifique vehículos de empresas que necesitan servicio basado en kilometraje o tiempo.

### 11. Analizar patrones estacionales en tipos de servicios
Identificar qué servicios se demandan más en ciertas épocas del año (aire acondicionado, neumáticos, etc.).

### 12. Calcular eficiencia de técnicos por tiempo vs presupuesto
Medir qué tan precisos son los técnicos estimando tiempo y costo real vs tiempo y costo presupuestado.

### 13. Obtener análisis de satisfacción del cliente por sucursal
Correlacionar reclamos, trabajos rehechos y retención de clientes por ubicación.

### 14. Generar reporte de cash flow basado en cuentas por cobrar
Proyectar flujo de efectivo considerando facturas pendientes, plazos de pago y patrones históricos.

### 15. Identificar oportunidades de cross-selling en servicios
Encontrar servicios complementarios que frecuentemente se realizan juntos para sugerir paquetes.

### 16. Calcular costo total de ownership por vehículo de flota
Determinar el costo completo de mantener cada unidad durante su vida útil para justificar renovación.

### 17. Analizar tendencias de precios de refacciones por proveedor
Monitorear evolución de costos de piezas para negociar mejores contratos y detectar oportunidades.

### 18. Obtener métricas de calidad por tipo de trabajo
Medir tasa de retrabajos, reclamos de garantía y satisfacción del cliente por categoría de servicio.

### 19. Generar análisis de competitividad de precios
Comparar tarifas del taller con mercado local para mantener competitividad sin sacrificar rentabilidad.

### 20. Calcular impacto económico de downtime de vehículos comerciales
Medir costo de oportunidad para clientes cuando sus vehículos comerciales están en reparación.

## Consultas Avanzado

### 1. Comparar rendimiento de técnicos generales vs especialistas
Utilizar UNION para combinar métricas de productividad de mecánicos generales con especialistas, y CASE WHEN para clasificar por eficiencia y calidad.

### 2. Identificar refacciones exclusivas por marca usando operaciones de conjunto
Usar EXCEPT para encontrar piezas que solo se usan en ciertas marcas de vehículos, e INTERSECT para piezas universales.

### 3. Generar reporte de pagos con manejo de múltiples formas
Utilizar COALESCE para mostrar información de pagos donde, si no hay pago en efectivo, se muestre tarjeta, si no cheque, si no "Pendiente".

### 4. Crear matriz de servicios por mes del año
Usar PIVOT para mostrar cada tipo de servicio como fila y meses como columnas, con cantidad de servicios realizados en cada período.

### 5. Encontrar vehículos con historial de mantenimiento idéntico
Aplicar INTERSECT para identificar unidades que han recibido exactamente los mismos servicios en el mismo orden.

### 6. Clasificar clientes por nivel de fidelidad con subconsultas correlacionadas
Usar subconsultas para categorizar clientes como "muy fieles", "regulares" o "esporádicos" basándose en frecuencia y años de relación.

### 7. Analizar estado de órdenes de trabajo con lógica condicional
Utilizar CASE WHEN para clasificar órdenes como "urgente", "normal", "atrasada" o "completada" según fechas y prioridades.

### 8. Identificar problemas recurrentes en garantías con subconsultas
Usar subconsultas EXISTS para encontrar patrones de fallas que se repiten en el mismo vehículo dentro del período de garantía.

### 9. Consolidar diferentes tipos de costos por orden de trabajo
Emplear UNION ALL para combinar costos de mano de obra, refacciones, subcontratistas y overhead en un reporte unificado.

### 10. Crear vista de disponibilidad de técnicos con valores por defecto
Usar COALESCE para mostrar horarios donde, si no hay técnico especialista disponible, se asigne generalista, o si no "Sin asignar".

### 11. Detectar anomalías en consumo de refacciones por técnico
Utilizar subconsultas para identificar técnicos que usan cantidades inusuales de ciertas piezas comparado con sus pares.

### 12. Generar tabla cruzada de garantías por proveedor y mes
Aplicar PIVOT para mostrar proveedores como filas y meses como columnas, indicando número de reclamos de garantía.

### 13. Comparar estrategias de inventario entre sucursales
Usar INTERSECT y EXCEPT para analizar diferencias en tipos de refacciones almacenadas y políticas de stock mínimo.

### 14. Segmentar vehículos por criticidad de mantenimiento
Emplear CASE WHEN con subconsultas para clasificar unidades como "críticas", "moderadas" o "bajas" según uso e historial.

### 15. Identificar servicios que siempre se realizan juntos
Usar INTERSECT para encontrar combinaciones de servicios que frecuentemente aparecen en las mismas órdenes de trabajo.

### 16. Sistema de alertas de inventario con priorización automática
Utilizar CASE WHEN para asignar prioridades: piezas críticas agotadas (urgente), stock bajo (alta), reposición normal (media).

### 17. Analizar migración de clientes entre sucursales
Aplicar EXCEPT para identificar clientes que han cambiado de sucursal habitual y analizar posibles causas.

### 18. Consolidar información de contacto con múltiples canales
Usar COALESCE para crear contacto de emergencia priorizando: teléfono móvil, teléfono casa, trabajo, correo electrónico.

### 19. Matriz de compatibilidad de servicios por tipo de vehículo
Emplear PIVOT para crear tabla con servicios como filas y tipos de vehículo como columnas, marcando aplicabilidad.

### 20. Identificar nichos de especialización únicos por sucursal
Utilizar subconsultas complejas para encontrar combinaciones de servicio-marca-modelo que solo maneja una sucursal específica.

## Consultas de Analítica

### 1. Modelado predictivo de fallas vehiculares basado en patrones históricos
Desarrollar algoritmos que analicen historiales de mantenimiento, kilometraje, uso y edad para predecir cuándo fallarán componentes específicos.

### 2. Optimización dinámica de inventarios con machine learning
Implementar sistemas que ajusten automáticamente niveles de stock basándose en estacionalidad, tendencias de fallas y tiempo de entrega de proveedores.

### 3. Análisis multidimensional de rentabilidad por cliente con segmentación avanzada
Crear perfiles complejos de clientes combinando valor de por vida, frecuencia de visitas, tipos de servicios y margen de ganancia.

### 4. Sistema de recomendación de mantenimiento preventivo personalizado
Utilizar IA para sugerir servicios específicos por vehículo basándose en uso, condiciones de operación y historial de la marca/modelo.

### 5. Análisis de network effects en cadena de suministro de refacciones
Modelar cómo las decisiones de compra y relaciones con proveedores afectan costos, disponibilidad y calidad en toda la red.

### 6. Optimización de scheduling de técnicos con algoritmos genéticos
Desarrollar sistemas que asignen automáticamente trabajos a técnicos considerando especialización, carga de trabajo y deadlines.

### 7. Análisis predictivo de rotación de personal y estrategias de retención
Crear modelos que identifiquen técnicos en riesgo de renunciar basándose en productividad, satisfacción y oportunidades externas.

### 8. Modelado de valor de fleet management para clientes empresariales
Calcular el ROI de servicios de mantenimiento preventivo para flotas considerando downtime evitado y extensión de vida útil.

### 9. Análisis de sentimiento en feedback de clientes con NLP
Procesar comentarios, quejas y sugerencias para identificar áreas de mejora y medir satisfacción de manera automática.

### 10. Optimización de precios dinámicos basada en demanda y capacidad
Desarrollar modelos que ajusten tarifas de servicios basándose en ocupación del taller, urgencia del trabajo y valor para el cliente.

### 11. Análisis geoespacial de expansión de sucursales con clustering
Identificar ubicaciones óptimas para nuevas sucursales basándose en densidad de clientes potenciales y competencia.

### 12. Modelado de ciclos de vida de vehículos con análisis de supervivencia
Predecir cuándo es más económico reemplazar que reparar, ayudando a clientes en decisiones de renovación de flota.

### 13. Análisis de competencia con inteligencia de mercado
Monitorear precios, servicios y estrategias de competidores para mantener ventaja competitiva y identificar oportunidades.

### 14. Optimización de rutas de distribución de refacciones entre sucursales
Usar algoritmos de optimización para minimizar costos y tiempo de transferencia de inventario entre ubicaciones.

### 15. Análisis de impacto de factores externos en demanda de servicios
Correlacionar clima, tráfico, eventos económicos y estacionales con patrones de demanda para planificación de capacidad.

### 16. Modelado de ecosistemas de garantías con blockchain
Implementar trazabilidad completa de trabajos y piezas para automatizar reclamos de garantía y mejorar transparencia.

### 17. Análisis de optimización de mix de servicios con teoría de colas
Determinar la combinación óptima de servicios rápidos vs complejos para maximizar throughput y satisfacción del cliente.

### 18. Predictive analytics para mantenimiento de equipos del taller
Modelar cuándo fallarán herramientas y equipos del taller para programar mantenimiento preventivo y evitar downtime.

### 19. Análisis de atribución multi-touch en acquisition de clientes
Determinar qué combinación de marketing, referencias y experiencias lleva a la adquisición exitosa de nuevos clientes.

### 20. Modelado de resiliencia operacional con análisis de escenarios
Simular diferentes crisis (desabasto de piezas, pérdida de personal, cambios regulatorios) para desarrollar planes de contingencia.