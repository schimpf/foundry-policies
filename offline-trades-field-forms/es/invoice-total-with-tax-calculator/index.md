# Total de factura con IVA: fórmula y calculadora

> Calcula el subtotal, el IVA y el total de una factura a partir de las líneas, con un ejemplo, reglas de redondeo y una calculadora sencilla.

- Web: https://apps.schimpf.es/offline-trades-field-forms/es/invoice-total-with-tax-calculator/
- App: Field Forms: Partes de obra, https://apps.schimpf.es/offline-trades-field-forms/es/index.md
Las facturas fallan por detalles pequeños: el IVA calculado sobre la cifra equivocada, un descuento aplicado dos veces o un céntimo de redondeo que hace que el total no coincida con la suma del cliente. Esta página muestra los pasos exactos, un ejemplo y una calculadora que puedes usar aquí mismo.

## La fórmula

Una factura con un solo tipo de IVA sigue tres pasos:

1. **Total de línea** = cantidad × precio unitario, en cada línea.
2. **Subtotal** (base imponible) = la suma de todos los totales de línea.
3. **IVA** = subtotal × tipo de IVA. **Total** = subtotal + IVA.

Los precios de las líneas se introducen sin IVA. El IVA se añade una sola vez, al final, sobre el subtotal. Así la factura es fácil de comprobar, con un tipo y una cuota de IVA.

## Ejemplo

Un técnico de calefacción factura mano de obra, una pieza y un descuento comercial. El tipo de IVA es del 21 %.

| Descripción | Cant. | Precio unitario | Total de línea |
|---|---|---|---|
| Mano de obra (horas) | 2,5 | 48,00 | 120,00 |
| Bomba | 1 | 86,40 | 86,40 |
| Descuento | 1 | -20,00 | -20,00 |

- Subtotal: 120,00 + 86,40 − 20,00 = 186,40
- IVA al 21 %: 186,40 × 0,21 = 39,144, redondeado 39,14
- Total: 186,40 + 39,14 = 225,54

El descuento es una línea con precio negativo. Como queda dentro del subtotal, el IVA se calcula sobre el importe reducido. Un anticipo ya cobrado funciona igual: introdúcelo como una línea negativa.

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/offline-trades-field-forms/es/invoice-total-with-tax-calculator/

## Reglas de redondeo

No existen fracciones de céntimo, así que cada paso se redondea a la unidad monetaria más pequeña. La app redondea "half up": un valor que termina justo en la mitad de una unidad se redondea alejándose de cero.

- Se redondea cada total de línea y después el IVA una vez más.
- Ejemplo: 1,5 × 3,33 = 4,995, redondeado 5,00.
- Ejemplo: el IVA de un subtotal de 10,03 al 17,5 % es 1,75525, redondeado 1,76.

La app guarda todos los importes como céntimos enteros y no usa números de coma flotante, por eso el resultado es siempre el mismo. El IVA se redondea una vez sobre el subtotal y no por línea. Así no aparece una diferencia entre las líneas y el total.

Algunas monedas, como el yen japonés, no tienen subunidad. La app lee el número de decimales del código de la moneda, por lo que esos importes se redondean a unidades enteras.

## Errores frecuentes

- **IVA sobre IVA.** No añadas IVA a precios que ya lo incluyen. Introduce precios sin IVA y deja que el total lo sume.
- **Descuento después del IVA.** Si restas el descuento del total en lugar del subtotal, el cliente paga IVA sobre el descuento.
- **Tipos mezclados.** Si una parte del trabajo lleva otro tipo de IVA, divídela en dos facturas o pregunta a tu gestor cómo reflejarlo. La app usa un solo tipo por documento.
- **Cantidad en minutos.** Usa horas con decimales: 90 minutos son 1,5 y 20 minutos son 0,333.

## Qué tipo de IVA usar

El tipo depende de dónde trabajas y de lo que vendes. Consúltalo en la Agencia Tributaria o con tu gestor. Esta página no indica el tipo de ningún país. El 21 % de arriba es solo un ejemplo.

## En la obra con Offline Trades Field Forms

En la app de Android **Offline Trades Field Forms** añades líneas con descripción, cantidad y precio unitario. La app hace las cuentas de arriba, suma el IVA con el tipo que fijas una vez en los ajustes y numera el documento automáticamente (INV-0001, INV-0002 y siguientes, con un prefijo que puedes cambiar).

- Fija un tipo de IVA por defecto y cámbialo en cada documento si hace falta.
- Introduce descuentos y anticipos como líneas negativas.
- Los presupuestos se convierten en factura con un toque cuando el cliente ha firmado en la pantalla.
- Las facturas tienen fecha de vencimiento, un interruptor de pagada y una marca de vencida.
- Todo funciona sin conexión y la factura sale de tu móvil en PDF desde el menú de compartir.
- La app está en inglés.
