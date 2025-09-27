# Salud y Vida - Atención que entiende a tu familia

## Introducción
Salud y Vida es una clínica que ofrece servicios médicos integrales, incluyendo atención primaria, especialidades médicas, análisis clínicos, imagenología y farmacia. Su objetivo es proporcionar atención de calidad a sus pacientes y facilitar el acceso a servicios médicos especializados.


En **Salud y Vida** se necesita un sistema integral para administrar toda la información relativa a los servicios que ofrece, aunque inicialmente será solo una parte. Le han pedido diseñe una base de datos que satisfaga sus necesidades de control de la información.

Para Salud y Vida, los clientes son importantes, son los que solicitan servicios de la clínica para sí mismos o para sus familiares, por lo cual se necesita conocer su nombre, apellidos, dirección y teléfono. Un cliente puede tener asociados a varios dependientes.

Los pacientes pueden llegar a ventanilla y solicitar diferentes servicios o agendar una cita por teléfono o por la web app.

El paciente llega a consulta con un médico general, el cual pregunta sobre los síntomas actuales y en caso de ser necesario realiza un examen físico. Si es la primera vez que asiste a Salud y Vida, le realiza también una serie de preguntas sobre sus antecedentes médicos, familiares y sociales, así como sobre cualquier tratamiento previo, incluyendo enfermedades pasadas, cirugías, alergias y medicamentos que esté tomando. En resumen hechos de salud del pasado y del problema actual.

Si el médico puede diagnosticar con esta información puede indicar un tratamiento que puede ser una serie de indicaciones o medicamentos, en cuyo caso emite una receta. En algunos casos lo puede derivar a un médico especialista de Salud y Vida o externo, en cuyo caso es dado de alta. 

Cualquiera de los médicos puede necesitar mas información para disgnosticar, por lo que puede ordenar algún procedimiento extra: análisis clinicos, biopsias o estudios de imagenología(rayos X, tomografía, resonancia, etc).

El personal medico de Salud y Vida está compuesto por doctores empleados y doctores independientes.
- **Doctores empleados**: Tienen relación laboral directa, salario, prestaciones y horarios fijos.
- **Doctores independientes** (renta de consultorio): Pagan renta, pueden tener agenda propia, y la clínica cobra comisión por consulta o servicios.

La receta es una lista de medicamentos, dosis, frecuencia, duración e indicaciones. Al imprimirse, lleva el nombre, firma y cédula del médico.

La receta se surte en la farmacia de Salud y Vida. El dependiente verifica la receta, si es de Salud y Vida la coteja con el sistema. Si es de un médico externo, el dependiente verifica que la receta sea válida y surte los medicamentos.




### Presentación de medicamentos y cálculo de entrega

Es necesario llevar un control del inventario de medicamentos. 

El sistema debe registrar la presentación de cada medicamento (por ejemplo, tabletas, cápsulas, frascos, miligramos por unidad, etc.) y su contenido por empaque. Al momento de surtir una receta, el sistema debe calcular automáticamente la cantidad total de medicamento necesaria para cubrir la dosis, frecuencia y duración del tratamiento indicado por el médico.

Con base en estos datos, el sistema sugerirá al dependiente el número exacto de cajas, frascos o unidades que debe entregar al paciente, procurando siempre entregar empaques completos y evitando fraccionamientos innecesarios. Además, el sistema debe advertir si el inventario es insuficiente para surtir la receta completa y permitir registrar entregas parciales si es necesario.


Todos los servicios de Salud y Vida se proporcionan independientemente si la orden es de un médico interno o externo. Se debe pagar antes de recibir el servicio. Los servicios de análisis clínicos e imagenología pueden ser consultados por los médicos o los clientes a través del sistema. A los clientes se les entrega y envía por email un comprobante con un número de servicio y una contraseña. Por email también se incluye una URL para facilidad de acceso *(Nota: esta URL no se guarda en la base de datos. Esto es para otra materia)*.

Un paciente registrado mayor de edad puede consultar toda su información a través de la web app. Un cliente puede hacerlo de sus dependientes menores de edad. 

Un cliente puede agregar a sus dependientes y todos los cargos derivados de atenderlos serán a su cuenta, aunque el paciente puede pagar también. *(Mejorar redacción)*

*Pendiente: Hospitalización y cirujías**


## Análisis clínicos

Los resultados de los análisis llevan la siguiente información:

**Identificación del Laboratorio:**
- Nombre y dirección del laboratorio.
- Información de contacto (teléfono, correo electrónico).

**Identificación del Paciente:**
- Nombre completo.
- Documento de identidad.
- Edad y sexo.
- Número de historia clínica o expediente.

**Fecha y Hora:**
- Fecha y hora de la toma de muestra.
- Fecha y hora de emisión del reporte.

**Detalles del Análisis:**
- Nombre del análisis realizado.
- Método utilizado para el análisis.
- Resultados obtenidos con sus respectivas unidades de medida.

