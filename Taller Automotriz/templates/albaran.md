# Albarán / Remito de recepción de mercadería

Propósito: Registrar la recepción física de piezas y materiales provenientes de un proveedor o traslado interno.

Campos principales:
- Albaran_ID
- Fecha_recepcion
- OC_ID relacionado (si aplica)
- Proveedor_ID
- Sucursal_receptora
- Lineas_recibidas: (part_number, descripcion, qty_pedida, qty_recibida, lote_serie)
- Responsable_recepcion (usuario)
- Observaciones (daños, faltantes)
- Documentos_adjunto (foto, PDF del transportista)

Notas:
- Al recepcionar realizar control de calidad visual y registrar discrepancias.
- Generar movimiento de stock hacia ubicación de almacén y actualizar balances.
