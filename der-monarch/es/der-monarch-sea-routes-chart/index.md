# Der Monarch rutas marítimas con coste, regreso y ganancia

> Las 10 rutas marítimas de Der Monarch con coste, años, probabilidad de regreso y botín, y la ganancia media de cada viaje.

- Web: https://apps.schimpf.es/der-monarch/es/der-monarch-sea-routes-chart/
- App: Der Monarch, https://apps.schimpf.es/der-monarch/es/index.md
En Der Monarch, los barcos sirven para convertir táleros en más táleros, grano o colonos. También pueden perderse. Esta tabla muestra las diez rutas marítimas y cuáles rinden más de media.

## Cómo funcionan los barcos

- Cada año el juego ofrece 3 de las 10 rutas, elegidas al azar.
- Puedes enviar un barco por ruta y año. El barco cuesta al instante el precio de la ruta.
- Un barco vuelve a los 1 a 4 años, según la ruta. Aparece en tu informe anual.
- Al llegar, regresa con la probabilidad de regreso de la ruta. Si no lo hace, el barco y su carga se pierden. El precio pagado se pierde en ambos casos.
- El botín se sortea de forma uniforme entre el mínimo y el máximo de la ruta.

## La tabla

| Ruta | Coste | Años | Probabilidad de regreso | Oro | Grano (fanegas) | Colonos |
|---|---|---|---|---|---|---|
| Nordsee (mar del Norte) | 600 | 1 | 95 % | ninguno | 1.200–1.950 | ninguno |
| Ostsee (Báltico) | 800 | 1 | 90 % | 200–400 | 1.100–2.100 | ninguno |
| Archangelsk (Arcángel) | 1.000 | 1 | 80 % | 800–1.200 | 800–1.400 | ninguno |
| Mittelmeer (Mediterráneo) | 1.200 | 1 | 85 % | 1.400–2.100 | ninguno | ninguno |
| Grönland (Groenlandia) | 1.200 | 2 | 60 % | 2.000–3.000 | ninguno | ninguno |
| Levante | 1.500 | 2 | 75 % | 2.000–3.000 | ninguno | ninguno |
| Neue Welt (Nuevo Mundo) | 2.000 | 2 | 70 % | 2.200–3.200 | 0–2.000 | 20–60 |
| Kapland (El Cabo) | 2.500 | 3 | 60 % | 4.000–5.300 | ninguno | 30–80 |
| Ostindien (Indias Orientales) | 3.500 | 3 | 50 % | 7.000–10.500 | ninguno | ninguno |
| China | 5.000 | 4 | 40 % | 12.500–18.750 | ninguno | ninguno |

## Valor esperado

La app valora un viaje por su valor medio, contando la probabilidad de perder el barco. Una fanega de grano vale 0,5 táleros y un colono, 10 táleros.

**valor esperado = probabilidad de regreso × (oro medio + grano medio × 0,5 + colonos medios × 10)**

### Ejemplo: Neue Welt

1. Oro medio: (2.200 + 3.200) / 2 = 2.700
2. Grano medio: (0 + 2.000) / 2 = 1.000, que vale 1.000 × 0,5 = 500
3. Colonos medios: (20 + 60) / 2 = 40, que valen 40 × 10 = 400
4. Suma: 2.700 + 500 + 400 = 3.600
5. Por la probabilidad de regreso del 70 %: 2.520 táleros
6. Menos el coste de 2.000 táleros: +520 táleros de media

## Ganancia media por ruta

La ganancia es el valor esperado menos el coste. La última columna la divide entre los años en el mar.

| Ruta | Valor esperado | Ganancia media | Ganancia por año en el mar |
|---|---|---|---|
| Nordsee | 748 | +148 | +148 |
| Ostsee | 990 | +190 | +190 |
| Archangelsk | 1.240 | +240 | +240 |
| Mittelmeer | 1.488 | +288 | +288 |
| Grönland | 1.500 | +300 | +150 |
| Levante | 1.875 | +375 | +188 |
| Neue Welt | 2.520 | +520 | +260 |
| Kapland | 3.120 | +620 | +207 |
| Ostindien | 4.375 | +875 | +292 |
| China | 6.250 | +1.250 | +313 |

Los valores están redondeados. La columna «por año» es una regla orientativa que no tiene en cuenta que el coste queda inmovilizado mientras el barco está fuera.

## Qué significan las cifras

- Todas las rutas tienen una ganancia media positiva, así que de media un barco compensa. Un solo viaje aún puede perderlo todo.
- Las rutas largas rinden más por viaje, pero también arriesgan más. China pierde el barco seis de cada diez veces.
- Las rutas cortas con alta probabilidad de regreso van bien con una caja pequeña. Nordsee vuelve el 95 % de las veces.
- Las rutas de grano ayudan en un año de mala cosecha. Nordsee y Ostsee traen sobre todo grano. Mira la [guía de cosecha y alimentación](der-monarch-feeding-and-harvest-guide).
- Neue Welt y Kapland traen colonos, que suman a tus habitantes para el siguiente rango. Mira los [requisitos de rango](der-monarch-rank-requirements).
- Solo se ofrecen 3 rutas al año, así que eliges la mejor de las que te tocan.

## Calendario

Un barco enviado en el año A por una ruta de 1 año se salda al final del año A y aparece en tu informe del año A+1. Una ruta de 3 años enviada en 1725 aparece en el informe de 1728. La partida termina después de 1760, así que los barcos que aún estén en el mar entonces no traen nada.

## Pruébalo

Der Monarch es un juego de Android para uno a cuatro jugadores en un mismo dispositivo. Todo el texto del juego está en alemán. Abre la app y prueba la pantalla Expeditionen (expediciones) el próximo año.
