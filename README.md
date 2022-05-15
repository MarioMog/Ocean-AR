# Ocean-AR

## Links de despliegue
| Software | Función | Link | Repositorio |
| ------------- | ------------- | ------------- | ------------- |
| OceanAR-Frontend | Está es la aplicación con la que interactuaran los usuarios | NA | ![Backend](https://github.com/armap99/Ocean-AR-Backend) |
| Ocean-AR-Backend | Es la API en la cual se realizarán las peticiones desde la aplicación del usuario | NA | ![Frontend](https://github.com/moiseshernandez26/OceanAR-Frontend) |

## Documentación
```mermaid
sequenceDiagram
    participant USER
    participant FRONT
    participant API
    participant BD
    USER->>FRONT: Interactua con la aplicación
    FRONT->>API: Realiza la petición a la base de datos
    API->>BD: Hace la consulta  deseada
    BD->>API: Retorna el registro
    API->>API: Realiza la logica correspondiente en el controlador
    API->>FRONT: Entrega una respuesta para la pretición realizada
    FRONT->>USER: Muestra la información recibida
```
