# 🌏 Endpoints

Aqui podemos ver los endpoints mas relevantes y asi poder interactuar con nuestra API.


### Acceder a la API
Su API de Spring Boot debería ser accesible ahora en el puerto predeterminado 8080. Abra su navegador web o una herramienta como Postman y acceda a la siguiente URL:

> http://localhost:8080/proyecto-de-ejemplo/swagger-ui.html

Claro, puedo proporcionarte ejemplos de endpoints para un CRUD (Crear, Leer, Actualizar, Borrar) en una aplicación web o API. Aquí tienes una estructura básica de endpoints RESTful para un recurso ficticio de "usuarios":

| Método | Endpoint          | Descripción                    |
|--------|-------------------|--------------------------------|
| GET    | /api/users        | Obtener todos los usuarios     |
| GET    | /api/users/{id}   | Obtener un usuario por ID      |
| POST   | /api/users        | Crear un nuevo usuario         |
| PUT    | /api/users/{id}   | Actualizar un usuario por ID   |
| DELETE | /api/users/{id}   | Borrar un usuario por ID       |

Aquí hay una breve descripción de cada endpoint:

1. **Obtener todos los usuarios**:
    - **Método**: GET
    - **Endpoint**: `/api/users`
    - **Descripción**: Retorna una lista de todos los usuarios almacenados en el sistema.

2. **Obtener un usuario por ID**:
    - **Método**: GET
    - **Endpoint**: `/api/users/{id}`
    - **Descripción**: Retorna la información de un usuario específico identificado por su ID.

3. **Crear un nuevo usuario**:
    - **Método**: POST
    - **Endpoint**: `/api/users`
    - **Descripción**: Crea un nuevo usuario con la información proporcionada en el cuerpo de la solicitud.

4. **Actualizar un usuario por ID**:
    - **Método**: PUT
    - **Endpoint**: `/api/users/{id}`
    - **Descripción**: Actualiza la información de un usuario existente identificado por su ID, utilizando los datos proporcionados en el cuerpo de la solicitud.

5. **Borrar un usuario por ID**:
    - **Método**: DELETE
    - **Endpoint**: `/api/users/{id}`
    - **Descripción**: Elimina un usuario específico identificado por su ID.

