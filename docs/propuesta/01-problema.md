# Propuesta: Gestor de negocios

*Introducción*
La digitalización empresarial ha marginado a un sector fundamental: los profesionales de oficios que trabajan a pie de calle. Mientras el mercado desarrolla complejas herramientas de gestión administrativa para entornos de oficina, el técnico autónomo sigue dependiendo del papel, el bolígrafo y la memoria. Esta brecha tecnológica provoca fugas de capital por ventas no cerradas y una carga burocrática inasumible al final de la jornada. Nuestro proyecto nace para resolver este problema mediante el diseño de interfaces (UX): una solución puramente móvil, táctil y de fricción cero, adaptada a la realidad de quien trabaja con las manos y necesita agilidad frente al cliente.

## 1. Identificación de la necesidad
*   *El problema:* Los autónomos pierden clientes por el retraso en la elaboración y envío de presupuestos. Además, la perdida constante de justificantes y tickets de compra físicos en papel genera pérdidas económicas al no poder deducir esos gastos.
*   *A quién afecta:* Autónomos y pequeños negocios de oficios tradicionales (electricistas, fontaneros, reformas, climatización) con baja alfabetización digital y cuya jornada laboral transcurre íntegramente fuera de una oficina.
*   *Frecuencia:* Diaria. Un técnico promedio realiza múltiples visitas a clientes y acude a almacenes de suministros varias veces en una misma jornada.
*   *Impacto:* Pérdida directa de ingresos por ventas no cerradas en caliente, problemas contables y pérdida de tiempo personal.
*   *Evidencias:* Foros de autónomos llenos de quejas sobre la burocracia, furgonetas comerciales acumulando facturas arrugadas en las guanteras, y valoraciones de una estrella en CRMs móviles quejándose de que "piden demasiados datos para hacer una factura rápida".
*   
## 2. Usuarios Objetivo y Casos de Uso

### User Persona 1: Paco, 52 años, Electricista Autónomo
*   *Necesidades:* Dar un precio cerrado al cliente en menos de 3 minutos, justo después de diagnosticar la avería, sin tener que teclear.
*   *Frustraciones:* Odia llegar a casa a las 20:00 y encender el ordenador para hacer cuentas en Excel. Los teclados de móvil pequeños le desesperan cuando tiene las manos sucias. Le abruma la jerga técnica (NIF, bases imponibles, devengos).
*   *Objetivos:* Cerrar el trato en persona, no perder ningún ticket de compra y tener las tardes libres de papeleo.
*   *Casos de uso principales:* 
    1. Pulsar 3 iconos visuales (ej. "Tubería" + "Mano de obra"), generar un enlace temporal y enviarlo por WhatsApp al cliente. 
    2. Hacer una foto al ticket de la ferretería y asociarlo a un trabajo activo con un clic.

### User Persona 2: Elena, 41 años, Clienta Particular
*   *Necesidades:* Obtener un presupuesto claro, desglosado y por escrito para aprobar una reparación en su domicilio.
*   *Frustraciones:* Recibir presupuestos informales mediante notas de voz ("te va a salir por unos 800€") que luego cambian, o tener que abrir PDFs pesados en el correo y responder formalmente.
*   *Objetivos:* Aprobar el gasto rápidamente desde su teléfono móvil y tener un registro de lo acordado.
*   *Casos de uso principales:* 
    1. Recibir un WhatsApp, abrir la URL del presupuesto, revisar el desglose y pulsar el botón "Aceptar".


## 3. Análisis de Competencia

*   *Competidor 1: Holded / Qonto*
    *   Fortalezas: Ecosistema financiero robusto, control de inventario, contabilidad legal y conciliación bancaria completa.
    *   Debilidades: Curva de aprendizaje extrema. Interfaz diseñada para administrativos con ratón y teclado. La versión móvil está saturada de menús contables que paralizan al técnico que solo quiere dar un precio.
*   *Competidor 2: FacturaDirecta / Billin*
    *   Fortalezas: Muy eficaces para la emisión legal de facturas en Pymes.
    *   Debilidades: Fricción de entrada inasumible en movilidad. Exigen rellenar una ficha completa de cliente (Nombre, Dirección, NIF, Código Postal) antes de permitir añadir una sola línea de "Mano de obra". Rompen la inmediatez del trabajo de campo.
*   *Competidor 3: Libreta de papel + WhatsApp*
    *   Fortalezas: Flexibilidad total, cero coste y cero curva de aprendizaje.
    *   Debilidades: Descontrol absoluto. El cliente no tiene desglose profesional, los presupuestos se entierran en el historial de chat, los tickets físicos se pierden y no hay vinculación entre el ingreso acordado y el material gastado.
*   *Oportunidades:* Ninguna app grande está atacando la "fase preventiva y operativa" con una experiencia UX puramente móvil, táctil y asíncrona mediante enlaces web.

## 4. Propuesta de Valor Única

Al *profesional de oficios tradicionales* le pasa que *pierde ventas por no poder entregar un presupuesto rápido in situ y pierde liquidez al extraviar justificantes físicos de compra. Hoy usa **el clásico bloc de notas o herramientas contables complejas (como Holded o FacturaDirecta), que fallan por **exigir la introducción manual de demasiados datos fiscales, estar diseñadas para ordenador y romper la inmediatez del trabajo de campo. Nosotros le damos **una aplicación web de bolsillo que permite generar presupuestos visuales en tres clics para su aceptación directa vía WhatsApp, y que archiva los gastos al instante utilizando únicamente la cámara del móvil*.
