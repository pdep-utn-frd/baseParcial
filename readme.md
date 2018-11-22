# Venta de Remeras

**Un comercio dedicado a la venta de remeras nos contrató para que hiciéramos un sistema que ayude a administrar sus pedidos.** 

### A. Remeras
El sistema trabaja con tres tipos de remeras: lisas, bordadas y sublimadas. De cada remera se desea calcular su costo.

- Remeras lisas: El costo de una remera lisa depende del talle y del color. El costo base para los talles 32 al 40 cuestan $80, mientras que los talles del 41 al 48 cuestan $100. Para esta etapa podemos considerar que estos valores no cambian (ver bonus 1). 	Ese costo base es válido para los colores básicos (blanco, negro y gris); las remeras de otros colores cuestan un 10% más.

*Ejemplo: una remera color gris de talle 40 cuesta $80, mientras que el talle 42 cuesta $100. En cambio, las mismas remeras en color verde cuestan $88 y $110 respectivamente.*

- Remeras bordadas: Cuestan lo mismo que la remera lisa más el costo del bordado. El costo del bordado depende de la cantidad de colores: $10 por cada color utilizado, con un mínimo de 20 pesos. 

*Ejemplo: una remera blanca talle 44 con un bordado de un solo color cuesta $120. Si el bordado usara hilos de 4 colores distintos costaría $140.*

- Remeras sublimadas: Cuestan lo mismo que la remera lisa más el costo del sublimado, que depende de la superficie a sublimar: 50 centavos por centímetro cuadrado de superficie. De cada sublimado se conoce el alto y el ancho, lo que permite calcular la superficie.  Algunos dibujos a sublimar pueden ser de marcas comerciales, que deben pagar derechos de autor, que son distintos según la empresa que sea dueña de esos derechos. En estos casos el costo de la remera debe incluir los derechos de autor.

*Ejemplo: Disney nos pide $100 por usar sus dibujos. Entonces, un sublimado de Frozen de 10 x 15 cm cuesta $175 (10 x 15 x 0.5 = $75 por el sublimado + $100 de derechos de autor). A este número hay que sumar el costo de la remera. Por ejemplo una remera gris talle 42 con el sublimado del ejemplo cuesta $275 ($100 de la remera + el sublimado).*

### B. Pedidos y sucursales
La empresa recibe pedidos. Cada pedido puede incluir una gran cantidad de remeras, pero todas iguales. Del pedido queremos saber su precio; el precio base se obtiene multiplicando el costo de cada remera x cantidad de remeras, pero en algunos casos puede aplicar un descuento por cantidad de remeras.

Los descuentos se aplican en función de la cantidad de remeras. Cada sucursal define la cantidad mínima de remeras a considerar para que a un pedido le aplique un descuento; para esto debemos saber en qué sucursal se hizo un pedido.

*Por ejemplo: la sucursal Flores hace descuentos en pedidos a partir de 10 remeras, mientras que la de Avellaneda y hace descuentos en pedidos a partir de 3 remeras.*

El porcentaje de descuento a aplicar depende del tipo de remera:
Las remeras bordadas se hacen a mano y por lo tanto no se hace ningún descuento por cantidad.
Algunas marcas comerciales tienen convenios de publicidad con nosotros. Cuando vendemos remeras sublimadas (en cantidad suficiente) con un dibujo de una marca con la que tenemos convenio, el descuento es del 20%.
En todos los demás casos, el descuento es del 10%.

Ejemplos: 
- Un pedido por 5 remeras lisas grises talle 42 tiene un precio de $500 en Flores ($100 de costo de la remera x 5 remeras, no le aplica descuento).
- El mismo pedido en Avellaneda se vende a $450 (idem anterior pero con un 10% de descuento).
- Suponiendo que tenemos acuerdo comercial con Disney y recibimos un pedido de 4 remeras de Frozen antes mencionadas (costo $275) en Flores se venderían a $1100 (= $275 x 4, no hay descuento).
- En Avellaneda, ese mismo pedido costaría un 20% menos ($880).
- Si no tuviéramos acuerdo comercial con Disney, el mismo pedido tendría sólo un 10% de descuento (ergo cuesta $990).

### C. Registro de pedidos
La empresa desea llevar un registro de todos los pedidos realizados, para poder llevar estadísticas. Se pide:
1. Registrar un nuevo pedido. 
2. Conocer el total facturado por la empresa.
3. Conocer el total facturado por una sucursal.
4. Conocer cuál es la sucursal que más facturó.
5. Conocer cuántos pedidos se han realizado de un color dado.
6. Obtener el pedido más caro de la empresa.
7. Conocer las sucursales que han vendido remeras de todos los talles.

