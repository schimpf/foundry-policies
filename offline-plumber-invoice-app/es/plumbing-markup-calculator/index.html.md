# Calculadora de margen sobre coste para fontaneros

> Calcula el precio de venta de tuberías, accesorios y piezas con tu coste y el % de recargo, y ve el margen que te queda. Fórmula y tabla.

- Web: https://apps.schimpf.es/offline-plumber-invoice-app/es/plumbing-markup-calculator/
- App: Facturas y Presupuestos, https://apps.schimpf.es/offline-plumber-invoice-app/es/index.md
## Fórmula del recargo para piezas de fontanería

El recargo (markup) es el porcentaje que sumas al coste de una pieza. El precio de venta es:

**precio de venta = coste × (1 + recargo ÷ 100)**

Un recargo del 35 % sobre una pieza que te cuesta 42,50 $ da 42,50 $ × 1,35 = 57,375 $, que se redondea a 57,38 $. Tu beneficio en la pieza es de unos 14,88 $.

La app redondea al céntimo hacia arriba desde la mitad. 57,375 pasa a 57,38 y 57,374 pasa a 57,37.

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/offline-plumber-invoice-app/es/plumbing-markup-calculator/

## Recargo y margen son números distintos

El recargo se mide sobre tu coste. El margen se mide sobre el precio de venta. La misma venta da dos porcentajes distintos.

- Recargo = beneficio ÷ coste
- Margen = beneficio ÷ precio de venta

Con un coste de 100 $ y un recargo del 30 %, el precio de venta es 130 $ y el beneficio es 30 $. El recargo es del 30 %. El margen es 30 $ ÷ 130 $ = 23,1 %.

Esto importa cuando un proveedor, un gestor o un libro de negocios habla de "margen". Si quieres un margen del 30 %, un recargo del 30 % se queda corto. Usa esta fórmula:

**recargo = margen ÷ (1 − margen)**

Para un margen del 30 % salen 0,30 ÷ 0,70 = 42,9 % de recargo.

## Tabla de recargo y margen

Todas las filas parten de un coste de 100 $.

| Recargo | Precio de venta | Beneficio | Margen |
|---------|-----------------|-----------|--------|
| 10 % | 110,00 $ | 10,00 $ | 9,1 % |
| 20 % | 120,00 $ | 20,00 $ | 16,7 % |
| 30 % | 130,00 $ | 30,00 $ | 23,1 % |
| 40 % | 140,00 $ | 40,00 $ | 28,6 % |
| 50 % | 150,00 $ | 50,00 $ | 33,3 % |
| 75 % | 175,00 $ | 75,00 $ | 42,9 % |
| 100 % | 200,00 $ | 100,00 $ | 50,0 % |

El margen nunca llega al 100 %, por alto que sea el recargo.

## Ejemplo: cambio de un calentador de agua

Imagina que compras estas piezas para un trabajo:

| Pieza | Cant. | Coste unidad | Recargo | Venta unidad | Total de línea |
|-------|-------|--------------|---------|--------------|----------------|
| Calentador de agua, 50 galones (unos 190 l) | 1 | 540,00 $ | 25 % | 675,00 $ | 675,00 $ |
| Flexible de conexión | 2 | 11,40 $ | 40 % | 15,96 $ | 31,92 $ |
| Vaso de expansión | 1 | 38,75 $ | 40 % | 54,25 $ | 54,25 $ |

El total de línea es la cantidad por el precio de venta, redondeado al céntimo. Las piezas suman 761,17 $ antes de impuestos y mano de obra.

Las piezas distintas suelen llevar recargos distintos. Los artículos grandes y fáciles de comparar, como un calentador, suelen llevar un porcentaje menor que los accesorios pequeños, porque el cliente puede buscar el precio del artículo grande en internet.

## Qué incluir en el coste

Empieza por el precio que pagas al proveedor. Después suma los costes que asumes con cada pieza, o se comen tu beneficio:

- El viaje al almacén, en tiempo o en combustible
- Las devoluciones que pagas tú cuando una pieza no es la correcta
- Las visitas de garantía por piezas que has suministrado

Un recargo pequeño sobre un accesorio de 3 $ rara vez cubre un viaje de 40 minutos. Por eso muchos fontaneros ponen un recargo más alto a las piezas pequeñas.

## Cómo trata la app el recargo

Offline Plumber Invoice App tiene un libro de precios con unos 120 artículos habituales de fontanería en ocho categorías: tubería, accesorios, válvulas, calentadores de agua, sanitarios, desagües, gas y mano de obra. Los artículos vienen sin precio.

1. Abre un artículo e introduce tu coste por unidad.
2. Introduce un recargo en % para ese artículo, o déjalo vacío para usar el recargo por defecto de tu perfil de empresa. Empieza en el 0 %.
3. El artículo muestra el precio de venta, por ejemplo "Sell price $57.38 / each".
4. Añade el artículo a un presupuesto. La línea toma el precio de venta y aún puedes cambiar el precio en la línea.

La app usa la fórmula de arriba con céntimos enteros y redondea hacia arriba desde la mitad. El recargo puede llegar al 1000 %. Un artículo sin coste no tiene precio, y el presupuesto no se puede firmar hasta que todas las líneas tengan uno.

Los artículos de mano de obra se marcan como mano de obra y no llevan impuesto por defecto. Para ver qué pasa después de fijar el precio, consulta [cómo un presupuesto suma el impuesto sobre las ventas y el depósito](../plumbing-quote-sales-tax-and-deposit/).

La app está pensada para fontaneros de EE. UU. y calcula en dólares. La app se usa en inglés.
