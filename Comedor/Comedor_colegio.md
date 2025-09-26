# Comedor del Colegio Pink Floyd

El “Colegio Pink Flor” con kínder y primaria busca mejorar sus servicios y lo han contratado a usted para desarrollar el sistema computacional que controle el servicio de comedor que ofrece a sus alumnos de lunes a viernes. 

Inicialmente el sistema es independiente del resto de los que posee el colegio, por lo tanto, necesita guardar información sobre los niños: su nombre, edad, nivel y grado, alergias alimenticias; del padre o tutor: su nombre, teléfono celular, teléfono y lugar de trabajo. 

El nutriólogo ha seleccionado cuidadosamente cientos de alimentos para el área de cocina. Para cada alimento se tiene una Receta que describe el procedimiento e ingredientes para preparar una cantidad de porciones. 

Cada semana el nutriólogo diseña un menú del cual los padres pueden seleccionar lo que comerán sus hijos. El menú consiste de al menos 7 opciones de comida, 7 bebidas y 7 postres, para cada una de ellas el nutriólogo calcula las calorías, carbohidratos, grasas y proteínas. Sobre los ingredientes de los alimentos, es importante identificar aquellos que son alergénicos. El nutriólogo puede reutilizar menúes. 

Con al menos 3 días de anticipación, el padre puede seleccionar los alimentos que recibirán sus hijos, que puede pagar en el momento o en abonos. Es necesario pues llevar un control de pagos. 

Los lunes y miércoles se hacen las compras de los ingredientes, es importante generar la lista de compras, considerando lo que se ha utilizado y aún queda en la cocina. De cada día de la semana se contabiliza cuantos niños recibirán cada comida específica. De cada comida se prepararán un múltiplo de las porciones que especifica la receta. La cantidad de cada ingrediente se multiplica por este factor. 
 
El niño come sólo lo que el padre apruebe del menú. Los niños pueden ser alérgicos a ciertos ingredientes, por lo cual es importante conocer sus alergias alimentarias. 

## Ejemplos

### Ejemplo 1 
Actualmente es la semana 20 y los padres pueden seleccionar de este menú:

| Comida	| Bebida	| Postre |
|-----------|-----------|--------|
|Mole poblano	|Agua de melón	|Gelatina sabores varios|
|Ceviche de soya	|Agua de sandía	|Pastel de 3 leches|
|Verduras al vapor con puré de papa	|Agua de jamaica	|Flan|
|Tacos de carne asada	|Limonada	|Fruta picada|
|Tamales de verdura	|Agua de piña	|Frutos rojos|
|Enchiladas verdes	|Agua de pepino	|Mangoneadas|
|Pollo a la plancha	|Agua de horchata	|Pastel de chocolate|

### Ejemplo 2
El señor Ramírez tiene 2 hijos, no se quiere complicar y ordena lo mismo para sus hijos; paga el total:

Órdenes de Juan para la semana 21
| Día	| Comida	| Bebida	| Postre |
|-------|-------|-------|-------|
| **Lunes**	| Tacos de carne asada|	Agua de horchata	| Frutos rojos|
| **Martes**	| Mole poblano	| Agua de pepino	| Mangoneadas|
| **Miércoles**	| Enchiladas verdes| Agua de jamaica	| Pastel de chocolate|
| **Jueves**	| Tamales de verdura	| Agua de piña	| Frutos rojos|
| **Viernes**	| Ceviche de soya| Agua de melón| Flan|

### Ejemplo 3 

El nutriólogo registra una nueva comida: 

**Crêpes salados**


 **Ingredientes** (Para 5 porciones)
 
- Harina de garbanzo: 110 g
- Agua: 250 ml
- Aceite de oliva virgen extra: 15 ml
- Sal: 2 g
- Cebollino: 10 gramos
- Pimienta negra molida: 1 gramo
- Aguacate: 1
- Cebolla morada: 1
- Pimiento rojo picante o dulce: 1  

