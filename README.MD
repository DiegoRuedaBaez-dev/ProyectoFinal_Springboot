# Proyecto Final Springboot - Gestor de Ecommerce

Este proyecto es una aplicación completa de Ecommerce que integra un frontend desarrollado con tecnologías web estándar y un backend robusto construido con Spring Boot. El sistema permite la gestión de productos, usuarios, pedidos y otras funcionalidades necesarias para un Ecommerce.

## Estructura del Proyecto

```plaintext
/proyectofinal_springboot/
├── frontend/
│   ├── css/
│   ├── img/
│   ├── js/
│   ├── api/
│   ├── index.html
│   ├── main.html
│   └── README.MD
├── backend/
│   ├── .mvn/
│   ├── src/
│   ├── .gitignore
│   ├── README.MD
│   ├── mvnw
│   ├── mvnw.cmd
│   └── pom.xml
└── README.MD
```

### Frontend

El frontend del proyecto está desarrollado utilizando HTML, CSS y JavaScript. Proporciona una interfaz de usuario interactiva para que los clientes naveguen, seleccionen productos y realicen pedidos.

#### Principales Archivos:
- **index.html**: Página principal que muestra los productos destacados y las categorías.
- **main.html**: Página secundaria que gestiona los detalles de los productos y el carrito de compras.
- **css/style.css**: Hojas de estilo para la interfaz de usuario.
- **js/**: Scripts JavaScript que manejan la lógica del cliente, como `auth.js`, `cart.js`, `product.js`, entre otros.
- **api/apirest.js**: Archivo JavaScript que contiene las funciones para interactuar con el backend utilizando AJAX.

### Backend

El backend del proyecto está construido con Spring Boot. Este gestiona todas las operaciones críticas del Ecommerce, incluyendo la autenticación de usuarios, la gestión de productos y pedidos, y la persistencia de datos en una base de datos MySQL.

#### Principales Características:
- **Spring Boot 3.3.2**: Framework utilizado para crear la aplicación backend.
- **JPA (Hibernate)**: Se usa para la persistencia de datos.
- **Spring Security**: Proporciona la autenticación y autorización de usuarios.
- **MySQL**: Base de datos relacional utilizada para almacenar los datos de la aplicación.
- **REST API**: Las operaciones CRUD y otras interacciones están expuestas a través de servicios REST.

#### Configuración:
- **application.properties**: Archivo de configuración principal que contiene las credenciales de la base de datos y otros parámetros importantes.
- **pom.xml**: Archivo de configuración de Maven que define las dependencias y plugins necesarios para la construcción del proyecto.

### Configuración y Ejecución

#### Prerrequisitos
- **Java 17** o superior
- **Node.js** (opcional, si se utiliza alguna herramienta de construcción o desarrollo frontend)
- **MySQL** (para la base de datos)
- **Maven** (para gestionar dependencias y construir el backend)

#### Instrucciones

1. **Clonar el repositorio**:
    ```bash
    git clone https://github.com/usuario/ProyectoFinal_Springboot
    cd ProyectoFinal_Springboot
    ```

2. **Configuración del Backend**:
   - Edita el archivo `backend/src/main/resources/application.properties` para configurar las credenciales de tu base de datos MySQL.
   - Construye y ejecuta la aplicación Spring Boot:
     ```bash
     cd backend
     mvn clean install
     mvn spring-boot:run
     ```

3. **Ejecución del Frontend**:
   - No se requieren pasos de compilación adicionales para el frontend.
   - Simplemente abre `frontend/index.html` en tu navegador para acceder a la interfaz de usuario.

4. **Acceso**:
   - Con el backend en ejecución, el frontend podrá interactuar con los endpoints RESTful del backend para gestionar productos, usuarios y pedidos.

### Problemas Conocidos y Solución de Problemas

- **Problemas de Conexión a la Base de Datos**: Asegúrate de que la base de datos MySQL esté corriendo y las credenciales en `application.properties` sean correctas.
- **Errores de CORS**: Si encuentras errores relacionados con CORS, verifica que las configuraciones en Spring Security estén correctamente configuradas para permitir el acceso desde el frontend.

### Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir, por favor sigue el flujo estándar de [Fork & Pull Request](https://guides.github.com/activities/forking/).
