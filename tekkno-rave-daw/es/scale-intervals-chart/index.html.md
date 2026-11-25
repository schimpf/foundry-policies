# Escalas y intervalos: menor, frigia, menor armónica

> Intervalos en semitonos de las escalas menor, mayor, frigia, menor armónica y pentatónica menor, con la razón de frecuencia de cada semitono.

- Web: https://apps.schimpf.es/tekkno-rave-daw/es/scale-intervals-chart/
- App: Tekkno Rave DAW: Crea Beats, https://apps.schimpf.es/tekkno-rave-daw/es/index.md
Los leads oscuros de hard techno y los acid stabs suelen moverse en una escala menor o frigia. Esta página lista los intervalos en semitonos de cinco escalas habituales, explica cómo formarlas desde cualquier nota base y da la razón de frecuencia de cada semitono para que veas qué pasa al transponer una muestra.

## Tabla de intervalos de las escalas

Los números son semitonos por encima de la nota base. La nota base es 0 y la octava es 12.

| Escala | Semitonos desde la nota base | Notas |
|--------|------------------------------|-------|
| Menor (menor natural) | 0, 2, 3, 5, 7, 8, 10 | 7 |
| Mayor | 0, 2, 4, 5, 7, 9, 11 | 7 |
| Frigia | 0, 1, 3, 5, 7, 8, 10 | 7 |
| Menor armónica | 0, 2, 3, 5, 7, 8, 11 | 7 |
| Pentatónica menor | 0, 3, 5, 7, 10 | 5 |

Estas fórmulas de intervalos son teoría musical occidental estándar. Para un tratamiento de manual, consulta a Kostka y Payne, *Tonal Harmony* (McGraw-Hill, 8.ª edición, 2017).

## Cómo suena cada escala

- La menor tiene una tercera bemol (3 semitonos), que da el aire oscuro y serio habitual en el techno.
- La frigia es la menor con segunda bemol (1 semitono). Ese paso corto sobre la nota base da el sonido tenso y agresivo de muchos leads de hardcore y gabber.
- La menor armónica es la menor con séptima elevada (11 semitonos). El hueco entre la 6.ª y la 7.ª nota da un impulso dramático de aire oriental.
- La mayor es más brillante y se usa menos en los estilos duros, pero sirve para melodías de hardcore eufórico.
- La pentatónica menor quita la 2.ª y la 6.ª nota. Con solo cinco notas casi nada suena mal, así que va bien para riffs.

## Cómo formar una escala desde cualquier nota base

1. Numera las 12 notas desde la base: Do = 0, Do sostenido = 1, Re = 2, Re sostenido = 3, Mi = 4, Fa = 5, Fa sostenido = 6, Sol = 7, Sol sostenido = 8, La = 9, La sostenido = 10, Si = 11.
2. Suma el número de la nota base a cada intervalo de la tabla.
3. Si el total es 12 o más, réstale 12.
4. Convierte los números otra vez en nombres de nota.

La app muestra las notas con letras (C, D, E, F, G, A, B). Do = C, Re = D, Mi = E, Fa = F, Sol = G, La = A, Si = B.

### Ejemplo: Fa frigio

Fa es 5. La frigia es 0, 1, 3, 5, 7, 8, 10.

- 5 + 0 = 5, Fa
- 5 + 1 = 6, Fa sostenido (Sol bemol)
- 5 + 3 = 8, Sol sostenido (La bemol)
- 5 + 5 = 10, La sostenido (Si bemol)
- 5 + 7 = 12, que es 0, Do
- 5 + 8 = 13, que es 1, Do sostenido (Re bemol)
- 5 + 10 = 15, que es 3, Re sostenido (Mi bemol)

Fa frigio es Fa, Sol bemol, La bemol, Si bemol, Do, Re bemol, Mi bemol.

## Razón de frecuencia de cada semitono

Transponer una muestra por remuestreo cambia su velocidad de reproducción. En el temperamento igual de 12 notas, cada semitono multiplica la frecuencia por la raíz duodécima de 2:

razón = 2^(semitonos / 12)

| Semitonos | Razón |
|-----------|-------|
| 0 | 1,0000 |
| 1 | 1,0595 |
| 2 | 1,1225 |
| 3 | 1,1892 |
| 4 | 1,2599 |
| 5 | 1,3348 |
| 6 | 1,4142 |
| 7 | 1,4983 |
| 8 | 1,5874 |
| 9 | 1,6818 |
| 10 | 1,7818 |
| 11 | 1,8877 |
| 12 | 2,0000 |

Los valores negativos bajan: -12 semitonos dan una razón de 0,5, la mitad de velocidad y una octava más grave. El remuestreo también cambia la duración de la muestra. Una muestra reproducida con razón 2 dura la mitad.

## Ejemplo: una fila de la cuadrícula en La menor

Tekkno Rave DAW asigna un tono a cada fila de la cuadrícula con esta regla. La fila 0 es la más baja y una fila más alta es un tono más alto. Con el ajuste a escala activado, cada fila es el siguiente grado de la escala, así que todas las filas están en la tonalidad. Las muestras están afinadas a Do 3 (C3), que es la nota MIDI 48, y el semitono 0 significa C3.

Para una escala con n notas:

semitonos = base + 12 x cambio de octava + 12 x (fila div n) + intervalo[fila mod n]

Toma La menor (base 9, 7 notas), cambio de octava 0 y fila 9:

1. 9 div 7 = 1, así que el patrón ha subido una octava: 12 x 1 = 12.
2. 9 mod 7 = 2, y el tercer intervalo de la menor (índice 2) es 3.
3. Total = 9 + 0 + 12 + 3 = 24 semitonos.
4. Razón = 2^(24 / 12) = 4,0.
5. La nota es MIDI 48 + 24 = 72, que es C5 (Do 5).

Compruébalo contando los grados de La menor desde la fila 0: La, Si, Do, Re, Mi, Fa, Sol, La, Si, Do. La fila 9 es la décima nota, Do. Coincide.

Con el ajuste desactivado, las filas son semitonos sin más (semitonos = base + 12 x cambio de octava + fila) y las filas dentro de la escala solo se tiñen de color.

## Pruébalo en la app

Tekkno Rave DAW tiene una cuadrícula de patrones con 12 filas, 8, 16, 32 o 64 pasos y un cambio de octava de -2 a +2. Elige menor, mayor, frigia, menor armónica o pentatónica menor con cualquier nota base, activa el ajuste y todas las filas se quedan en la tonalidad. Abre un patrón y pinta notas para oír las escalas de esta tabla.
