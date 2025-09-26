# TrumpetWare

## Descripción General
TrumpetWare es un fabricante de productos de belleza y del hogar que distribuye a través de embajadores. Debido al crecimiento reciente, es necesario diseñar una Base datos para soportar una **Mobile App** y una **Web App** que permitan gestionar las ventas, pedidos y embajadores. Este caso práctico detalla los requisitos de la empresa.

## Requisitos del Sistema
### Productos

Cada producto tiene:
- Nombre, clave, descripción.
- Precio al público, precio al embajador y costo de producción (no visible al embajador).
- Cada producto pertenece a una o más categorías:
  - Belleza, Limpieza del hogar, Ropa, Jardinería, Organizadores.
- Algunos productos se venden solo en ciertas épocas del año y pueden estar descontinuados.
- Durante campañas, los productos pueden tener promociones (descuentos aplicados sobre su precio de venta).

### Campañas y Temporadas
- Las campañas tienen una duración de 1 mes y no se traslapan.
- Cada campaña incluye un subconjunto de productos.
- Tres campañas forman una temporada.
- Las temporadas ofrecen promociones adicionales a los embajadores que superen niveles de ventas:
  - $5000, $10,000, $20,000.

### Embajadores
- Los embajadores pueden ser de tres niveles:
  - Plata: Nivel inicial.
  - Oro: Asesoran a embajadores Plata.
  - Platino: Asesoran a embajadores Oro.
- Para subir de nivel, un embajador debe mantener un nivel de ventas por al menos 1 año.
- Cada embajador:
    - Tiene una cartera de clientes y pertenece a una región (con un CEDIS asignado).
    - Puede hacer órdenes personales para adquirir productos a precio de embajador o aprovechar promociones.
    - Establece metas personales de ventas.

#### Beneficios para embajadores:
- Bonificaciones por desempeño:
  - Plata: Acceso a productos en promoción por superar ventas de $5000.
  - Oro: Bono en efectivo por ventas mayores a $10,000.
  - Platino: Acceso a productos exclusivos por ventas superiores a $30,000.
- Recompensas no monetarias:
    - Diplomas y reconocimientos digitales/físicos.
    - Cursos gratuitos en marketing y liderazgo.
    - Invitaciones a eventos exclusivos.
- Concursos de temporada:
    - Los mejores embajadores pueden ganar viajes o kits prémium.
- Planes de antigüedad:
    - Descuentos adicionales y bonos por trayectoria de 2, 5 y 10 años.

### Clientes

De cada cliente se guarda:
- Nombre, teléfonos y direcciones geolocalizadas.
- Un cliente solo puede tener un embajador asignado.
- Un cliente puede:
  - Pagar los pedidos en abonos, siempre y cuando no tenga deudas pendientes mayores a 3 meses.
  - Hacer pedidos a su embajador o directamente en la página web.
  - Los pagos se distribuyen de los pedidos más antiguos a los más nuevos.

### Órdenes y Pedidos
- Los embajadores agrupan los pedidos de sus clientes en órdenes  de compra:
  - Pueden realizar varias órdenes durante una campaña.
  - En órdenes menores al mínimo establecido para su nivel, se cobra un costo de envío.
  - Las órdenes pueden pagarse en abonos, pero no se permite abonar si hay deudas previas.
- Los clientes pueden recibir los productos directamente o a través de su embajador.

### Logística

#### Regiones y CEDIS

El territorio nacional está dividido en regiones logísticas.
- Cada región tiene un CEDIS (Centro de Distribución), que gestiona:
  - Nombre, dirección y geolocalización.
  - Recepción de productos desde la empresa.
  - Almacenamiento de inventario.
  - Procesamiento y envío de órdenes.
- Información del CEDIS:
  - Capacidad máxima de almacenamiento.

#### Procesos logísticos
1. Inventario:
- Cada CEDIS mantiene un inventario actualizado.
- Productos en promoción tienen prioridad de reabastecimiento.
- Procesamiento de órdenes:
  - Órdenes de embajadores: Enviadas al CEDIS de su región.
  - Órdenes de clientes: Procesadas por el CEDIS correspondiente según la región del cliente.
2. Envíos:
- Plazos de entrega: 1-7 días hábiles.
- Costos de envío:
  - Gratuitos si las órdenes superan el mínimo según el nivel del embajador.
3. Rastreo:
- Los pedidos cuentan con un sistema de seguimiento en tiempo real.
4. Optimización del sistema logístico
- Predicción de demanda por región para ajustar inventarios.
- Optimización de rutas para reducir costos de transporte.
- Evaluación de ventas por campaña para planificar reabastecimientos.

