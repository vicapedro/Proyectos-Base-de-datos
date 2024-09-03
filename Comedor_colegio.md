## Comedor del Colegio Pink Floyd

El “Colegio Pink Flor” con kínder y primaria busca mejorar sus servicios y lo han contratado a usted para desarrollar el sistema computacional que controle el servicio de comedor que ofrece a sus alumnos de lunes a viernes. 

Inicialmente el sistema es independiente del resto de los que posee el colegio, por lo tanto, necesita guardar información sobre los niños: su nombre, edad, nivel y grado, alergias alimenticias; del padre o tutor: su nombre, teléfono celular, teléfono y lugar de trabajo. 

El nutriólogo ha seleccionado cuidadosamente cientos de alimentos para el área de cocina. Para cada alimento se tiene una Receta que describe el procedimiento e ingredientes para preparar una cantidad de porciones. 

Cada semana el nutriólogo diseña un menú del cual los padres pueden seleccionar lo que comerán sus hijos. El menú consiste de al menos 7 opciones de comida, 7 bebidas y 7 postres, para cada una de ellas el nutriólogo calcula las calorías, carbohidratos, grasas y proteínas. Sobre los ingredientes de los alimentos, es importante identificar aquellos que son alergénicos. El nutriólogo puede reutilizar menúes. 

Con al menos 3 días de anticipación, el padre puede seleccionar los alimentos que recibirán sus hijos, que puede pagar en el momento o en abonos. Es necesario pues llevar un control de pagos. 

Los lunes y miércoles se hacen las compras de los ingredientes, es importante generar la lista de compras, considerando lo que se ha utilizado y aún queda en la cocina. De cada día de la semana se contabiliza cuantos niños recibirán cada comida específica. De cada comida se prepararán un múltiplo de las porciones que especifica la receta. La cantidad de cada ingrediente se multiplica por este factor. Sea n<sub>dc</sub> el numero de niños que consumirán que consumirán la comida c el día d. La receta para c rinde para p<sub>c</sub> porciones. Por lo tanto el factor fdc=ceil(ndc/p<sub>c</sub>). Si del ingrediente i se necesita la cantidad qci entonces para el día d se necesita Qdi=fdc(qci) de i.
 
Comida	Lunes	Martes	Miércoles	Total
Limonada (4 porciones)
1.	Limón (2pza)
2.	Agua   (1lt)
3.	Azúcar(3g)	13
f=4
Q1=4(2)=8pza
Q2=4(1)=4lt
Q3=4(3)=12g	21
f=6
Q1=6(2)=12pza
Q2=6(1)=6lt
Q3=6(3)=18g	8
F=2
Q1=2(2)=4pza
Q2=2(1)=2lt
Q3=2(3)=6g	

24pza 
12lt
36g

El niño come sólo lo que el padre apruebe del menú. Los niños pueden ser alérgicos a ciertos ingredientes, por lo cual es importante conocer sus alergias alimentarias. 

Algunos niños tienen dieta especial que debe ser proporcionada al colegio por el papá con una semana de anticipación. Por este servicio se realiza un cobro extra. El niño no puede recibir otra cosa que lo que marca su dieta. 

Ejemplos:
## Ejemplo 1 
Actualmente es la semana 20 y los padres pueden seleccionar de este menú:

| Comida	| Bebida	| Postre |
|-----------|-----------|--------|
|Mole poblano	|Agua de melón	|Gelatina sabores varios|
|Ceviche de soya	|Agua de sandía	|Pastel de 3 leches|
|Verduras al vapor con puré de papa	|Agua de jamaica	|Flan|
|Tacos de carne asada	|Limonada	|Fruta picada|
|Tamales de verdura	|Agua de piña	|Frutos rojos|
|Enchiladas verdes	|Agua de pepino	|Mangoneadas|
|Pollo a la plancha	|Agua de horchata	|Pastel de chocolate|

## Ejemplo 2
El señor Ramírez tiene 2 hijos, no se quiere complicar y ordena lo mismo para sus hijos; paga el total:

Órdenes de Juan para la semana 21
|Día	|Comida	|Bebida	|Postre |
|-------|-------|-------|-------|
|Lunes	|Tacos de carne asada|	Agua de horchata	|Frutos rojos|
|Martes	|Mole poblano	|Agua de pepino	|Mangoneadas|
|Miércoles	|Enchiladas verdes|	Agua de jamaica	|Pastel de chocolate|
|Jueves	|Tamales de verdura	|Agua de piña	|Frutos rojos|
|Viernes	|Ceviche de soya|	Agua de melón|	Flan|

## Ejemplo 3 

El nutriólogo registra una nueva comida: 

### Crêpes salados

**Ingredientes** (Para 5 porciones)
Harina de garbanzo: 110 g

- Agua: 250 ml
- Aceite de oliva virgen extra: 15 ml
- Sal: 2 g
- Cebollino: 10 gramos
- Pimienta negra molida: 1 gramo
- Aguacate: 1
- Cebolla morada: 1
- Pimiento rojo picante o dulce: 1

**Preparación:**

Disponer la harina de garbanzos en un cuenco o jarra con el agua…

… Continuar hasta terminar con toda la masa, rellenar con los ingredientes preparados y servir.


## Ejemplo 4
Ana Flérida está en la fila, es su turno, pone su credencial de la escuela en el sensor, en su pantalla y la de la barra aparece su orden para ese día. Marko le sirve, le entrega y oprime el botón de entregado.   
