# Viabilidad Técnica · <Equipo 1>

## 1. Análisis de Requisitos Funcionales y Priorización (MoSCoW)

### Must have 

1. Registrar un nuevo usuario (autónomo/técnico) en el sistema.
2. Iniciar sesión en la aplicación móvil con credenciales seguras.
3. Crear un presupuesto añadiendo líneas de concepto rápidas (ej. “Mano de obra”, “Material”).
4. Generar un enlace público temporal para compartir un presupuesto.
5. Subir una fotografía desde la cámara del móvil de un ticket de compra.
6. Asociar la fotografía de un ticket a un presupuesto/trabajo en curso.

### Should have 

7. Aceptar o rechazar un presupuesto desde el enlace público (vista del cliente).
8. Listar el histórico de presupuestos con su estado (pendientes, aceptados, rechazados).
9. Listar los gastos acumulados a partir de los tickets fotografiados en un mes.
10. Redirigir automáticamente a la app nativa de WhatsApp con un mensaje predefinido que incluya el enlace.

### Could have 

11. Calcular el beneficio neto de un trabajo restando los tickets asociados al total presupuestado.
12. Descargar un presupuesto aceptado en formato PDF.

### Won't have

13. Integrar con cuentas bancarias para la conciliación de pagos.
14. Gestionar el inventario y stock físico de los materiales del almacén.

## 2. Producto Mínimo Viable (MVP)

El MVP se compone estrictamente de los 6 requisitos funcionales catalogados como **Must have**. Todo lo demás queda fuera de esta primera iteración.

### Recorrido mínimo del usuario:

- Acceso: Abre la aplicación móvil e inicia sesión con su cuenta.

- Creación: Tras diagnosticar una avería in situ, crea un nuevo presupuesto añadiendo líneas de gasto básicas (material y mano de obra).

- Envío: Genera un enlace público temporal de ese presupuesto y se lo envía a su cliente por WhatsApp para que lo vea al instante.

- Registro de gasto: Al salir, pasa por el almacén a comprar repuestos. Toma una fotografía del ticket físico de papel usando la cámara de la propia aplicación.

- Asociación: Asocia esa fotografía al presupuesto recién creado, dejando el gasto registrado y resolviendo su problema principal sin necesitar un ordenador.