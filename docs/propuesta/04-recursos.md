## Introducción
La Fase 4 detalla la organización humana, tecnológica y metodológica del equipo para el desarrollo del proyecto. Define los roles técnicos, el reparto de responsabilidades por módulo de negocio, el herramental de desarrollo normalizado y los flujos de gestión en Git para asegurar una integración continua limpia durante todo el ciclo de vida del software.

## 1. Las personas

### Roles técnicos

| Persona | Rol | De qué responde |
| :--- | :--- | :--- |
| *José luis* | Frontend Lead & UX | Revisa y aprueba los PRs de client/. Responde de la usabilidad mobile-first, el diseño en Tailwind CSS y el estado global en React (Zustand). |
| *Dylan* | Backend Lead & Auth | Revisa y aprueba los PRs de server/. Responde de la arquitectura REST con Express, la seguridad con JWT y el procesamiento de archivos (multipart/form-data). |
| *Manuel* | Database Manager & QA/DevOps | Responde del diseño y consistencia de esquemas BSON en MongoDB Atlas, la integración con Cloudinary, el pipeline de Git y los despliegues en Vercel/Render. |

### Responsables por módulo

| Módulo | Requisitos (RF del MVP) | Responsable | Apoyo |
| :--- | :--- | :--- | :--- |
| *Autenticación y Usuarios* | RF-01, RF-02 | José luis | Dylan |
| *Gestión de Presupuestos* | RF-03, RF-04 | Dylan | Manuel |
| *Captura y Gestión de Tickets* | RF-05, RF-06 | José luis | Manuel |

### Comunicación
El canal principal de comunicación diaria, normas de convivencia y resolución de bloqueos están definidos en nuestro [docs/CONTRATO.md](../CONTRATO.md).

## 2. La tecnología

### Stack, servicios y APIs
El stack técnico MERN (MongoDB, Express, React, Node.js), junto con las bibliotecas auxiliares y sus correspondientes límites en capas gratuitas, están detallados y justificados en [02-viabilidad-tecnica.md](../02-viabilidad-tecnica.md).

### Herramientas de desarrollo

| Para qué | Herramienta |
| :--- | :--- |
| *Editor e Inspección de código* | VS Code estandarizado con extensiones de ESLint y Prettier. |
| *Entorno de ejecución* | Node.js v20.x LTS (fijada la misma versión para todos los integrantes). |
| *Pruebas de API REST* | Bruno / Postman para validación de endpoints HTTP y tokens JWT. |
| *Testing Frontend* | Vitest para pruebas unitarias y de componentes en React. |
| *Testing Backend* | Jest + Supertest para pruebas de integración de la API Express. |
