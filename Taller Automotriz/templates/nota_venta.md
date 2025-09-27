# Nota de Venta / Factura

Propósito: Documento fiscal que detalla la venta de mano de obra y piezas al cliente.

Campos principales:
- Documento_ID (factura/nota)
- Fecha_emision
- Sucursal
- Cliente_ID / Cliente_nombre (o Público en general)
- Referencia_OT_ID
- Lineas: (tipo: Mano_obra / Pieza / Servicio, codigo, descripcion, cantidad, precio_unitario, subtotal_linea)
- Subtotal, Descuentos, Impuestos, Total
- Forma_de_pago (efectivo, tarjeta, transferencia, crédito)
- Pagos_parciales: lista de pagos (fecha, monto, método)
- Emisor (usuario que emitió)
- Observaciones

Notas:
- Debe referenciar la OT para control de garantías y para conciliación financiera.
- Incluir datos de garantía de piezas y mano de obra cuando aplique.
