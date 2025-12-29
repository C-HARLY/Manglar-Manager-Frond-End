#  Manglar Manager - Frontend Client

> **Interfaz de usuario web para la plataforma de gestión empresarial Manglar Manager.**

![React](https://img.shields.io/badge/React-v18-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![Socket.IO](https://img.shields.io/badge/Socket.IO-Client-black)

##  Descripción

Este repositorio contiene el código fuente de la **Single Page Application (SPA)** de Manglar Manager. Es la cara visible del sistema, diseñada para ofrecer una experiencia fluida e intuitiva a administradores y empleados.

La aplicación consume la API del Backend para la gestión de datos y mantiene una conexión persistente mediante **WebSockets** para el módulo de chat en tiempo real.

---

##  Características de la Interfaz

* * Arquitectura de Componentes:** Desarrollo modular utilizando React.js.
* * Gestión de Sesiones:** Manejo de autenticación (Login) y persistencia de sesión segura.
* * Diseño Responsivo:** Adaptable a diferentes tamaños de pantalla.
*   Chat Interactivo:** Cliente de **Socket.IO** integrado para mensajería instantánea sin recargas.
* **Rutas Protegidas:** Sistema de navegación que restringe el acceso a ciertas páginas según el rol del usuario (Admin vs Empleado).

---

##  Stack Tecnológico

* **Librería Principal:** React.js (Hooks & Functional Components)
* **Enrutamiento:** React Router DOM
* **Peticiones HTTP:** [Axios / Fetch API]
* **Tiempo Real:** Socket.io-client
* **Estilos:** [CSS Modules / Bootstrap] 
* **Iconos:** [React Icons / FontAwesome]

---

##  Galería de Vistas (Screenshots)



| Inicio de Sesión | Panel Principal (Dashboard) |
|:---:|:---:|
| ![Login](./src/img/manglar%20login.png) | ![Logeo exitoso](./src/img/manglar%20logeado.png) |

| Menu | Panel Principal Usuario  |
|:---:|:---:|
| ![Crear usuario](./src/img/crear%20manglar.png) | ![Guardado exitoso](./src/img/Guardar%20Manglar.png) |

| Menu | Panel Departamentos |
|:---:|:---:|
| ![Crear usuario](./src/img/Depertamentos%20Manglar.png) | 


| Menu | Perfil  |
|:---:|:---:|
| ![Crear usuario](./src/img/User%20profile.png) | 


| Menu | Tareas pendientes  |
|:---:|:---:|
| ![Crear usuario](./src/img/TAREAS%20PENDIENTES%20USER.png) | 



| Chat en Vivo | Gestión de Tareas |
|:---:|:---:|
| ![Chat Vista Administrador ](./src/img/Chatear%20con%20usuarios%20admin.png) | ![Chat Vista Usuario](./src/img/Chat%20vista%20user.png) |

---

##  Estructura del Proyecto

Organización estándar de una aplicación React escalable:

```text
/src
  ├── /assets         # Imágenes, fuentes y estilos globales
  ├── /components     # Componentes reutilizables (Botones, Inputs, Navbar)
  ├── /context        # Context API (Estados globales de Auth o Chat)
  ├── /hooks          # Custom Hooks
  ├── /pages          # Vistas principales (Login, Dashboard, Chat)
  ├── /services       # Lógica de conexión a la API (Endpoints)
  ├── App.js          # Componente raíz y Rutas
  └── index.js        # Entry point
```


##  Instalación y Despliegue

1.  **Clonar el repositorio:**
    ```bash
    git clone https://github.com/C-HARLY/Manglar-Manager-Frond-End.git
    ```
2.  **Instalar dependencias:**
    Este paso es vital porque descarga todas las librerías necesarias (React, Socket.IO, etc.):
    ```bash
    npm install
    ``
3.  **Iniciar la aplicación:**
    ```bash
    npm start
    ```
    *La aplicación se abrirá automáticamente en tu navegador en http://localhost:5173*


    ##  Credenciales de Acceso 

Para facilitar la revisión del proyecto y probar todas las funcionalidades (como la gestión de tareas y departamentos), puedes utilizar la cuenta de **Administrador** predeterminada:

| Rol | Usuario (Username) | Contraseña (Password) |
| :--- | :--- | :--- |
| **Administrador** | `ADMINA` | `admin` |

> **Nota:** Con este usuario tendrás acceso total al Dashboard, panel de chat y asignación de tareas.