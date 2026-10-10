SISTEMA DE FACTURACIÓN DE REPUESTOS VINI

1. Descripción del sistema
Proyecto académico orientado a organizar la facturación y el control de las operaciones de un negocio de repuestos, incluyendo clientes, productos, ventas, pagos e inventarios.

2. Objetivo
   Diseñar un sistema que facilite la elaboración de facturas, el registro de pagos y la administración de los productos y clientes.

3. Problema que resuelve
   Buscar reducir los errores de los registros manuales, mejorar la consulta de información y facilitar el control de las ventas y las existencias.

 4. Funcionalidades Principales
    Gestión de clientes y productos.
    Consulta de precios y disponibilidad.
    Elaboración y cálculo de facturas.
    Registro de pagos.
    Actualización del inventario.
    Consulta de historial de facturación.

5. Arquitectura del sistema
   Se propone una arquitectura por capaz que separa las responsabilidades y facilita el mantenimiento.

   Frontend: Interfaz para el administrador y cajero.
   Backend: Lógica de negocio, validaciones y gestión de las operaciones.
   Base de datos: Almacenamiento de usuarios, clientes, productos, facturas y pagos.

   6. Herramienta Utilizada
      GitHub: repositorio y control de versiones.
      GitHub Projects: Planificación y seguimiento de tareas.
      GitHub Issues: Registro de incidencias y mejoras.
      Visual Paradigm Online: Modelado UML y Arquitectura.
      Microsoft Word: Documentación académica.

   7. Organización y Seguimiento
      El proyecto se organiza mediante columnas Blacklog, Por Hacer, En progreso, En revisión y Finalizado. Las tareas e incidencias se actualizan según su avance real.

    8. Estado Actual
         Se han trabajado los requisitos, los modelos UML, el diseño arquitectónico y la planificación del proyecto. La documentación y las evidencias técnicas se están organizando en GitHub para facilitar su revisión y continuar con las siguiente etapas.

   9. Mantenimiento de la documentación
          Los cambios, las incidencias y las tareas pendientes se registrarán en las herramientas correspondientes. El README se actuializará cuando existan avances relevantes en el diseño o desarrollo del sistema.

         Asignatura: Ingenieria en software.
         Proyecto: Sistema de Facturación de Repuestos Vini

   10. Arquitectura tecnológica del sistema
          El sistema de facturación de Repuestos Vini se plantea con una arquitectura por capas, separando la interfaz de usuario, la lógica de negocio y el almacenamiento de los datos. Esta organización facilita el mantenimiento, las pruebas y las futuras mejorar del sistema.

   10.1 Frontend
              El frotend será la interfaz gráfica utilizada por el administrador y el empleado/cajero para gestionar clientes, consultar productos, elborar facturas y registrar pagos.
       Tecnologías propuestas: HTML5, CSS3 Y JavaScript.
       Responsabilidad: mostrar formularios, presentar información, validar datos básicos de entrada y enviar solicitudes al backend.
       
   10.2 Backend
   El bankend será responsable de procesar las operaciones del negocio y aplicar las reglas necesarias para garantizar la consistencias de la información.
   Tecnología propuesta: C# con.NET 9 y ASP.NET core Web API.
   Responsabilidad: gestionar clientes, productos, facturas, pagos, cálculos de subtotales e ITEBIS, y actualización del inventario.
   Comunicación: exponer una API REST para recibir solicitudes del fronted y devolver respuestas con los resultados de las operaciones.

   10.3 Base de Datos
   La base de datos almacenará la información del sistema.

   Las entidades principales previstas son:
   -Clientes
   -Productos
   -Facturas
   -Detalle de facturas
   -Pagos
   -Usuarios
    Tecnología de base de datos: Pendiente de confirmar antes de iniciar la implementación.

   10.4 Comunicación entre los componentes
   1. El usuario realiza una operación desde el frontend.
   2. El frontend envía una solicitud HTTP a un endpoint de la API REST.
   3. El bakend validad la solicitud y ejecuta la lógica del negocio.
   4. El bakend devuelve una respuesta, normalmente en un formato JSON.
   5. El bakend consulta o actualiza la base de dato cuando le corresponde.
   6. El frontend presenta el resultado al usuario.

   10.5 Estado Actual de la Aquitectura
   La arquitectura se encuentra en fase de documentación y diseño. El repositorio contiene documentación Inicial y diagramas UML. La implementación del backend, la conexión con la base de datos y la integración con el frontend quedan pendientes de desarrollo y verificación.
   
   