**Preparación:**

Disponer la harina de garbanzos en un cuenco o jarra con el agua…

… Continuar hasta terminar con toda la masa, rellenar con los ingredientes preparados y servir.
</td></tr>

### Ejemplo 4
Ana Flérida está en la fila, es su turno, pone su credencial de la escuela en el sensor, en su pantalla y la de la barra aparece su orden para ese día. Marko le sirve, le entrega y oprime el botón de entregado.

## Historias de Validación

### Historia 1: La crisis alérgica de la semana 15
Durante la semana 15, se presenta una situación crítica: la mamá de Sofía Martínez (3° grado) reporta que su hija desarrolló una nueva alergia al huevo, pero ya había pagado y seleccionado sus comidas para toda la semana, incluyendo "Pastel de 3 leches" (martes), "Flan" (jueves) y "Crêpes salados" (viernes), todos con huevo en sus ingredientes. Paralelamente, 3 niños más reportan alergias nuevas: Luis a los lácteos, Carmen a los frutos secos y Diego al gluten. El nutriólogo debe revisar urgentemente todas las recetas de la semana, identificar ingredientes problemáticos y ofrecer sustitutos. Se crean versiones alternativas de 8 recetas diferentes: flan sin huevo, crêpes de avena, pastel vegano, etc. Los padres afectados pueden cambiar sus selecciones sin costo adicional, pero algunos requieren reembolsos parciales. Al final, se atiende a 12 niños con restricciones alimentarias especiales esa semana.

**Pregunta para validar:** ¿Cómo manejarías cambios de último minuto por alergias nuevas, sustitución de recetas con ingredientes alternativos, reembolsos parciales y la creación de menús alternativos para niños con restricciones?

### Historia 2: El día del festejo y la orden masiva
Para celebrar el Día del Niño, la directora decide ofrecer un menú especial gratuito para todos los 450 alumnos del colegio. El menú incluye: "Tacos de carnitas" como plato fuerte, "Agua de jamaica" como bebida y "Pastel de chocolate" de postre. Sin embargo, surgen complicaciones: la receta original de tacos es para 5 porciones y necesitan 450, el proveedor de carne solo puede entregar 30 kg (necesitan 45 kg), el chocolate para el pastel está agotado en 2 proveedores locales, y 15 niños tienen restricciones que impiden comer el menú especial. El nutriólogo debe: calcular ingredientes para 90 porciones de tacos (18 veces la receta base), encontrar proveedores alternativos urgentes, crear 15 menús individuales especiales para niños con alergias, y coordinar con 8 cocineros trabajando en doble turno. La celebración es exitosa, pero los costos superan el presupuesto en 40%.

**Pregunta para validar:** ¿Cómo registrarías un evento especial con escalamiento masivo de recetas, búsqueda urgente de proveedores alternativos, menús individualizados para casos especiales y el control de costos extraordinarios?

### Historia 3: La semana de los pagos atrasados y las restricciones
En la semana 22, 35 familias tienen pagos atrasados por diferentes montos y períodos. La política del colegio es clara: sin pago al día, no hay servicio de comedor. Sin embargo, surgen situaciones especiales: la familia González tiene 3 hijos y debe $1,200 de 2 semanas, pero la mamá perdió su trabajo; los gemelos Rodríguez necesitan comida especial por diabetes, pero sus papás están en proceso de divorcio y ninguno quiere pagar; la familia Morales pide plan de pagos porque el papá está hospitalizado. El administrador debe: generar reportes de morosos por días y montos, crear planes de pago especiales para 8 familias, coordinar con trabajo social del colegio para 5 casos vulnerables, y gestionar 12 niños que llegan sin orden pero necesitan comer. Se implementa un sistema de crédito temporal y vale de emergencia que permite a niños en situación crítica recibir una comida básica mientras se resuelve su situación.