### Producción

**Proceso de Producción**
La empresa produce sus propios artículos y gestiona su fabricación con base en:
- Productos: La lista completa de productos manufacturados.
- Recetas de producción: Cada producto tiene una receta que especifica los materiales necesarios y su cantidad.
- Líneas de producción: Fábricas o áreas designadas para fabricar productos específicos.
- Tiempos de producción: El tiempo estimado en horas/días para fabricar cada unidad del producto.
- Costo de producción: Calculado con base en materiales, mano de obra y costos indirectos.

**Materiales**
Los materiales necesarios para la producción incluyen:
- Nombre y descripción del material.
- Unidad de medida (kg, litros, piezas, etc.).
- Costo por unidad.
- Stock actual en el almacén de materias primas.
- Proveedor asignado.

**Gestión de inventario de materias primas**
- Se monitorea el inventario de materiales en los almacenes.
- Si el inventario cae por debajo del mínimo requerido, se genera una orden de compra al proveedor.
- Los materiales son asignados a órdenes de producción según su disponibilidad.

**Órdenes de Producción**
La producción se organiza en órdenes de producción, que incluyen:
- Producto a fabricar.
- Cantidad requerida.
- Fecha de inicio y finalización estimada.
- Línea de producción asignada.
- Estado de la orden: Pendiente, En Proceso, Completada.

Las órdenes se generan con base en:

- La demanda proyectada para las campañas.
- Inventario disponible en los CEDIS.
- Optimización de Producción
- Pronóstico de demanda: Basado en ventas históricas y campañas futuras, se ajusta el volumen de producción.
- Producción escalonada: Para productos de alta demanda o con alta rotación, se producen lotes en intervalos planificados.
- Capacidad de las líneas: Se considera la capacidad diaria de las líneas de producción para evitar cuellos de botella.

**Proveedores**
De cada proveedor se registra:
- Nombre, dirección, datos de contacto.
Materiales que suministra.
- Tiempos de entrega promedio.
- Historial de cumplimiento de órdenes.

**Control de calidad**
Antes de enviar los productos a los CEDIS, se realiza un control de calidad que evalúa:
- Dimensiones, peso, y especificaciones del producto.
- Lotes defectuosos se separan para ser reprocesados o desechados.



### Casos Prácticos
#### Órdenes agrupadas:

- Juan, un embajador nivel Plata, agrupa pedidos de tres clientes y realiza una orden de $950. Se le aplica un costo de envío de $100. Recibe los productos en 5 días.

#### Promoción para embajadores:

- Rosa López, nivel Plata, alcanza $12,000 en ventas y adquiere productos en promoción. Posteriormente, revende uno de ellos a precio normal.

#### Adeudos de clientes:

- Sandra Bullrock detecta que Javier Quezada no ha pagado un pedido de hace 3 meses. El cliente no puede realizar más compras hasta que regularice su deuda.

#### Devolución:

- Cristina Van Rankin devuelve un producto defectuoso y recibe el reemplazo en 3 días.

#### Demanda regional:

- En la región norte, el CEDIS recibe reabastecimientos prioritarios para productos de limpieza debido a su alta demanda.

#### Producción

1. Falta de Materiales Críticos:

  - La línea de producción de "Loción en Gel My Precious" se detiene porque el inventario de aceite esencial de lavanda cae por debajo del mínimo requerido.
  - El sistema genera automáticamente una orden de compra al proveedor asignado, con un plazo de entrega estimado de 3 días.
  - Mientras tanto, el equipo de producción reorganiza la planificación para priorizar productos que no dependen de ese material.

2. Producción Escalonada por Temporada:

  - Para la campaña "Verano Fresco", el sistema proyecta una alta demanda de la "Colonia TW9 100ml".
  - Se emiten 3 órdenes de producción escalonadas para fabricar 10,000 unidades:
    - Primera orden: 4,000 unidades (completadas en mayo).
    - Segunda orden: 4,000 unidades (junio).
    - Última orden: 2,000 unidades (julio, para cubrir posibles pedidos tardíos).

3. Control de Calidad:

   - En una revisión de un lote de "Baterías de Cocina Titanio", el equipo de calidad detecta que 20 unidades presentan rayones.
   - Las unidades defectuosas se separan y el sistema registra el lote como "Parcialmente Aceptado", mientras el resto se envía al CEDIS.
   - El equipo de producción reprograma la fabricación de 20 unidades adicionales para reponer las dañadas.

