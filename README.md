# Practica_Merge

🔗 Fusión de Datos - Olist E-commerce

📌 ¿Qué se hizo en este código?
Este notebook trabaja con datos de la plataforma de e-commerce brasileña Olist y realiza una integración de tablas (similar a un "JOIN" en bases de datos) para combinar información que originalmente estaba separada en diferentes archivos.

El proceso fue:
Cargar 4 archivos CSV con información de:

Pedidos (orders)

Clientes (customers)

Productos vendidos en cada pedido (items)

Catálogo de productos (products)

Fusionar tablas relacionadas:

Unir orders con customers usando el ID del cliente

Unir items con products usando el ID del producto

Analizar los resultados para entender qué información nueva se obtuvo y cómo podía usarse.

🎯 ¿Para qué sirvió?
Unir pedidos con clientes (orders_customers)
Antes: Teníamos pedidos con IDs de clientes, pero no sabíamos quiénes eran realmente esos clientes (dónde viven, etc.).

Después: Cada pedido ahora incluye información del cliente como:

Ciudad y estado donde vive

Código postal

Utilidad: Ahora podemos saber, por ejemplo:

¿De qué ciudades vienen más pedidos?

¿Hay regiones donde los pedidos tardan más en llegar?

¿Qué tipos de clientes compran con más frecuencia?

Unir productos vendidos con catálogo (items_products)
Antes: Teníamos registros de qué productos se vendieron, pero solo con IDs numéricos.

Después: Cada producto vendido ahora incluye sus características completas:

Categoría (ej. "electrónicos", "muebles", "papelería")

Peso y dimensiones

Cantidad de fotos y longitud de la descripción

Utilidad: Esto permite:

Analizar qué categorías de productos se venden más

Ver si el precio es justo según el tamaño/peso del producto

Calcular mejor los costos de envío
