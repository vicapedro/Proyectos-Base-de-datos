# Nota de Devolución / Crédito

Propósito: Documentar la devolución de piezas o la emisión de nota de crédito al cliente o al proveedor.

Campos principales:
- Devolucion_ID
- Fecha
- Documento_origen (Factura/OT/Albarán/OC)
- Tipo_devuelve: Cliente / Proveedor
- Partidas_devuelta: (part_number, descripcion, qty, motivo_devuelta)
- Autorizacion_tecnica (usuario + fecha)
- Resultado: Aceptada / Rechazada / Reparacion
- Nota_credito_id (si aplica)
- Observaciones

Notas:
- Registrar el estado físico de la pieza devuelta y vincular con lote/serie.
- Si la devolución es por garantía, vincular claramente con condiciones de la garantía.