4. Optimización de Costos:

- Durante la campaña "Amor en Tiempos del Covid", el sistema sugiere ajustar la receta de "Talco Corporal Perfumado" reemplazando un material por otro de igual calidad, pero con menor costo.
- El cambio es aprobado, reduciendo el costo de producción en un 5% sin afectar las ventas.

5. Demanda no prevista:

- Un artículo nuevo, "Organizador Multifuncional", tiene una demanda 30% mayor a lo proyectado en su primera campaña.
- El sistema detecta el agotamiento del inventario en los CEDIS y genera una orden de producción urgente.
- El área de producción reorganiza las líneas y fabrica 5,000 unidades adicionales en 2 semanas.

6. Pronóstico Erróneo:

- Un exceso de inventario de "Velas Aromáticas Pure Serenity" tras la campaña "Otoño Místico" obliga a la empresa a realizar ajustes.
- Las velas restantes se redistribuyen a las siguientes campañas como productos en promoción, lo que ayuda a minimizar pérdidas.

7. Pedidos Especiales:

- Un gran cliente solicita 1,000 unidades personalizadas del "Eau d’parfum".
- Se genera una orden de producción específica con su propio número de lote.
- La producción se prioriza, y el cliente recibe el pedido en tiempo y forma.

## Historias de Validación

### Historia 1: La embajadora estrella y su ascenso meteórico
Sofía Herrera inicia como embajadora Plata en enero de 2024 en la región Norte. En su primera campaña logra $6,200 en ventas personales y recluta a 3 nuevas embajadoras bajo su mentoreo. Durante la temporada "Primavera Radiante" (campañas 4-6), sus ventas explotan: $12,500, $18,300 y $25,400 respectivamente, superando todas las metas y ganando bonificaciones en efectivo. Por su desempeño excepcional, asciende a nivel Oro en agosto y recibe una cartera de 15 embajadoras Plata para asesorar. Sin embargo, en la temporada "Otoño Elegante", 5 de sus asesoradas renuncian por presión de ventas, 3 clientes importantes se quejan de entregas tardías, y sus propias ventas bajan a $8,900 promedio por campaña. Para diciembre debe decidir si mantiene su nivel Oro o acepta regresar a Plata con menos responsabilidades pero metas más alcanzables.

**Pregunta para validar:** ¿Cómo registrarías la progresión de niveles de una embajadora, el manejo de equipos bajo mentoreo, el cálculo de bonificaciones por múltiples conceptos, y la posible degradación de nivel por bajo rendimiento?

### Historia 2: La crisis logística del CEDIS Occidente durante temporada alta
Durante la temporada "Navidad Mágica", el CEDIS Occidente (que atiende 8 estados) enfrenta una crisis perfecta: un incendio menor daña 30% del almacén, el proveedor principal de envases cosméticos quiebra dejando 15,000 unidades sin empacar, y una huelga de transportistas locales retrasa entregas por 10 días. La situación afecta a 450 embajadoras y 12,000 clientes finales. La gerencia implementa un plan de contingencia: redistribuye inventario desde los CEDIS Norte y Sur, contrata una empresa de paquetería externa con 40% más costo, habilita 3 centros de distribución temporales en tiendas asociadas, y permite que embajadoras Gold recojan pedidos directamente de fábrica. El proceso de recuperación toma 6 semanas, cuesta $350,000 extra, pero se logra cumplir con el 85% de entregas navideñas. Como compensación, se otorgan créditos a clientes afectados y bonificaciones extraordinarias a embajadoras que perdieron ventas.

**Pregunta para validar:** ¿Cómo manejarías una crisis logística con redistribuición de inventario entre múltiples CEDIS, costos extraordinarios de envío, centros temporales de distribución, y el sistema de compensaciones masivas?

### Historia 3: El cliente problemático y la cadena de pagos complicada
Margarita Vásquez, cliente de la embajadora Carmen López, tiene un historial de pagos complejo: debe $2,400 de pedidos de las últimas 3 campañas, pero quiere hacer un pedido nuevo de $1,800 para regalos de Día de las Madres. Las políticas de TrumpetWare prohíben nuevos pedidos con deudas mayores a 3 meses, pero Margarita ofrece un plan: pagar $800 inmediatos, $600 a los 15 días, y el resto en abonos de $200 mensuales. Paralelamente, su hija también es cliente de otra embajadora y quiere transferir su cuenta a Carmen para "consolidar pagos familiares". La situación se complica cuando Margarita reclama que 3 productos de su último pedido llegaron defectuosos, pero ya los había usado parcialmente. Carmen debe navegar entre las políticas corporativas, mantener la relación cliente, gestionar devoluciones parciales, y crear un plan de pagos que satisfaga a ambas partes mientras protege sus propias comisiones.

