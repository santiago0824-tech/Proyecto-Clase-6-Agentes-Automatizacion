# Proyecto · Clase 6 · Ana decide qué delegar del reporte semanal de ventas

**Tema:** Agentes y automatización  
**Rol:** Ana (Ventas)  
**Empresa:** Distribuidora Solmar

## 1. Mi flujo de trabajo

Para ayudar a Ana a reducir el tiempo que dedica a elaborar el reporte semanal, propongo un flujo en el que la IA se encargue de organizar, clasificar y calcular la información. Sin embargo, Ana conservará la responsabilidad de revisar y aprobar el reporte final.

| Pieza | ¿Cómo funcionaría? |
|---|---|
| **1. Disparador** | Todos los lunes a las 9:00 a. m., cuando termina el plazo para recibir los reportes de los tres vendedores. |
| **2. Registro** | La IA recibe los reportes de Beto, Carla y Mauricio, identifica los folios, clientes, montos y estatus, y organiza la información en una sola tabla. |
| **3. Decisión** | La IA considera una venta válida únicamente cuando está facturada dentro de la semana anterior, de lunes a domingo. Excluye pedidos cancelados, cotizaciones y folios repetidos. Los casos dudosos se envían a Ana para su revisión. |
| **4. Respuesta** | La IA prepara un borrador con las ventas de cada vendedor, el porcentaje de cumplimiento de su meta, el total del equipo y las operaciones excluidas. Ana revisa y aprueba el documento antes de enviarlo al Director Comercial a las 11:00 a. m. |
| **5. Evidencia** | Se conserva una tabla con las ventas aceptadas, las excluidas, sus motivos y los cálculos realizados. Ana revisa esta evidencia cada lunes antes de aprobar el reporte. |

## 2. Lo que no delegaría

No dejaría que la IA enviara directamente el reporte al Director Comercial, porque un error en los montos o en la clasificación de las ventas podría afectar las decisiones de la empresa.

Tampoco le delegaría la resolución de situaciones confusas, como folios con información diferente, facturas sin confirmar o ventas cuyo estatus no esté claro. Esos casos deben pasar directamente con Ana para que pueda verificar los datos con el vendedor correspondiente.

La IA sería una herramienta de apoyo, pero Ana conservaría la responsabilidad de validar la información y autorizar el envío.

## 3. Mi prueba con los reportes de este lunes

### Prompt que utilicé

Le indiqué al asistente que actuara como auxiliar de operaciones de ventas y que organizara los tres reportes siguiendo las reglas de Distribuidora Solmar.

**Instrucciones para el asistente:**

Analiza los siguientes reportes de ventas de Beto Ríos, Carla Núñez y Mauricio Pérez.

Aplica estas reglas:

- Una venta cuenta únicamente si está facturada dentro de la semana reportada.
- No cuentes pedidos cancelados, cotizaciones ni folios repetidos.
- La meta individual es de $60,000 por vendedor.
- La meta del equipo es de $180,000.
- Calcula las ventas válidas de cada vendedor y su porcentaje de cumplimiento.
- Calcula el total válido del equipo y su porcentaje de cumplimiento de la meta.
- Identifica las operaciones excluidas y explica el motivo.
- Si encuentras información dudosa o inconsistente, señálala para que Ana la revise.
- No inventes datos ni cambies el estatus de una venta.
- Prepara un borrador para el Director Comercial, pero no lo envíes. Ana debe aprobarlo primero.

### Datos que proporcioné

**Beto Ríos**

| Folio | Cliente | Monto | Estatus |
|---|---|---:|---|
| F-1041 | Papelería Lupita | $12,400 | Facturado |
| F-1042 | Abarrotes El Sol | $18,900 | Facturado |
| F-1044 | Miscelánea Norte | $9,500 | Cancelado |
| F-1045 | Super Hogar | $27,300 | Facturado |

Total reportado: $68,100.

**Carla Núñez**

- F-2210, Ferretería Centro: $31,000.
- F-2211, Mercado Verde: $22,500.
- F-2211, Mercado Verde: $22,500 (repetido).
- F-2213, Tienda La Esquina: $15,800.

Total reportado: $91,800.

**Mauricio Pérez**

- Papelería Central: $24,500, facturado.
- Cafetería Roma: $17,200, facturado.
- Hoteles del Valle: $33,000, en proceso de cierre.

Total reportado: $74,700.

### Resultado que entregó el asistente

#### A. Ventas válidas por vendedor

| Vendedor | Ventas válidas | Meta | Cumplimiento |
|---|---:|---:|---:|
| Beto Ríos | $58,600 | $60,000 | 97.67% |
| Carla Núñez | $69,300 | $60,000 | 115.50% |
| Mauricio Pérez | $41,700 | $60,000 | 69.50% |
| **Total del equipo** | **$169,600** | **$180,000** | **94.22%** |

#### B. Operaciones excluidas

| Vendedor | Operación | Motivo de exclusión |
|---|---|---|
| Beto Ríos | F-1044, Miscelánea Norte ($9,500) | Pedido cancelado. |
| Carla Núñez | Segunda aparición del folio F-2211 ($22,500) | Folio repetido; solo se cuenta una vez. |
| Mauricio Pérez | Hoteles del Valle ($33,000) | Está en proceso de cierre y todavía no está facturado. |

#### C. Borrador del reporte para el Director Comercial

**Asunto: Reporte semanal de ventas – Distribuidora Solmar**

Durante la semana reportada, el equipo registró ventas válidas por un total de **$169,600**, alcanzando un cumplimiento del **94.22%** de la meta establecida de $180,000.

Por vendedor, los resultados fueron:

- Beto Ríos: $58,600, equivalente al 97.67% de su meta.
- Carla Núñez: $69,300, equivalente al 115.50% de su meta.
- Mauricio Pérez: $41,700, equivalente al 69.50% de su meta.

Se excluyeron un pedido cancelado de Beto, un folio duplicado de Carla y una operación de Mauricio que todavía se encuentra en proceso de cierre.

El equipo quedó $10,400 por debajo de la meta semanal.

**Estado:** Borrador pendiente de revisión y aprobación de Ana.

## 4. Mi revisión

Al comparar los resultados con los reportes originales, comprobé que el asistente identificó correctamente las tres operaciones que no debían contarse. También detecté que los totales originales de Beto y Carla incluían operaciones que no cumplían las reglas.

Además, revisé que Mauricio había expresado sus cantidades en miles de pesos, por lo que fue necesario convertirlas a pesos para mantener el mismo formato. Después de verificar las sumas y porcentajes, consideré que el borrador podía pasar a la aprobación de Ana.

## 5. Conclusión

Con este ejercicio comprendí que la inteligencia artificial puede ayudar a automatizar actividades repetitivas, como organizar reportes, identificar datos duplicados y realizar cálculos. Sin embargo, no es conveniente dejar que tome todas las decisiones o envíe información importante sin supervisión. Lo mejor es utilizarla como apoyo y mantener una revisión humana para evitar errores antes de entregar los resultados.
