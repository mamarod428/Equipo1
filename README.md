#  Gestor de Negocios

> Aplicación web *mobile-first* de fricción cero para profesionales de oficios tradicionales.

La digitalización empresarial suele olvidar a quienes trabajan a pie de calle. **Gestor de Negocios** es una solución diseñada para eliminar la burocracia, la pérdida de ventas por presupuestos tardíos y la fuga de liquidez causada por el extravío de justificantes físicos en papel. Permite a los técnicos realizar sus gestiones diarias directamente desde su teléfono móvil y en el lugar de trabajo, sin complejas interfaces contables.

##  Características principales (MVP)

Nuestro Producto Mínimo Viable se centra en reducir a cero la fricción operativa mediante flujos de trabajo rápidos y eficientes:

-  **Presupuestos *in situ*:** Creación y emisión de presupuestos frente al cliente en menos de 3 minutos.
-  **Integración con WhatsApp:** Envío inmediato de propuestas mediante un enlace temporal a través de la app nativa de WhatsApp.
-  **Captura inteligente de gastos:** Toma de fotografías de tickets de compra usando la cámara del navegador móvil en menos de 30 segundos.
-  **Trazabilidad:** Vinculación instantánea de los tickets de gastos con su presupuesto correspondiente.

##  Stack Tecnológico

El proyecto está construido bajo una arquitectura MERN, optimizada para un rendimiento fluido en pantallas táctiles de gama baja mediante el uso de CSS nativo.

**frontend:**
- react (con vite)
- zustand (gestor de estado global)
- css nativo (variables y modules, sin frameworks pesados)
- axios & react hook form
- despliegue en vercel

**backend:**
- node.js & express
- autenticación segura (JWT & bcrypt)
- multer (gestión de ficheros)
- despliegue en render

**base de datos & almacenamiento:**
- mongoDB atlas (esquemas BSON)
- cloudinary (almacenamiento multimedia efímero para tickets)

##  Desarrollado por:

Desarrollado bajo metodologías ágiles y flujos de trabajo estrictos en git (Integración Continua):

- **Dylan Bauti Huelva:** Frontend lead & UX (arquitectura react, estado global, navegación)
- **Rocío Luque Montes:** Frontend developer & asabilidad (vistas, maquetación CSS, formularios, cámara)
- **Manuel Amado Rodríguez:** Backend lead & Auth (arquitectura REST, seguridad JWT, procesamiento de ficheros)
- **José Luis Yuani Barea:** Database manager & QA/DevOps (mongoDB, cloudinary, flujo git, despliegues)

---
*Desarrollado para facilitar el día a día de los profesionales que trabajan con las manos.*

## Tablero de Trabajo
[Acceso a la documentación del proyecto](https://github.com/users/mamarod428/docs/propuesta.md)

[Acceso al tablero del proyecto](https://github.com/users/mamarod428/projects/7)

---
