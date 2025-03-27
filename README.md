# Mantencion_cliente
Este código permite gestionar clientes de un taller, registrando su información, los servicios solicitados y calculando el tiempo total de reparación. También permite añadir servicios adicionales como lavado de auto o gamuza. Finalmente, muestra el estado y el tiempo estimado de cada cliente.
# Sistema de Gestión de Clientes para Taller Mecánico

Este proyecto es un sistema simple para gestionar clientes en un taller mecánico. Permite registrar información sobre los clientes, los servicios solicitados y calcular el tiempo total de reparación.

## Funcionalidades

- **Agregar Clientes**: Permite ingresar la información de los clientes, incluyendo su RUT, nombre, marca y modelo del automóvil.
- **Agregar Servicios**: Los usuarios pueden agregar múltiples servicios solicitados para cada cliente.
- **Calcular Tiempo de Reparación**: El sistema calcula el tiempo total de reparación basado en los servicios solicitados y si se desea realizar un lavado de auto o de gamuza.
- **Mostrar Estado**: Al finalizar la entrada de datos, se muestra el estado del cliente y el tiempo estimado de reparación.

## Estructura del Código

### Clase `Cliente`

La clase `Cliente` tiene los siguientes atributos y métodos:

- **Atributos**:
  - `rut`: RUT del cliente.
  - `nombre`: Nombre completo del cliente.
  - `marca`: Marca del automóvil.
  - `modelo`: Modelo del automóvil.
  - `servicios`: Lista de servicios solicitados.
  - `estado`: Estado actual del cliente (por defecto "trabajando").

- **Métodos**:
  - `agregar_servicio(servicio)`: Agrega un servicio a la lista de servicios del cliente.
  - `actualizar_estado(estado)`: Actualiza el estado del cliente.
  - `tiempo_total_reparacion(lavar_auto=False, lavado_gamuza=False)`: Calcula el tiempo total de reparación basado en los servicios solicitados.
  - `mostrar_estado(lavar_auto=False, lavado_gamuza=False)`: Muestra el estado del cliente y el tiempo total de reparación.

### Función `agregar_clientes()`

Esta función permite al usuario ingresar múltiples clientes y sus servicios. Al finalizar, muestra el estado de cada cliente.

## Uso

1. Clona este repositorio o descarga el archivo.
2. Asegúrate de tener Python instalado en tu máquina.
3. Ejecuta el script en tu terminal o entorno de desarrollo.
4. Sigue las instrucciones en pantalla para agregar clientes y servicios.

## Ejemplo de Uso
Ingrese el RUT del cliente: 12345678-9 
Ingrese el nombre completo del cliente: Juan Pérez 
Ingrese la marca del automóvil: Toyota 
Ingrese el modelo del automóvil: Corolla 
Ingrese un servicio solicitado (o 'salir' para terminar): Revision 1000 km 
Ingrese un servicio solicitado (o 'salir' para terminar): Cambio Aceite 
Ingrese un servicio solicitado (o 'salir' para terminar): salir 
¿Desea lavar el auto? (si/no): si
¿Desea lavado de gamuza? (si/no): no 
¿Desea agregar otro cliente? (si/no): no


## Notas

- Los tiempos de reparación para cada servicio están predefinidos en el código.
- El sistema permite agregar múltiples clientes y servicios en una sola ejecución.

## Contribuciones

Las contribuciones son bienvenidas. Si deseas mejorar el código o agregar nuevas funcionalidades, siéntete libre de hacer un fork del repositorio y enviar un pull request.

## Licencia

Este proyecto está bajo la Licencia MIT. Para más detalles, consulta el archivo LICENSE.