**Valores de Referencia:**
- Rangos normales o valores de referencia para cada análisis.
- Comparación de los resultados del paciente con los valores de referencia.

**Interpretación de Resultados:**
- Comentarios o interpretaciones del médico o especialista del laboratorio.
- Observaciones adicionales relevantes para la interpretación de los resultados.

**Responsable del Análisis:**
- Nombre y firma del profesional que realizó el análisis.
- Número de cédula profesional.

**Observaciones Adicionales:**
Cualquier información adicional que pueda ser relevante para el diagnóstico o tratamiento del paciente.

Estos elementos aseguran que los resultados sean precisos, comprensibles y útiles tanto para los pacientes como para los profesionales de la salud

## Imagenología

Los servicios de imagenología que se ofrecen son: 
- Rayos X
- Tomografía Computarizada (TC)
- Resonancia Magnética (RM)
- Ultrasonido (Ecografía)
- Mamografía
- Densitometría Ósea

Un estudio de imagenología incluye varios elementos clave para asegurar una evaluación precisa y completa del paciente.

**Identificación del Paciente:**
- Nombre completo.
- Documento de identidad.
- Edad y sexo.
- Número de historia clínica o expediente.

**Detalles del Estudio:**
- Tipo de estudio realizado (radiografía, tomografía computarizada, resonancia magnética, ultrasonido, etc.).
- Fecha y hora del estudio.
- Indicación clínica o motivo del estudio.

**Descripción Técnica:**
- Parámetros técnicos utilizados (por ejemplo, dosis de radiación, tipo de contraste utilizado).
- Protocolo de adquisición de imágenes.

**Imágenes Obtenidas:**
- Imágenes en diferentes planos y cortes según el tipo de estudio.
- Anotaciones o marcas en las imágenes para resaltar áreas de interés.

**Informe del Técnico:**
- Descripción detallada de los hallazgos observados en las imágenes.
- Interpretación de los hallazgos en el contexto clínico del paciente.
- Diagnóstico diferencial si es necesario.
- Recomendaciones para estudios adicionales o seguimiento.

**Conclusión:**
- Resumen de los hallazgos más importantes.
- Diagnóstico final si es posible.

**Firma y Credenciales:**
- Nombre y firma del radiólogo responsable del informe.
- Número de cédula profesional.

## Servicios médicos

En Salud y Vida se ofrecen diferentes servicios médicos que aseguran que los pacientes reciban una atención integral y especializada según sus necesidades.

**Medicina General:**
Atención primaria y seguimiento de pacientes con diversas condiciones de salud.

**Pediatría:**
Cuidado de la salud de los niños y adolescentes.

**Ginecología y Obstetricia:**
Salud reproductiva de la mujer, incluyendo embarazo, parto y enfermedades ginecológicas.

**Cardiología:**
Diagnóstico y tratamiento de enfermedades del corazón y el sistema circulatorio.

**Dermatología:**
Tratamiento de enfermedades de la piel, cabello y uñas.

**Endocrinología:**
Manejo de trastornos hormonales y enfermedades del sistema endocrino, como diabetes y problemas de tiroides.

**Gastroenterología:**
Diagnóstico y tratamiento de enfermedades del sistema digestivo.

**Ortopedia:**
Tratamiento de lesiones y enfermedades del sistema musculoesquelético.

**Neurología:**
Diagnóstico y tratamiento de enfermedades del sistema nervioso.

**Psiquiatría:**
Tratamiento de trastornos mentales y emocionales.

**Oftalmología:**
Cuidado de la salud visual y tratamiento de enfermedades oculares.

**Urología:**
Tratamiento de enfermedades del sistema urinario y, en hombres, del sistema reproductor.

## Reportes

- Los médicos deben poder ver las citas que tienen programadas por día y por semana
- Reporte de Inventario de medicamentos por categoría
- Ingresos por especialidad por doctor

## Historias de Validación

### Historia 1: La urgencia de la Sra. María
La Sra. María González llega sin cita a las 2:00 PM con dolor fuerte en el pecho. La recepcionista la registra como nueva paciente: 45 años, vive en Col. Centro #123, teléfono 811-555-0987, sin alergias conocidas. El Dr. Ramírez (médico general) la atiende inmediatamente. Después del examen inicial, ordena electrocardiograma, análisis de sangre (troponinas, CPK) y radiografía de tórax. Los estudios muestran que no es infarto, sino reflujo gastroesofágico severo. Le receta Omeprazol 20mg (1 cápsula cada 12 horas por 30 días) y Domperidona 10mg (1 tableta antes de cada comida por 15 días). La Sra. María paga la consulta ($450), los estudios ($890) y los medicamentos ($280) con tarjeta de crédito.

**Pregunta para validar:** ¿Cómo registrarías este caso desde la llegada hasta la salida, incluyendo la atención de urgencia, los estudios ordenados y la receta surtida?

