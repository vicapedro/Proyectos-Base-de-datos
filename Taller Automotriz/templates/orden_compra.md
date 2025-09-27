# Orden de Compra (OC)

Propósito: Solicitar repuestos o materiales al proveedor o a otro centro de la red.

Campos principales:
- OC_ID: identificador único
- Fecha_solicitud
- Sucursal_solicitante
- Solicitante_ID (usuario)
- Proveedor_ID / Proveedor_nombre
- Lineas_pedido: cada línea contiene (part_number, descripcion, cantidad_solicitada, unidad, costo_unitario, moneda, prioridad)
- Fecha_requerida (ETA)
- Estado_OC: Pendiente / Parcial / Recepcionado / Cancelado
- Referencia_OTs: lista de OT_IDs relacionadas
- Observaciones

Notas:
- Permitir recepciones parciales; cada recepción debe generar un albarán.
- Registrar número de lote/serie cuando aplique para trazabilidad.
