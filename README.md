# Administracion-de-Bases-de-datos-2026
#
Repositorio para el proyecto de la EE Administración de Bases de datos
#
Archivos del proyecto final de la EE Administración de Bases de Datos 2026
#
URL de documento: https://docs.google.com/document/d/12wIfVVEoqosCSUsGEaB1CFcIJCy8tV0Xeo7WeiNm9G4/edit?pli=1&tab=t.0
#
# Descripcion del proyecto
La agencia "Automóviles Imperiales" " requiere la implementación de un sistema de administración informático para gestionar las operaciones de ventas, inventario de autos, clientes, proveedores y reportes. Actualmente, la gestión se realiza manualmente, lo cual resulta ineficiente y propenso a errores. Se necesita un sistema que optimice las operaciones y mejore la eficiencia de la agencia.

El desarrollo de la solución debe realizarse con tecnologías actuales y un diseño de base de datos optimizado. La interfaz de usuario debe ser intuitiva y fácil de usar, compatible tanto con dispositivos de entrada tradicionales (teclado y ratón).

Se pretende que el nuevo sistema se desarrolle bajo una arquitectura cliente – servidor y que sea de instalación local (software de escritorio) conectado a una base de datos relacional. 

El sistema estará compuesto por los siguientes módulos principales:

## Módulo Usuarios
+ Registro de usuarios: El sistema debe permitir registrar usuarios que sean empleados de la agencia (administradores, vendedores, personal administrativo, etc.). Los datos de un usuario son: nombre, apellidos, teléfono, correo electrónico, dirección (calle y número), código postal, ciudad, puesto, tipo de usuario (administrador, vendedor). Adicionalmente, se debe guardar un nombre de usuario y contraseña para acceder al sistema.

+ Edición de usuario: El sistema debe permitir la edición de la información de los empleados.

+ Eliminar usuario: El sistema debe permitir eliminar la información de los empleados. Si la cuenta a eliminar es la del usuario que tiene la sesión activa, ésta no podrá ser eliminada.
Nota: La eliminación es lógica (un campo de estado en la base de datos).

+ Buscar usuario: El sistema debe permitir buscar usuarios por nombre o puesto. En caso de nombre, se debe poder encontrar la información sin importar si son mayúsculas o minúsculas.

+ Inicio de sesión: El sistema debe contar con una autenticación de usuario y contraseña para poder acceder.

## Módulo Inventario
+ Registro de Autos Nuevos: El sistema debe permitir registrar los autos nuevos disponibles para la venta. Los datos a considerar son: marca, modelo, año, color, número VIN (Vehicle Identification Number), precio, cantidad disponible, características especiales (como tipo de motor o tecnología).

+ Edición de Auto: El sistema debe permitir la edición de la información del auto registrado.

+ Eliminar Auto: El sistema debe permitir eliminar la información del auto. Si el auto ya ha sido vendido o está reservado, no podrá ser eliminado.
Nota: La eliminación es lógica (un campo de estado en la base de datos).

+ Buscar Auto: El sistema debe permitir buscar autos por marca, modelo o características. En caso de búsqueda por marca o modelo, se debe poder encontrar la información sin importar si son mayúsculas o minúsculas.

## Módulo Clientes
+ Registro de Clientes: Registrar información sobre los clientes interesados en comprar autos. Los datos a considerar son: nombre, apellidos, teléfono, correo electrónico, dirección (calle y número), código postal y ciudad.

+ Edición de Cliente: Permitir editar la información del cliente registrada.

+ Eliminar Cliente: Permitir eliminar información del cliente. Si el cliente tiene compras pendientes o reservas activas, no podrá ser eliminado.
Nota: La eliminación es lógica (un campo de estado en la base de datos).

+ Buscar Cliente: Permitir buscar clientes por nombre o número telefónico.

## Módulo Ventas
+ Registrar Venta: Registrar las ventas realizadas a los clientes. La información a considerar es: fecha de venta, cliente asociado, auto vendido (incluyendo detalles como VIN), precio final, forma de pago (efectivo, financiamiento), y notas adicionales.

+ Editar Venta: Permitir editar detalles sobre una venta registrada.

+ Cancelar Venta: Permitir cancelar una venta generando un registro correspondiente.

+ Buscar Ventas: Permitir buscar ventas por cliente o fecha.

## Módulo Proveedores
+ Gestión de Proveedores: Registrar información sobre los proveedores que suministran autos a la agencia. Los datos a considerar son: nombre del proveedor, dirección, teléfono, correo electrónico y contacto principal.

+ Registrar Compras a Proveedores: Registrar las compras realizadas a proveedores para adquirir nuevos autos. Incluir detalles como fecha, cantidad comprada y precios unitarios.

+ Gestionar Pagos a Proveedores: Registrar los pagos realizados a los proveedores incluyendo fecha y monto.

## Módulo Reportes
+ Reporte de Ventas: Generar reportes sobre las ventas realizadas en un período determinado (diario, semanal o mensual), mostrando detalles como cantidad vendida por modelo y total recaudado.

+ Reporte de Inventario: Generar reportes sobre el inventario actual disponible en la agencia incluyendo cantidad por modelo y marca.

+ Reporte Financiero: Generar reportes sobre ingresos totales por ventas menos gastos operativos durante un período determinado.

+ Reporte de Clientes: Generar reportes sobre clientes registrados e interesados en adquirir vehículos.

Este esquema proporciona una base sólida para desarrollar un sistema administrativo adaptado a las necesidades específicas de una agencia dedicada a la venta de autos nuevos.
