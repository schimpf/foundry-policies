# Presupuesto de fontanería: impuesto sobre ventas y depósito

> Cómo sumar el impuesto sobre ventas solo a las líneas sujetas, fijar un % de depósito sobre el total y hallar el saldo pendiente. Ejemplo y calculadora.

- Web: https://apps.schimpf.es/offline-plumber-invoice-app/es/plumbing-quote-sales-tax-and-deposit/
- App: Facturas y Presupuestos, https://apps.schimpf.es/offline-plumber-invoice-app/es/index.md
## Las tres cifras de un presupuesto

Un presupuesto de fontanería termina con tres importes: el impuesto, el total y el depósito. Dependen unos de otros en un orden fijo. El impuesto sobre las ventas (sales tax) es el impuesto de venta de EE. UU., que se suma al precio.

1. Suma todas las líneas. Cada línea es cantidad × precio unitario, redondeado al céntimo. Es el subtotal.
2. Suma solo las líneas marcadas como sujetas a impuesto. Multiplica ese importe por el tipo de impuesto. Es el impuesto.
3. Subtotal más impuesto es el total.
4. Multiplica el total por el porcentaje de depósito. Es el depósito.
5. Total menos lo que el cliente ya ha pagado es el saldo pendiente.

Offline Plumber Invoice App sigue exactamente este orden. Redondea hacia arriba desde la mitad al céntimo, así que 223,797 pasa a 223,80.

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumber-invoice-app/es/plumbing-quote-sales-tax-and-deposit/

## Ejemplo: cambio de tuberías en un baño

El trabajo tiene estas líneas:

| Línea | Cant. | Precio unitario | Sujeta a impuesto | Total de línea |
|-------|-------|-----------------|-------------------|----------------|
| Tubería PEX, 3/4 in (20 mm) | 100 ft (unos 30 m) | 1,20 $ | sí | 120,00 $ |
| Accesorios y válvulas | 1 | 292,00 $ | sí | 292,00 $ |
| Mano de obra | 6 h | 50,00 $ | no | 300,00 $ |

- Subtotal: 120,00 $ + 292,00 $ + 300,00 $ = 712,00 $
- Base sujeta a impuesto: 120,00 $ + 292,00 $ = 412,00 $
- Impuesto al 8,25 %: 412,00 $ × 0,0825 = 33,99 $
- Total: 712,00 $ + 33,99 $ = 745,99 $
- Depósito al 30 %: 745,99 $ × 0,30 = 223,797 $, redondeado a 223,80 $
- Saldo tras el depósito: 745,99 $ − 223,80 $ = 522,19 $

El tipo de impuesto es un único tipo combinado, tal como aparece en la tabla de tipos de tu zona (estado más condado más ciudad). La app toma un tipo por documento.

## Impuesto sobre las líneas, no sobre el total

El impuesto se aplica a la base sujeta. En el ejemplo, aplicarlo a los 712,00 $ completos daría 58,74 $, es decir 24,75 $ de más. Si la mano de obra lleva impuesto depende del estado y del tipo de trabajo. Algunos estados gravan la mano de obra de reparación, otros solo los materiales, y algunos tratan la obra nueva de forma distinta a la reparación. Busca la norma de tu estado en la web del departamento de hacienda estatal (Department of Revenue) o pregunta a tu gestor antes de preparar tus líneas.

En la app, cada línea tiene su propia casilla de impuesto. Los artículos del libro de precios marcados como mano de obra empiezan sin impuesto y los demás empiezan con impuesto. Puedes cambiar cualquiera de los dos en la línea. Cada presupuesto tiene su propio tipo de impuesto y su propio % de depósito, y un presupuesto nuevo parte de los valores por defecto de tu perfil de empresa.

## El depósito es una parte del total

El porcentaje de depósito se aplica al total con impuesto. Un depósito del 30 % sobre 745,99 $ son 223,80 $. Cóbralo antes de pedir material o empezar en trabajos grandes.

El depósito no tiene documento propio. Cuando lo cobras, lo registras como un cobro en la factura, con la fecha y un método: efectivo, cheque u otro. La factura muestra entonces el saldo pendiente. En el ejemplo, un segundo cobro de 200,00 $ con cheque deja 322,19 $.

## Qué comprueba la app por ti

- Un presupuesto no se puede firmar sin líneas ni con una línea sin precio.
- El impuesto y el depósito se actualizan mientras escribes.
- No puedes registrar un cobro mayor que el saldo pendiente.
- Cuando el cliente firma con el dedo, el presupuesto queda bloqueado. Con un toque pasa a factura y las líneas se copian.
- El estado de la factura pasa a "Partially paid" tras el primer cobro y a "Paid" cuando los cobros cubren el total.

Para fijar antes el precio de una pieza, consulta la [fórmula del recargo y la tabla para fontanería](../plumbing-markup-calculator/).

La app funciona sin cobertura. Puedes hacer el presupuesto en un sótano, recoger allí la firma y enviar el PDF después desde la bandeja de salida (Outbox).

La app calcula en dólares con un tipo de sales tax por documento. No calcula IVA.
