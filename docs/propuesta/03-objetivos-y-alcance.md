# Objetivos y alcance

**Equipo:** <Equipo 1>

## Introducción

En la Fase 3 se definen los límites y las metas medibles del proyecto **“Gestor de Negocios”**.

Una vez validada la viabilidad técnica en las fases anteriores, este documento:

- Fija los objetivos SMART que servirán para la evaluación final.
- Acota el alcance del Producto Mínimo Viable (MVP).
- Deja constancia de las líneas de desarrollo que quedan fuera de esta iteración.

## 1. Objetivos

### Objetivo general

Facilitar que los profesionales de oficios tradicionales puedan emitir presupuestos y guardar sus tickets de gasto en el momento, desde el móvil y directamente en el lugar de trabajo, eliminando la carga administrativa al acabar la jornada.

### Objetivos específicos

| ID         | Objetivo SMART                                                             | Qué se mide                                                                                                         | Valor de éxito                    | Cómo se comprueba                                                                       |
|------------|----------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|-----------------------------------|-----------------------------------------------------------------------------------------|
| **OBJ-01** | Emisión rápida de presupuestos *in situ* tras diagnosticar una avería.     | Tiempo transcurrido desde que se inicia la creación del presupuesto hasta que se genera el enlace de WhatsApp.      | Menos de 3 minutos.               | Prueba cronometrada con 3 autónomos en sus móviles antes de la defensa final.           |
| **OBJ-02** | Captura y archivo inmediato de justificantes de compra desde la web móvil. | Tiempo total desde que se abre la cámara hasta que la foto del ticket se guarda en la nube y se vincula en la BBDD. | Menos de 30 segundos.             | Registro de tiempos en cliente/servidor mediante pruebas de rendimiento en red 4G real. |
| **OBJ-03** | Consulta y aprobación de presupuestos por el cliente sin fricción.         | Tiempo de carga y aprobación del presupuesto a través del enlace de WhatsApp, sin necesidad de registro.            | Menos de 1 minuto.                | Pruebas de usabilidad con 3 clientes en sus propios smartphones.                        |
| **OBJ-04** | Optimización del uso de datos móviles en la subida de fotos de tickets.    | Peso final de la imagen enviada a la API de almacenamiento.                                                         | Inferior a 500 KB por fotografía. | Comprobación directa de metadatos en el panel de Cloudinary.                            |

## 2. Alcance

### El MVP

El Producto Mínimo Viable y su flujo de trabajo están detallados en [`02-viabilidad-tecnica.md`](02-viabilidad-tecnica.md).

El alcance se limita estricta y exclusivamente a los **6 requisitos clasificados como Must have**:

- Autenticación del técnico.
- Creación rápida de presupuestos.
- Generación de enlaces temporales.
- Captura fotográfica de tickets.
- Vinculación ticket-presupuesto.

### Plataforma

- **Tipo:** Aplicación web con enfoque estrictamente *mobile-first*.
- **Compatibilidad:** Optimizada para navegadores móviles Chrome y Safari en iOS y Android.
- **Exclusiones:** No se desarrollarán aplicaciones nativas para App Store ni Google Play Store.

### Usuarios y datos

- **Usuarios:** 1 rol activo, correspondiente al autónomo o técnico.
- **Clientes finales:** Acceso público mediante un token único.
- **Entorno de datos:** Datos de prueba (*seed data*) que simulan la actividad diaria de autónomos, incluyendo:
    - Clientes ficticios.
    - Presupuestos de prueba.
    - Fotografías reales de tickets comprimidas.

## 3. Lo que no haremos

| Funcionalidad excluida                         | Motivo                                                                                                                                 |
|------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| **Conciliación bancaria y cobros *in-app***    | Añade una complejidad elevada de integración con APIs bancarias y supone un riesgo de seguridad innecesario para el tiempo del módulo. |
| **Gestión de inventario y stock**              | Evita recargar la interfaz táctil con formularios largos, manteniendo el principio de cero fricción en movilidad.                      |
| **Generación de facturas contables oficiales** | El proyecto se enfoca en el trabajo de campo —presupuestos y tickets—. La facturación fiscal queda pospuesta para fases futuras.       |

## 4. Ampliaciones futuras

### Generación automática de facturas en PDF

Conversión, con un solo clic, de presupuestos aceptados a un PDF descargable.

### Exportación de gastos para gestorías

Generación de un archivo comprimido (`.zip`) con todos los tickets de un periodo determinado para enviarlo al gestor.

### PWA (Progressive Web App)

Conversión del proyecto a una PWA para permitir:

- La instalación en la pantalla de inicio del móvil.
- El soporte fuera de línea (*offline*).