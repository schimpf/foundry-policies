# Factura: fecha de vencimiento y facturas vencidas

> Fija el plazo de pago, calcula la fecha de vencimiento y sabe cuándo una factura está vencida, con un ejemplo y una rutina de cobro.

- Web: https://apps.schimpf.es/offline-trades-field-forms/es/invoice-due-date-and-overdue/
- App: Field Forms: Partes de obra, https://apps.schimpf.es/offline-trades-field-forms/es/index.md
"Pago a 14 días" parece claro hasta que alguien pregunta cuándo es el día 14 o desde cuándo la factura va con retraso. Esta página explica cómo contar los días, qué significa factura vencida y cómo llevar el control sin una hoja de cálculo.

## La fórmula

- **Fecha de vencimiento** = fecha de factura + plazo de pago (en días).
- **Vencida** = la factura está sin pagar y hoy es posterior a la fecha de vencimiento.

Una factura que vence el 17 de marzo sigue en plazo el 17 de marzo. Pasa a estar vencida el 18 de marzo. Una factura pagada nunca está vencida, por antigua que sea.

## Ejemplo

Emites una factura el 3 de marzo con un plazo de pago de 14 días.

1. Empieza el 3 de marzo.
2. Suma 14 días: 3 + 14 = 17, así que la fecha de vencimiento es el 17 de marzo.
3. El 17 de marzo la factura está pendiente, pero todavía no vencida.
4. El 18 de marzo lleva 1 día vencida.
5. El 25 de marzo lleva 8 días vencida.

Al cruzar el fin de mes se cuenta igual. Con un plazo de 30 días desde el 20 de junio, la fecha de vencimiento es el 20 de julio. Con 14 días desde el 25 de febrero en un año no bisiesto, vence el 11 de marzo.

| Fecha de factura | Plazo | Vencimiento | Primer día vencida |
|---|---|---|---|
| 3 de marzo | 14 días | 17 de marzo | 18 de marzo |
| 20 de junio | 30 días | 20 de julio | 21 de julio |
| 25 de febrero (año no bisiesto) | 14 días | 11 de marzo | 12 de marzo |

## Cómo elegir el plazo de pago

- **Los plazos cortos van bien para trabajos pequeños.** Entre siete y catorce días es habitual con particulares.
- **Los plazos largos van mejor con empresas,** que suelen tener su propio calendario de pagos. Acuérdalo antes de empezar.
- **Indica el plazo en el presupuesto,** así el cliente ya lo ha aceptado cuando recibe la factura.
- **Consulta la normativa.** Los derechos por impago y los intereses de demora cambian según el país y según si el cliente es una empresa o un consumidor. En España, la Ley 3/2004 de lucha contra la morosidad regula las operaciones comerciales entre empresas. Ante la duda, pregunta a tu gestor o a la Agencia Tributaria.

## Una rutina sencilla para reclamar el pago

1. **Envía la factura el mismo día** del trabajo, en PDF, al correo del propio cliente.
2. **Revisa las facturas pendientes una vez por semana.** Un día fijo funciona bien.
3. **El día del vencimiento** no hagas nada. Todavía no hay retraso.
4. **Con un día de retraso,** envía un recordatorio breve y amable con el número de factura y el importe.
5. **Con una semana de retraso,** llama al cliente.
6. **Marca la factura como pagada** el día que llegue el dinero, con la fecha de pago.

## Qué poner en la factura

Incluye estos datos en cada factura para que no haya nada que discutir después:

- El número de factura y la fecha de factura.
- La fecha de vencimiento, escrita como fecha y no solo como "14 días".
- El total a pagar, con el IVA en una línea aparte.
- El nombre de tu negocio, dirección, teléfono, correo y NIF.
- Cómo quieres cobrar, por ejemplo los datos de tu cuenta bancaria.

Con una fecha concreta no hay dudas sobre cuándo empieza la cuenta. Si el cliente firma antes un presupuesto, la fecha de factura es el día en que emites la factura.

## Anticipos y descuentos

Un anticipo que ya has recibido reduce lo que queda por pagar. Introdúcelo en la factura como una línea negativa, así el total muestra solo el resto. Los descuentos funcionan igual. En el ejemplo de la página sobre el total de la factura se ve cómo afecta esto al IVA.

## Llévalo en Offline Trades Field Forms

La app de Android **Offline Trades Field Forms** hace las cuentas de fechas por ti.

- El plazo de pago se fija una vez en los ajustes. Por defecto son 14 días, y la fecha de vencimiento se puede cambiar en cada factura.
- Un interruptor de pagada/pendiente guarda la fecha de pago.
- Una factura muestra **Overdue** (vencida) cuando está sin pagar y ha pasado su fecha de vencimiento. La etiqueta lleva texto y no solo color.
- Un trabajo muestra su estado más urgente: vencida, luego pendiente, luego presupuesto aceptado, luego borrador.
- El widget de la pantalla de inicio muestra el total de facturas pendientes y vencidas, con un botón para empezar un trabajo nuevo. Los importes se ocultan mientras el bloqueo de la app está activado.
- Las facturas se numeran solas (INV-0001 y siguientes), y un presupuesto firmado se convierte en factura con un toque.
- Funciona sin cobertura y sin cuenta. La app está en inglés.
