# Ocean-AR

## Problemática
Especies en peligro de extinción.

## Solución
Mostrar las especies en peligro de extinción  con el fin de concientizar a la población de una forma interactiva y divertida.

## Links de despliegue
| Software | Función | Link | Repositorio |
| ------------- | ------------- | ------------- | ------------- |
| OceanAR-Frontend | Está es la aplicación con la que interactuaran los usuarios | NA | [Backend](https://github.com/armap99/Ocean-AR-Backend) |
| Ocean-AR-Backend | Es la API en la cual se realizarán las peticiones desde la aplicación del usuario | [Link](https://moiseshernandez26.github.io/OceanAR-Frontend/) | [Frontend](https://github.com/moiseshernandez26/OceanAR-Frontend) |

## Documentación
```mermaid
sequenceDiagram
    participant USER as Usuario
    participant FRONT as Aplicación web
    participant API
    participant BD
    USER->>FRONT: Interactua con la aplicación
    FRONT->>API: Realiza la petición a la base de datos
    API->>BD: Hace la consulta  deseada
    BD->>API: Retorna el registro
    API->>API: Realiza la lógica correspondiente en el controlador
    API->>FRONT: Entrega una respuesta para la pretición realizada
    FRONT->>USER: Muestra la información recibida
```

