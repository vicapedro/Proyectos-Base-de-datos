# Pawfect Care
Empresa que ofrece el serivioc de Hotel de Cuidado de Mascotas con Venta y Servicios Adicionales

## Descripción
### Gestión de Mascotas
El sistema debe permitir registrar las mascotas que están bajo el cuidado del hotel, incluyendo nombre, especie, raza, edad, historial médico (vacunas, alergias), comportamiento y características especiales. Además, debe registrar la mascota como huésped del hotel o como mascota en venta, y actualizar el historial médico de cada mascota (vacunas, tratamientos, enfermedades). También debe gestionar la disponibilidad de mascotas en el hotel, ya sea para cuidado, venta o como mascotas de compañía.

### Gestión de Clientes
El sistema debe gestionar la información de los dueños de mascotas (nombre, dirección, contacto) y asociarlos con sus mascotas. Además, debe mantener un historial de reservas, compras y contratos de alquiler de mascotas.

### Gestión de Reservas de Cuidado
El sistema debe gestionar la reserva de espacios para el cuidado temporal de mascotas, registrando fechas de entrada y salida, servicios requeridos (alimentación, paseo, aseo) y costos asociados. También debe ofrecer servicios adicionales como baños, entrenamiento y asistencia veterinaria, que se puedan añadir a las reservas de cada mascota.

### Gestión de Ventas de Productos y Mascotas
El sistema debe gestionar un inventario de productos (alimentos, juguetes, accesorios, medicinas) y mantener el stock actualizado. Además, debe gestionar las transacciones de venta de productos, registrando la información del cliente, productos comprados, cantidades y pagos. También debe permitir la venta de mascotas disponibles en el hotel, con información detallada sobre cada mascota (especie, raza, edad, estado de salud).

### Servicio de Mascotas de Compañía
El sistema debe registrar las mascotas que están disponibles para el servicio de compañía temporal, incluyendo estado de salud, especie, raza, edad, comportamiento y disponibilidad. Además, debe permitir la creación y gestión de contratos de alquiler para las mascotas de compañía, incluyendo fechas de inicio y fin, cliente asociado, mascota asignada, tarifas y estado del contrato (activo, completado, cancelado). También debe registrar el historial de cada mascota de compañía, con detalles de los clientes que la han alquilado y las fechas del servicio.

### Facturación y Pagos
El sistema debe generar facturas automáticamente para todas las transacciones, ya sea de servicios de cuidado, ventas de productos, ventas de mascotas o contratos de alquiler de mascotas de compañía. Además, debe soportar múltiples tipos de pagos (efectivo, tarjeta de crédito, transferencias electrónicas) y registrar un historial de todos los pagos realizados por cada cliente.

## Historias de Validación

### Historia 1: La llegada de Max
Carmen Rodríguez llama por teléfono para reservar hospedaje para su Golden Retriever llamado Max durante sus vacaciones del 15 al 25 de marzo. Max tiene 3 años, está vacunado contra rabia y parvovirus (última vacuna el 10 de enero), es alérgico al pollo y necesita medicamento para la artritis cada 12 horas. Carmen solicita servicio de paseos diarios y baño antes de recogerlo. El precio base son $300 por día, más $50 por paseo diario y $150 por el baño. Carmen paga $500 de anticipo con tarjeta de crédito y programan el pago del resto al momento de la entrega.

**Pregunta para validar:** ¿Cómo registrarías toda esta información y asegurarías que Max reciba sus cuidados especiales durante su estancia?

### Historia 2: La venta de Luna
Los hermanos García visitan Pawfect Care buscando adoptar una mascota. Se interesan por Luna, una gatita persa de 6 meses que está disponible para venta. Luna fue encontrada abandonada hace 2 meses, ha recibido todas sus vacunas, está desparasitada y esterilizada. Su precio es de $2,500. Los hermanos deciden llevarla y además compran: una caja transportadora ($450), arena para gato ($120), alimento premium para gatitos ($280) y juguetes ($150). Pagan todo en efectivo y solicitan factura a nombre de "Hogar García" con RFC: GAHO860125XXX.

**Pregunta para validar:** ¿Cómo procesarías esta venta mixta (mascota + productos) y generarías la documentación fiscal correcta?

### Historia 3: El servicio de compañía para la Sra. Elena
La Sra. Elena Martínez, de 75 años, vive sola y ha solicitado el servicio de mascota de compañía. Necesita un perro tranquilo y cariñoso que la acompañe de lunes a viernes de 9:00 AM a 6:00 PM durante todo el mes de abril. Le asignan a Toby, un Labrador senior de 8 años, muy dócil y entrenado para compañía de adultos mayores. El servicio cuesta $200 por día. Durante la segunda semana, Elena llama para reportar que Toby no está comiendo bien. Pawfect Care envía al veterinario de confianza, quien diagnostica un malestar estomacal menor y receta medicamento. El tratamiento veterinario ($350) se añade a la factura de Elena.

**Pregunta para validar:** ¿Cómo manejarías el contrato de compañía, el seguimiento de la salud de Toby y los costos adicionales no previstos?

### Historia 4: La emergencia de Rocco
Es sábado por la noche cuando Roberto Vega llega urgentemente con su Bulldog Francés, Rocco. Rocco tiene dificultades para respirar y necesita atención veterinaria inmediata. No tienen cita previa, pero Pawfect Care acepta la emergencia. El veterinario de guardia examina a Rocco y determina que necesita oxígeno y medicamentos durante toda la noche. Roberto autoriza el tratamiento ($1,200) y decide dejar a Rocco hospitalizado hasta el lunes. Durante su estancia, Rocco requiere cuidados intensivos ($400 por día) y una segunda consulta veterinaria el domingo ($300). Roberto paga todo con tarjeta de crédito al recoger a Rocco el lunes.

**Pregunta para validar:** ¿Cómo registrarías esta situación no planificada, los múltiples servicios añadidos y asegurarías el seguimiento médico correcto?

### Historia 5: El paquete familiar de los Mendoza
La familia Mendoza trae tres mascotas para cuidado durante dos semanas: Bruno (Pastor Alemán de 5 años), Mia (gata siamesa de 2 años) y Kiwi (loro amazónico de 10 años). Bruno necesita ejercicio intenso diario y está a dieta (alimento especial sin granos). Mia es muy territorial y debe estar en un espacio separado de otros gatos. Kiwi requiere interacción social constante y una dieta específica de frutas y semillas. Los Mendoza también compran alimento especial para Bruno (3 bolsas de $180 cada una) y semillas para Kiwi ($95). El costo total es $8,450. Pagan $3,000 de anticipo en efectivo y el resto lo programan en tres pagos quincenales con tarjeta.

**Pregunta para validar:** ¿Cómo organizarías el cuidado individualizado de cada mascota y manejarías el esquema de pagos programados?

### Historia 6: El regalo sorpresa
María José quiere sorprender a su novio Pablo con una mascota por su cumpleaños. Compra a Charlie, un hamster ruso de 3 meses ($150), junto con una jaula completa ($320), rueda de ejercicio ($45), casa pequeña ($35), alimento ($40) y juguetes ($60). Como es regalo, solicita que todo se entregue el día del cumpleaños (jueves 18) en la dirección de Pablo, no en la suya. María José paga todo por adelantado con transferencia bancaria y solicita que incluyan una tarjeta de felicitación. El jueves, cuando llegan a entregar, Pablo no está en casa, pero su hermano acepta recibir todo y firma de recibido.

**Pregunta para validar:** ¿Cómo manejarías una venta con entrega a domicilio a una dirección diferente del comprador y validarías la entrega correcta?

