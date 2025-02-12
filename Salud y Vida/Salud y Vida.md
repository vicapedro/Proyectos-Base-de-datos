## Salud y Vida

En **Salud y Vida** se necesita un sistema integral para administrar toda la información relativa a los servicios que ofrece, aunque inicialmente será solo una parte. Le han pedido diseñe una base de datos que satisfaga sus necesidades de control de la información.

Para Salud y Vida, los clientes son importantes, son los que solicitan servicios de la clínica para sí mismos o para sus familiares, por lo cual se necesita conocer su nombre, apellidos, dirección y teléfono. Un cliente puede tener asociados a varios dependientes.

Los pacientes pueden llegar a ventanilla y solicitar diferentes servicios o agendar una cita por teléfono o por la web app.

El paciente llega a consulta con un médico general, el cual pregunta sobre los síntomas actuales y en caso de ser necesario realiza un examen físico. Si es la primera vez que asiste a Salud y Vida, le realiza también una serie de preguntas sobre sus antecedentes médicos, familiares y sociales, así como sobre cualquier tratamiento previo, incluyendo enfermedades pasadas, cirugías, alergias y medicamentos que esté tomando. En resumen hechos de salud del pasado y del problema actual.

Si el médico puede diagnosticar con esta información puede indicar un tratamiento que puede ser una serie de indicaciones o medicamentos, en cuyo caso emite una receta. En algunos casos lo puede derivar a un médico especialista de Salud y Vida o externo, en cuyo caso es dado de alta. 

Cualquiera de los médicos puede necesitar mas información para disgnosticar, por lo que puede ordenar algún procedimiento extra: análisis clinicos, biopsias o estudios de imagenología(rayos X, tomografía, resonancia, etc).

La receta es una lista de medicamentos, dosis, frecuencia, duración e indicaciones. Al imprimirse, lleva el nombre, firma y cédula del médico.

La receta se surte en la farmacia de Salud y Vida. El dependiente verifica la receta, si es de Salud y Vida la coteja con el sistema, si no simplemente la surte *(Pendiente: medicamento controlado ¿Es necesario hacer la distinción?)* y cobra. 

Es necesario llevar un control del inventario de medicamentos. 

*Pendiente de redacción: presentación de medicamentos, dosis. Para que el sistema le indique al dependiente con la dosis, frecuencia y duración del tratamiento, cuantas cajas darle al paciente.*

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
- 