**Pregunta para validar:** ¿Cómo manejarías múltiples estados de pago atrasado, planes de pago personalizados, casos sociales especiales, sistema de crédito temporal y la generación de reportes de cobranza?

### Historia 4: La intoxicación alimentaria y la investigación
El miércoles de la semana 18, 8 niños de diferentes grados presentan síntomas de intoxicación alimentaria después del almuerzo. Todos habían consumido "Ceviche de soya" y "Agua de sandía". Se inicia una investigación urgente: revisar el lote de ingredientes utilizado, identificar a todos los niños que consumieron estos alimentos (32 en total), contactar a todos los padres afectados, coordinarse con el departamento de salud, y suspender temporalmente estos alimentos del menú. La investigación revela que el proveedor de soya entregó un lote contaminado, y la sandía no se lavó adecuadamente. Se debe: reemplazar todos los menús que incluían estos ingredientes por el resto de la semana, ofrecer revisión médica gratuita a los 32 niños expuestos, implementar nuevos protocolos de higiene, cambiar de proveedor de soya, y manejar 12 reclamaciones de padres preocupados. El incidente resulta en nuevas políticas de trazabilidad de ingredientes y protocolos de respuesta a emergencias.

**Pregunta para validar:** ¿Cómo rastrearías todos los niños que consumieron alimentos específicos, manejarías una suspensión temporal de ingredientes, implementarías cambios de menú de emergencia y documentarías el protocolo de respuesta a crisis alimentarias?

### Historia 5: La semana de la feria de ciencias y los horarios especiales
Durante la semana 25, el colegio organiza su feria anual de ciencias con horarios modificados: algunos grados almuerzan a las 11:30 AM, otros a la 1:30 PM y los de kínder mantienen su horario normal de 12:30 PM. Además, llegan 120 visitantes externos (padres, jueces, invitados especiales) que también necesitan almorzar. El nutriólogo debe: adaptar las cantidades de cada receta para 3 horarios diferentes, crear un menú especial para visitantes (algunos son vegetarianos, otros veganos), coordinar con 6 cocineros para preparar comidas en lotes escalonados, gestionar el inventario para que no falten ingredientes en ningún horario, y manejar 15 cambios de último minuto de padres que decidieron acompañar a sus hijos. La cocina trabaja desde las 7:00 AM hasta las 3:00 PM sin parar, se utilizan 3 veces más ingredientes de lo normal, y se sirven 690 comidas en total en lugar de las 280 habituales.

**Pregunta para validar:** ¿Cómo coordinarías múltiples horarios de servicio, escalamiento variable de recetas por horario, menús especiales para visitantes externos, y el control de inventario con demanda triplicada en un solo día?

### Historia 6: El cambio de nutriólogo y la transición de menús
En la semana 30, la nutrióloga Dra. Patricia Vega renuncia y es reemplazada por el Dr. Carlos Hernández, quien tiene una filosofía alimentaria completamente diferente. El Dr. Hernández quiere: eliminar todos los postres con azúcar refinada, introducir 15 recetas veganas nuevas, cambiar 8 proveedores por otros más orgánicos (pero más caros), modificar las porciones según nuevos estándares nutricionales, y rediseñar completamente el sistema de menús semanales. Sin embargo, ya hay 200 familias que pagaron por 3 semanas de menús con el sistema anterior. Se debe: honrar los menús ya pagados mientras se implementan los cambios gradualmente, capacitar a 5 cocineros en las nuevas recetas, negociar precios con 8 proveedores nuevos, comunicar los cambios a 280 familias, manejar 45 quejas de padres que prefieren el sistema anterior, y ajustar 25 casos de niños con alergias a las nuevas recetas. La transición toma 6 semanas completas y requiere mantener ambos sistemas funcionando simultáneamente.

**Pregunta para validar:** ¿Cómo manejarías una transición completa de sistema de menús, mantenimiento de compromisos previos, capacitación de personal, cambio masivo de proveedores, y la gestión de resistencia al cambio de los usuarios?   
