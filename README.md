# Restful Booker API Testing

Proyecto práctico de API Testing desarrollado con Postman sobre la API pública Restful Booker.

El objetivo del proyecto es validar un flujo CRUD completo mediante requests HTTP, autenticación, variables de entorno y tests automatizados.

## Tecnologías utilizadas

- Postman
- REST API
- JSON
- HTTP
- JavaScript básico para assertions
- Collection Runner

## Escenarios implementados

### Authentication
- POST - Create Token
- Validación de status code
- Validación de generación del token
- Almacenamiento dinámico del token en una variable de entorno

### Booking
- POST - Create Booking
- GET - Get Booking
- PUT - Update Booking
- PATCH - Partial Update Booking
- DELETE - Delete Booking
- GET - Verify Booking Deleted

## Validaciones realizadas

Se validaron, entre otros aspectos:

- Status codes
- Datos recibidos en las respuestas
- Creación dinámica de Booking ID
- Persistencia de datos
- Actualización completa de recursos
- Actualización parcial
- Autenticación mediante token
- Eliminación de recursos
- Validación de respuesta 404 luego de eliminar una reserva

## Variables de entorno

El proyecto utiliza:

- `base_url`
- `token`
- `booking_id`

Los valores de `token` y `booking_id` se generan dinámicamente durante la ejecución de la colección.

## Ejecución automatizada

La colección puede ejecutarse completamente mediante Postman Collection Runner.

Resultado obtenido:

- 7 requests ejecutados
- 25 tests
- 25 passed
- 0 failed
- 0 errors

## Evidencia

![Collection Runner](evidence/collection-runner-25-tests-passed.png)

## Cómo ejecutar el proyecto

1. Importar la Collection ubicada en `/postman`.
2. Importar el Environment `Restful Booker - QA`.
3. Seleccionar el environment.
4. Ejecutar la colección mediante Collection Runner.
5. Mantener el orden definido de los requests.

## Flujo

POST Create Token  
↓  
POST Create Booking  
↓  
GET Get Booking  
↓  
PUT Update Booking  
↓  
PATCH Partial Update Booking  
↓  
DELETE Delete Booking  
↓  
GET Verify Booking Deleted

## Objetivo profesional

Este proyecto fue realizado como parte de mi formación en API Testing con Postman, con el objetivo de fortalecer conocimientos técnicos aplicables a roles de Analista Funcional y QA.
