El proyecto planteado se sitúa en un escenario de una veterinaria Las funcionalidades a implementar mínimamente son:

- Las entidades (y los campos mínimos) a contemplar son: Propietarios (nombre, apellido, nro de documento, fecha de nacimiento, domicilio, teléfono y correo electrónico) y Mascotas (nombre, especie, raza, sexo, fecha de nacimiento, pelaje). La cardinalidad se establece en 1:N, un Propietario puede tener N Mascotas, pero una Mascota solo pertenece a un Propietario.

- Implementar una API para cumplir con el CRUD (creación, lectura del listado de items, lectura de un item en particular, modificación de valores, eliminación) de ambas entidades generadas mediante los modelos correspondientes y realizar tales operaciones de en una base de datos (queda a elección el motor a utilizar, debe ser uno relacional).

- La implementación del backend deberá estar correctamente separada en capas: interfaz de usuario (los endpoints), lógica de negocio, persistencia. Además de contemplar excepciones tanto genéricas como personalizadas (al menos una -1-) para el control de errores.

Por cada endpoint de la API se deberá considerar:

- Uso adecuado del tipo de request HTTP.

- Armado de la respuesta en JSON utilizando correctamente los códigos de cada item para las mismas.

- Devolver respuestas consistentes en caso de error (contemplando error en la request y los que aplican para el lado del servidor).
-----
- Se deberá considerar un conjunto de datos del negocio (nombre de fantasía, dirección, datos de contacto) que serán persistidos en un archivo .JSON que deberá administrarse desde la misma aplicación.

- Para el frontend se deberá contar con una UI que debe generarse con Blazor WebAssembly para poder ejecutar el CRUD haciendo las llamadas a la API del backend. Deberá considerar una comunicación adecuada con el usuario final y la visualización de mensajes ante los eventos que sean registrados.