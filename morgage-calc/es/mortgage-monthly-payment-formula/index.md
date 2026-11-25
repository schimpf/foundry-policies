# Fórmula de la cuota de una hipoteca, con ejemplo

> Cómo se calcula la cuota mensual de una hipoteca a tipo fijo: fórmula, ejemplo con 200.000 euros al 2,60 % a 30 años y una calculadora para probar.

- Web: https://apps.schimpf.es/morgage-calc/es/mortgage-monthly-payment-formula/
- App: Hipoteca: simulador y cálculo, https://apps.schimpf.es/morgage-calc/es/index.md
Una hipoteca a tipo fijo tiene la misma cuota todos los meses. Sale de una sola fórmula, la del sistema francés de amortización (también llamada anualidad). Esta página explica la fórmula, resuelve un ejemplo a mano y muestra adónde va el dinero.

## La fórmula

**Cuota = C × i / (1 − (1 + i)^−n)**

- **C** es el capital del préstamo.
- **i** es el tipo mensual: el tipo anual (TIN) dividido entre 12.
- **n** es el número de cuotas mensuales: años × 12.

Si el tipo es 0 %, la fórmula no sirve (divide entre cero). La cuota es entonces C / n.

## Ejemplo resuelto

Préstamo de 200.000 euros, TIN del 2,60 %, 30 años.

1. Tipo mensual: i = 0,026 / 12 = 0,0021667
2. Número de cuotas: n = 30 × 12 = 360
3. (1 + i)^−360 = aproximadamente 0,4588
4. 1 − 0,4588 = 0,5412
5. Cuota = 200.000 × 0,0021667 / 0,5412 = aproximadamente 800,68 euros al mes

En todo el préstamo:

- Total pagado: 360 × 800,68 = aproximadamente 288.245 euros
- Intereses totales: aproximadamente 88.245 euros

## Adónde va cada cuota

Cada mes el banco cobra intereses sobre lo que aún debes. El resto de la cuota reduce la deuda (amortización de capital).

1. Intereses = capital pendiente × i
2. Capital amortizado = cuota − intereses
3. Nuevo capital pendiente = capital pendiente anterior − capital amortizado

Mes 1 del ejemplo:

- Intereses: 200.000 × 0,0021667 = 433,33 euros
- Capital amortizado: 800,68 − 433,33 = aproximadamente 367,35 euros
- Nuevo capital pendiente: aproximadamente 199.632,65 euros

Como el capital pendiente baja, los intereses también bajan y cada cuota posterior destina más a capital. La cuota no cambia.

| Mes | Parte de intereses | Parte de capital |
|---|---|---|
| 1 | aproximadamente 54 % | aproximadamente 46 % |
| Último | menos del 1 % | más del 99 % |

## Qué cambia más la cuota

- **Plazo.** Un plazo más largo baja la cuota pero sube los intereses totales. Con el mismo 2,60 %, 20 años en vez de 30 suben la cuota a unos 1.070 euros y bajan los intereses totales a unos 56.700 euros.
- **Tipo de interés.** En el ejemplo, pasar del 2,60 % al 3,60 % sube la cuota de unos 801 a unos 909 euros, alrededor de un 14 % más.
- **Importe.** La cuota es proporcional al préstamo. Si el préstamo se reduce a la mitad, la cuota también.

## Hipotecas variables y mixtas

La fórmula supone que el tipo no cambia. En una hipoteca variable el tipo es el Euríbor más un diferencial y se actualiza en cada revisión (normalmente cada 12 meses). En cada revisión el banco recalcula la cuota con la misma fórmula, con estos datos:

- C = el capital que aún debes
- i = el nuevo tipo dividido entre 12
- n = los meses que quedan

Una cuota variable es, por tanto, el mismo cálculo repetido con datos nuevos. La cuota que ves hoy solo vale hasta la próxima revisión.

## Lo que la fórmula no incluye

- **TIN y TAE.** La fórmula usa el TIN, el tipo nominal. La TAE también cuenta comisiones y productos vinculados, como los seguros, y por eso suele ser más alta que el TIN.
- **Gastos de compra.** Impuestos, notaría, registro y la entrada se pagan aparte del préstamo y no están en la cuota.
- **Redondeo.** Los bancos redondean cada cuota al céntimo. El cuadro de amortización de tu banco puede diferir unos céntimos de un cálculo a mano.

## Pruébalo

An interactive calculator is on the web page: https://apps.schimpf.es/morgage-calc/es/mortgage-monthly-payment-formula/

## En la app

Hipoteca aplica esta fórmula a tu propia oferta. Introduce el precio, los ahorros, el plazo y el tipo de interés para ver la cuota mensual, el TIN y la TAE, el reparto entre capital e intereses y el dinero que necesitas el primer día. La tabla anual y el gráfico del capital pendiente muestran cómo baja la deuda, y puedes exportar el cuadro de amortización en PDF o CSV. En préstamos variables y mixtos, la app también prueba qué pasa con la cuota si sube el Euríbor.

Los resultados son estimaciones y no sustituyen una oferta de tu banco.
