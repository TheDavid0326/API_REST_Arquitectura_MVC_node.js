# Proyecto de Películas - Arquitectura MVC

Este proyecto implementa una API RESTful para gestionar una colección de películas utilizando la arquitectura MVC (Modelo-Vista-Controlador). La aplicación está construida con Node.js y Express.

## Estructura del Proyecto

La estructura del proyecto está organizada de la siguiente:

.
├── controllers
│   └── movies.js
├── middlewares
│   └── cors.js
├── models
│   └── local-file-system
│       └── movie.js
├── routes
│   └── movies.js
├── schemas
│   └── movies.js
├── utils.js
└── app.js

### `app.js`

Este archivo es el punto de entrada de la aplicación y configura el servidor Express, los middlewares y las rutas.

## Rutas (routes/movies.js)
Este archivo define las rutas de la API y asocia cada ruta con el método correspondiente del controlador.

## Modelos (models/local-file-system/movie.js)
Este archivo define el modelo de datos para las películas y contiene métodos para interactuar con el almacenamiento de datos.

## Controladores (controllers/movies.js)
Este archivo define los métodos del controlador que manejan las solicitudes y respuestas de la API.

## Endpoints de la API
- **GET /movies**: Obtiene todas las películas. Se puede filtrar por género.
- **POST /movies**: Crea una nueva película.
- **GET /movies/:id**: Obtiene una película por ID.
- **PATCH /movies/:id**: Actualiza una película por ID.
- **DELETE /movies/:id**: Elimina una película por ID.

## Validación
Utilizamos Zod para la validación de los datos de entrada. Los esquemas de validación se encuentran en `schemas/movies.js`.

## Middleware
El middleware de CORS está configurado en `middlewares/cors.js`.

## Conclusión
Desarrollar este proyecto utilizando la arquitectura MVC ha sido una experiencia enriquecedora que ha permitido mantener un código limpio, organizado y fácil de mantener. La separación clara entre modelos, vistas y controladores no solo facilita la escalabilidad del proyecto, sino que también mejora la colaboración y la comprensión del código entre los desarrolladores. Espero que este proyecto sirva como una base sólida para futuras implementaciones y que proporcione una guía útil para quienes deseen construir aplicaciones similares. ¡Gracias por tu interés y colaboración!