**Pregunta para validar:** ¿Cómo registrarías un historial complejo de deudas con planes de pago personalizados, transferencia de clientes entre embajadoras, devoluciones de productos parcialmente usados, y la protección de comisiones durante disputas?

### Historia 4: La campaña "Edición Limitada" y el caos de inventario
TrumpetWare lanza la campaña especial "Tesoros Dorados" con 8 productos de edición limitada disponibles solo durante 2 semanas. La demanda explota: en las primeras 48 horas se reciben pedidos por 25,000 unidades cuando solo se produjeron 15,000. El sistema de inventario no logra actualizar en tiempo real, permitiendo que 200 embajadoras confirmen pedidos de productos ya agotados. La crisis se amplifica cuando se descubre que la línea de producción del "Set de Brochas Doradas" tiene un defecto que afecta al 40% de las unidades producidas. La empresa debe: cancelar 5,000 pedidos confirmados, ofrecer productos sustitutos con descuento del 20%, reprogramar producción urgente de 3,000 unidades adicionales, crear un sistema de lista de espera con prioridades, y compensar a 150 embajadoras que perdieron ventas por productos no disponibles. La situación genera 300 reclamaciones de clientes y obliga a replantear el sistema de gestión de inventario en tiempo real.

**Pregunta para validar:** ¿Cómo manejarías sobreventa de productos con inventario limitado, cancelaciones masivas de pedidos confirmados, productos sustitutos con descuentos especiales, listas de espera con prioridades, y la gestión de reclamaciones masivas?

### Historia 5: La reorganización territorial y el cambio de embajadoras
Por optimización logística, TrumpetWare decide fusionar las regiones Centro y Bajío, cerrando el CEDIS Bajío y reubicando todo en el CEDIS Centro ampliado. El cambio afecta a 280 embajadoras y 8,500 clientes activos. Durante la transición de 3 meses surgen múltiples complicaciones: 45 embajadoras solicitan cambio de región para mantener proximidad con sus clientes, 12 embajadoras Oro pierden parte de su equipo asesorado que se reasigna a otras mentoras, los tiempos de entrega aumentan temporalmente de 3 a 7 días en ciertas zonas, y 150 clientes solicitan cambio de embajadora asignada por la nueva distancia. Adicionalmente, el nuevo CEDIS requiere 15 empleados adicionales, nuevo software de ruteo optimizado, y renegociación de contratos con 8 empresas de paquetería local. Al final de la transición, se logra reducir costos operativos en 12%, pero se pierden 35 embajadoras y 400 clientes activos por inconformidad con los cambios.

**Pregunta para validar:** ¿Cómo registrarías una reorganización territorial masiva con reasignación de embajadoras y clientes, cambios en jerarquías de mentoreo, modificación de centros de distribución, y el seguimiento de la retención vs abandono durante la transición?

### Historia 6: El lanzamiento del producto estrella y la competencia desleal
TrumpetWare invierte $500,000 en desarrollar "Serum Regenerador Platinum", su producto más innovador con 18 meses de investigación. El lanzamiento en la campaña "Belleza Infinita" es espectacular: 15,000 unidades vendidas en la primera semana, trending en redes sociales, y reconocimiento de influencers de belleza. Sin embargo, a las 3 semanas aparece en el mercado "Golden Repair Serum" de la competencia, con fórmula prácticamente idéntica y precio 30% menor. La investigación revela que un ex-empleado de producción vendió la fórmula, y que 2 embajadoras Platino están promocionando secretamente el producto de la competencia a sus clientes. TrumpetWare debe: iniciar acciones legales por robo de propiedad intelectual, investigar la filtración interna, separar de la red a las embajadoras desleales, lanzar una campaña de marketing defensiva, ofrecer descuentos temporales para mantener competitividad, y rediseñar protocolos de seguridad en investigación y desarrollo. El incidente resulta en $200,000 en gastos legales y pérdida del 25% de las ventas proyectadas del producto estrella.

**Pregunta para validar:** ¿Cómo manejarías el seguimiento de desarrollo de productos con costos de investigación, competencia desleal con productos copiados, investigación interna de filtración de información, separación de embajadoras por violación de exclusividad, y el impacto financiero completo del incidente?