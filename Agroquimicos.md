# Agroquímicos “Gallo Giro” 

La empresa de agroquímicos "Gallo Giro” necesita controlar el movimiento de sus productos en toda la región noroeste del país. Para esto está organizada en diferentes zonas, que agrupan varios municipios. Es necesario llevar un registro de los TI, las ventas y las compras de productos, así como el control de los clientes y proveedores. 

Los productos que maneja pertenecen a varias familias, por ejemplo: fertilizantes, semillas, herbicidas, fungicidas, etc. Cada producto puede venir en diferentes tamaños o presentaciones (Faena 1lt, 1/2 lt, galón, etc.) y cada una tiene diferente UPC (https://es.wikipedia.org/wiki/C%C3%B3digo_Universal_de_Producto)

Diferentes productos comerciales pueden tener el mismo componente activo. Cada producto es provisto por un proveedor con cierto costo y se vende a otro precio al público. Los productos tienen un punto de reorden, que es la cantidad mínima de existencia antes de solicitar más producto, para cada sucursal y CEDIS.

La empresa tiene varias sucursales en el estado, que mantienen una cierta cantidad de algunos productos en sus instalaciones. Otros productos son mantenidos en los Centros de distribución (CEDIS) por su volumen o peligrosidad. Un CEDIS mantiene una gran cantidad de productos que distribuye sólo a las sucursales que de él dependen. En ocasiones es necesario trasladar mercancía de un CEDIS a otro o de una sucursal a su CEDIS, esto se conoce como Traslado de Inventario (TI). Estos no pueden realizarse de sucursal a sucursal, ni a, o desde un CEDIS ajeno. Un CEDIS nunca vende, una sucursal nunca compra. De cada TI se necesita conocer el nombre del almacenista que solicita los productos y de quien autoriza, fecha y hora de salida y de entrada. Puede haber varios CEDIS en una zona.

Cuando se realiza una compra se genera la orden de compra que especifica una de 3 formas de entregar el producto al cliente: 
- **En el momento de la compra.** Si el producto y cantidad se tiene en sucursal. La orden se marca como entregada.
- **En el CEDIS.** Si el producto o cantidad no se tiene en sucursal, pero el cliente quiere recogerlo en persona. En la Orden de compra se imprime la dirección del CEDIS a donde debe acudir el cliente. Al entregarle al cliente la orden se marca como entregada.
- **A domicilio**. El producto se entrega en el domicilio o campo donde se utilizará el producto. Se necesita registrar la dirección de entrega. Al regresar del repartidor de entregarle al cliente, la orden se marca como entregada.

Los clientes pueden ser: 
- **Doméstico:** personas que compran productos para su jardín o huerto familiar. 
- **Agricultor:** el que siembra grandes cantidades de tierra. A su vez, puede ser horticultor, fruticultor, productor de granos y semillas, etc. 

Los clientes pueden tener crédito en la empresa. Los días 10 del mes se hace corte, que se utiliza para calcular los intereses sobre las compras. El día 30 es el límite para pagar sin generar intereses. Todas las compras son a 6 meses. Si un pago se retrasa, genera un cargo del 10%.

Ejemplos:
- El CEDIS “Aeropuerto” compra, a “Fertilizantes del Bajío”, 
    - Fertilizante triple 17 “Ever Green” en diferentes presentaciones: 20 costales de 5 kilos, 100 bolsas de 1 kilo, 50 bolsas de medio kilo; 
    - 20 cajas con 100 paquetes de 50 bolsitas de 10 gramos de fertilizante de liberación lenta “Ever Grow”; 
    - Fertilizante foliar “Beauty flower”: 100 botellas de 1 litro,  50 botellas de un galón.
- Juan Méndez del CEDIS “Imala” solicita al CEDIS “Aeropuerto” un TI de:
    - 40 sacos de 50 kilos de fertilizante Urea “Tepeyac”. 
    - 20 sacos de 50Kg de semilla de trigo <br>    
    Felipe Mejía de “Aeropuerto” acepta y lo envía con Alberto Zamudio, en “Imala” recibe Alfonzo Cuadras.
- La Ing. Brenda Solares compra a la sucursal “Caballito”, via telefónica:
    - 10 toneladas de NAC27 de “Fertiberia” <br>
    Pide que se lo lleven al “Campo Victoria”; lo cargan a su cuenta. <br>
    El primer pago se retrasa por 3 meses. Por lo que se generan intereses de esos primeros meses. El resto de los pagos los realiza a tiempo.
- El señor Manuel Castro compra para su huerto familiar:
    - 3 bolsitas de 7 gramos de ácido giberélico “Raligeb”  
    - 1 botella de 1 litro de foliar “EcoJal”; <br> 
    Paga en efectivo.
 
