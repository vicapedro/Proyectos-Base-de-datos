# Orden de Trabajo (OT)

Propósito: Documentar el trabajo a realizar en un vehículo, autorizar al taller a intervenir y servir de vínculo entre recepción, taller, almacén y facturación.

Campos principales (mínimos):
- OT_ID: identificador único (formato prefijo por sucursal, p. ej. SLP-000123)
- Fecha_creacion: fecha y hora de creación
- Sucursal: código o nombre de la sucursal
- Recepcionista_ID: usuario que registró la recepción
- Cliente_ID / Cliente_nombre: referencia al cliente (si aplica)
- Tipo_cliente: Particular / Flota / Empresa
- Vehículo_VIN: VIN
- Matrícula: número de placa
- Marca, Modelo, Año
- Kilometraje_ingreso
- Motivo_ingreso: descripción libre proporcionada por el cliente
- Estado_OT: Abierta / En curso / Esperando repuesto / Parcialmente entregada / Terminada / Entregada
- Técnico_asignado (puede ser varios): lista de técnicos con ID
- Tareas: lista de tareas propuestas (cada tarea: código, descripción, tiempo_estimado_horas)
- Repuestos_requeridos: lista (part_number, descripcion, qty_solicitada, qty_reservada)
- Prioridad: Normal / Urgente / Programado
- Presupuesto_estimado: monto estimado
- Aprobacion_cliente: boolean + firma_fecha
- Observaciones_tecnicas (texto largo)
- Adjuntos: enlaces a fotos, PDFs, escaneos

Notas de uso:
- Reservar stock al crear OT; si no hay stock crear OC y ligar ambas referencias.
- Registrar tiempos reales por tarea para cálculo de productividad y coste.
- Mantener historial de cambios de estado con timestamps y usuario responsable.
