DISEÑO DE LA BASE DE DATOS

SISTEMA DE FACTURACIÓN DE REPUESTOS VINI

1. Objetivo
   Definir la estructura lógica de la base de datos del sistema de facturación, incluyendo las entidades principales, sus atributos y las relaciones necesarias
   para gestionar clientes, productos, facturas, pagos y usuarios.
2. Tecnología Prevista
   La tecnología de base de datos está pendiente de confirmación durante la implementación. El diseño se plantea para una base de datos relacional.
3. Entidades Principales
   Clientes
   -id_cliente(clave primaria)
   -nombre
   -descripción
   -precio
   -existencia
   -estado

   Usuarios
   -id_usuario(clave primaria)
   -nombre
   -correo
   -contrasena_hash
   -rol
   -estado

   Facturas
   -id_factura(clave primaria)
   -id_cliente(clave foránea)
   -id_usuario(clave foránea)
   -fecha
   -subtotal
   -impuesto
   -total
   -estado

   Detalle_Factura
   -id_detalle(clave primaria)
   -id_factura(clave foránea)
   -id_producto(clave foránea)
   -cantidad
   -precio_unitario
   -importe

   Pagos
   -id_pago(clave primaria)
   -id_factura(clave foránea)
   -fecha
   -monto
   -metodo_pago
   -referencia

   4. Relaciones entre entidades
      -Un cliente puede tener muchas facturas.
      -Un usuario puede registrar muchas facturas.
      -Una factura puede contener varios detalles.
      -Cada detalle corresponde a un producto.
      -Una factura puede tener uno o varios pagos.
      -Un producto puede aparecer en muchos detalles de factura.

   5. Reglas de integridad
      -Cada entidad tendrá una clave primaria única.
      -Las claves foráneas mantendrán la relación entre las tablas.
      -La cantidad de productos y los montos de las operaciones deberá ser validada.
      -Los precios utilizados en las facturas se conservarán en el detalle para mantener el historial de ventas.
      -Las contraseñas no deberán almacenarse en texto plano.

   6. Estado Actual
      Este documento representa el diseño lógico propuesto. La creación física de las tablas, la configuración de las relaciones y las pruebas
      de integridad quedan pendientes de implementación y verificación en el backend.

   7. Próximas actividades
      -Confirmar el montor de base de datos.
      -Crear las tablas y definir sus tipos de datos.
      -Implementar las relaciones y restricciones.
      -Configurar la conexión desde el bakend.NET.
      -Realizar pruebas de inserción, consulta, actualización y eliminación. 
   
