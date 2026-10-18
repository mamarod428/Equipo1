# Fase 4 · Recursos · Equipo 1

## Introducción
La Fase 4 detalla la organización humana, tecnológica y metodológica del equipo para el desarrollo del proyecto. Define los roles técnicos, el reparto de responsabilidades por módulo de negocio, el herramental de desarrollo normalizado y los flujos de gestión en Git para asegurar una integración continua limpia durante todo el ciclo de vida del software.

## 1. Las personas

### Roles técnicos

| Persona | Rol | De qué responde |
| :--- | :--- | :--- |
| Dylan | Frontend Lead & UX | Revisa y aprueba los PRs de `client/`. Responde de la arquitectura en React, el estado global con Zustand y la navegación. |
| Rocío | Frontend Developer & Usabilidad | Implementación de vistas de cliente/técnico, maquetación con CSS nativo (CSS Modules), validación de formularios y captura de cámara. |
| Manuel | Backend Lead & Auth | Revisa y aprueba los PRs de `server/`. Responde de la arquitectura REST con Express, la seguridad con JWT y el procesamiento de ficheros (`multipart/form-data`). |
| José Luis | Database Manager & QA/DevOps | Responde del diseño y consistencia de esquemas BSON en MongoDB Atlas, integración de Cloudinary, flujo de ramas en Git y despliegues en Vercel/Render. |

### Responsables por módulo

| Módulo | Requisitos (RF del MVP) | Responsable | Apoyo |
| :--- | :--- | :--- | :--- |
| Autenticación y Usuarios | RF-01, RF-02 | Manuel | Dylan |
| Gestión de Presupuestos | RF-03, RF-04, RF-07 | Dylan | Rocío |
| Captura y Gestión de Tickets | RF-05, RF-06 | José Luis | Manuel |

### Comunicación
El canal principal de comunicación diaria, normas de convivencia y resolución de bloqueos están definidos en nuestro [docs/CONTRATO.md](../CONTRATO.md).

## 2. La tecnología

### Stack, servicios y APIs
El stack técnico MERN (MongoDB, Express, React, Node.js), junto con las bibliotecas auxiliares y sus correspondientes límites en capas gratuitas, están detallados y justificados en [02-viabilidad-tecnica.md](02-viabilidad-tecnica.md).

### Herramientas de desarrollo

| Para qué | Herramienta |
| :--- | :--- |
| Editor e Inspección de código | VS Code estandarizado con extensiones de ESLint y Prettier. |
| Entorno de ejecución | Node.js v20.x LTS (fijada la misma versión para todos los integrantes). |
| Pruebas de API REST | Bruno / Postman para validación de endpoints HTTP y tokens JWT. |
| Testing Frontend | Vitest para pruebas unitarias y de componentes en React. |
| Testing Backend | Jest + Supertest para pruebas de integración de la API Express. |

## 3. La gestión

### Tablero
La gestión de tareas y el seguimiento del sprint se realiza mediante un tablero Kanban en GitHub Projects, vinculado directamente a los Issues del repositorio.

### Ramas
- **Estructura:** La rama `main` contiene el código estable de producción. La rama `develop` actúa como base de integración.
- **Workflow:** Cada funcionalidad o corrección se desarrolla en una rama independiente creada desde `develop` con la nomenclatura `feature/nombre-tarea` o `fix/nombre-tarea`.
- **Integración:** Las tareas vuelven a `develop` únicamente mediante Pull Request (PR) aprobado. Al finalizar cada sprint, se realiza un PR de `develop` a `main`.
- **Protección:** Tanto `main` como `develop` están protegidas en GitHub, exigiendo la aprobación explícita de al menos 1 compañero (distinto del autor) para permitir el merge.

### Estructura de carpetas
El proyecto se organiza en la raíz en dos carpetas principales más la documentación:
- `client/`: contendrá la aplicación frontend en React.
- `server/`: contendrá la aplicación backend con Node.js y Express.
- `docs/`: documentación de la propuesta, contratos y especificaciones del proyecto.
