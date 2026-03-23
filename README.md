# Alhaja_Garcia_Carmen_RetoRefactorizacion

Reto de Refactorización: Sistema de Gestión de Parque de Atracciones.

Este proyecto consiste en el diseño de un diagrama de clases para un sistema de gestión integral de un parque de atracciones, basado en unos requisitos específicos de negocio.

El objetivo era modelar la estructura del parque, el cual se divide en zonas temáticas. Cada zona debe tener obligatoriamente un hotel y al menos una atracción, un restaurante, una tienda y un espectáculo.
Además, el sistema debe gestionar las ventas, permitiendo a los clientes comprar entradas para fechas específicas y, de forma opcional, realizar reservas de hotel asociadas a dicha compra.

Ahorro de líneas de código mediante el uso de grupos:
Al utilizar grupos de elementos en el XSD, hemos conseguido una reducción significativa en la extensión del código.
Líneas ahorradas: Aproximadamente unas 15 líneas de código. En lugar de repetir los mismos atributos y elementos (como nombre, ram o cpu) en cada tipo de servidor, los hemos agrupado en una sola definición. Esto hace que el archivo sea mucho más corto, fácil de leer y, sobre todo, más sencillo de mantener si en el futuro queremos añadir una característica nueva a todos los servidores a la vez.

Validación de identificadores únicos (ID):
Siguiendo las instrucciones de la actividad, se ha definido un indicador unique para el atributo id de los servidores. Esto garantiza que cada máquina sea única en todo el sistema. Error en VS Code: Si intentamos introducir dos servidores con el mismo ID, Visual Studio Code marca el archivo con un subrayado rojo. El mensaje de error que aparece indica algo como: Duplicate identity constraint value. 
Resultado: Esto impide que el XML sea válido, forzándonos a corregir el identificador para que no se repita en el catálogo.