### Historia 2: El tratamiento familiar de los Herrera
Roberto Herrera agenda citas para toda su familia para chequeos anuales: él (42 años), su esposa Ana (38 años) y sus hijos Sofía (12 años) y Diego (8 años). Todos son pacientes regulares. El Dr. Morales atiende a Roberto y encuentra presión alta, lo deriva con el cardiólogo Dr. Vázquez (interno) para el siguiente martes. Ana necesita estudios ginecológicos: papanicolau y ultrasonido pélvico. A Sofía le encuentran miopía, la refieren con oftalmología externa. Diego está sano, solo se actualiza su cartilla de vacunación con refuerzo de hepatitis B. Roberto paga todas las consultas ($450 x 4), los estudios de Ana ($650), la vacuna de Diego ($120) y agenda por separado la cita cardiológica ($650) que pagará después.

**Pregunta para validar:** ¿Cómo manejarías múltiples pacientes de una misma familia con diferentes necesidades y especialistas tanto internos como externos?

### Historia 3: La emergencia del tratamiento oncológico
El Sr. Pedro Morales llega con una receta externa del oncólogo Dr. Salinas para quimioterapia. Necesita: Cisplatino 50mg (6 viales), Ondansetrón 8mg (30 tabletas) y Dexametasona 4mg (20 tabletas). El dependiente de farmacia verifica que es receta válida y consulta inventario. Solo hay 4 viales de Cisplatino disponibles. El sistema calcula que faltan 2 viales para completar el tratamiento. Se programa entrega parcial inmediata (lo disponible: $3,450) y se ordena el faltante al proveedor con entrega en 2 días. Pedro autoriza el fraccionamiento, paga lo disponible en efectivo y deja su teléfono para avisar cuando llegue el resto.

**Pregunta para validar:** ¿Cómo procesarías una receta externa con inventario insuficiente y manejarías la entrega parcial con seguimiento?

### Historia 4: La consulta virtual seguida de presencial
Carmen Vega, paciente diabética regular, agenda teleconsulta con su endocrinólogo Dr. Mendoza por síntomas de descontrol. Durante la videollamada (30 minutos), revisan sus lecturas de glucosa de los últimos días y el Dr. Mendoza modifica su tratamiento: suspende Metformina 850mg y prescribe Metformina XR 1000mg (1 tableta en la cena) por 30 días, más Glibenclamida 5mg (1 tableta en el desayuno) por el mismo periodo. Como los síntomas no mejoran en 3 días, Carmen agenda cita presencial de urgencia. El Dr. Mendoza la examina y ordena hemoglobina glucosilada y química sanguínea de 27 elementos. Carmen paga la teleconsulta ($350), la consulta presencial ($450), análisis ($380) y medicamentos nuevos ($195) todo con transferencia bancaria.

**Pregunta para validar:** ¿Cómo vincularías la teleconsulta con la consulta presencial posterior y el ajuste de medicamentos del mismo paciente?

### Historia 5: El paciente con múltiples especialidades
Luis Jiménez, 65 años, llega derivado del Dr. García (médico general) por múltiples molestias. Su expediente muestra diabetes, hipertensión y problemas de próstata. El Dr. García lo refiere simultáneamente a: Endocrinología (Dr. Ruiz) para diabetes descontrolada, Cardiología (Dr. López) para ajuste de antihipertensivos, y Urología externa (Dr. Ramón Silva) para evaluación prostática. En Endocrinología ajustan insulina: suspenden Lantus 20 UI y prescriben Tresiba 25 UI. En Cardiología cambian Losartán por Telmisartán 80mg. El urólogo externo ordena antígeno prostático y biopsia. Luis paga cada consulta al recibirla ($450 x 3), los nuevos medicamentos ($890), los análisis ($290) y programa la biopsia ($1,450) para la siguiente semana.

**Pregunta para validar:** ¿Cómo coordinarías el tratamiento de un paciente que ve múltiples especialistas con cambios de medicamentos y estudios de diferentes áreas?

### Historia 6: La emergencia pediátrica nocturna
A las 11:30 PM llega urgente la familia Martínez con su hijo Emilio de 4 años con fiebre alta (39.5°C) y dificultad para respirar. La Dra. Torres (pediatra de guardia) lo examina y sospecha neumonía. Ordena inmediatamente: radiografía de tórax, biometría hemática completa y cultivo de garganta. La radiografía confirma neumonía del lóbulo inferior derecho. Prescribe tratamiento ambulatorio: Amoxicilina suspensión 250mg (1 cucharadita cada 8 horas por 10 días), Paracetamol gotas (según fiebre) y Salbutamol inhalador (2 puffs cada 6 horas por 5 días). Los padres pagan todo en efectivo ($650 consulta + $420 estudios + $340 medicamentos) y programan cita de control en 3 días. A las 2 AM dan de alta a Emilio con mejoría.


**Pregunta para validar:** ¿Cómo registrarías una atención de urgencia pediátrica nocturna con estudios inmediatos y tratamiento de alta con seguimiento programado?
  




