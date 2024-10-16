#Consultas SQL
Este repositorio contiene un conjunto de consultas SQL y procedimientos para la gestión de productos, órdenes y otros datos, diseñadas para ejecutarse en SQL Server Management Studio (SSMS).
#Estructura del archivo
El archivo principal incluye las siguientes operaciones:

1. Inserciones de productos:
Inserciones en la tabla cs_productos con diferentes productos y sus precios (costo, venta y mercado).

2. Modificación de la estructura de tablas:
Se agrega una nueva columna ganancia_real_acumulada a la tabla cs_productos para almacenar la ganancia acumulada.

3. Creación de la tabla cs_ordenes:
Se define una tabla para las órdenes de compra, con llaves foráneas que enlazan a proveedores.

4.Inserciones en la tabla de órdenes:
Varias órdenes de compra se añaden con fechas de emisión, entrega, y referencia a proveedores.

5.Procedimiento almacenado actualizar_productos:
Un procedimiento que verifica si un producto apa8ece en alguna orden antes del 01/01/2011. Si no aparece, se inserta en una nueva tabla y se reduce su precio de venta en un 10%.

#Notas
-Estructura de las tablas: Asegúrate de tener creadas previamente las tablas cs_productos, cs_ordenes, y cs_proveedores antes de ejecutar las inserciones y el procedimiento.
-Datos ficticios: Los datos de productos, proveedores y órdenes son ficticios y se utilizan para demostrar el funcionamiento de las consultas y el procedimiento almacenado.
