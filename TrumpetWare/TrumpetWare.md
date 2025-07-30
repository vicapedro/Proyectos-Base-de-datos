# TrumpetWare

## Descripción General
TrumpetWare es un fabricante de productos de belleza y del hogar que distribuye a través de embajadores. Debido al crecimiento reciente, es necesario diseñar una Base de Datos para soportar una **Mobile App** y una **Web App** que permitan gestionar las ventas, pedidos y embajadores. Este caso práctico detalla los requisitos de la empresa.

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
