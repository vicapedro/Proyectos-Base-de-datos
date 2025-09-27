# Registro de Garantía y Reclamos

Propósito: Llevar control de garantías de piezas y mano de obra y gestionar reclamos.

Campos principales:
- Garantia_ID
- Fecha_reclamo
- OT_ID_original
- Documento_factura
- Vehículo_VIN
- Cliente_ID
- Partes_en_garantia: (part_number, descripcion, lote_serie, fecha_instalacion)
- Motivo_reclamo (descripción)
- Evaluacion_tecnica (resultado de la inspección)
- Decision: Reemplazar / Reparar / Emitir_nota_credito / Rechazar
- Acciones_realizadas (detalle)
- Responsable_resolucion (usuario)
- Fecha_resolucion
- Evidencia (fotos, informes)

Notas:
- Registrar si la garantía recae sobre proveedor o taller.
- Llevar tiempos de respuesta y SLA por tipo de reclamo.
