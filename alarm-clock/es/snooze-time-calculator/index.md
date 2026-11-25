# Calculadora para posponer la alarma: tu hora real

> Calcula cuántos minutos te cuesta posponer la alarma y a qué hora suena por última vez. Incluye calculadora y un ejemplo resuelto.

- Web: https://apps.schimpf.es/alarm-clock/es/snooze-time-calculator/
- App: Despertador con misiones, https://apps.schimpf.es/alarm-clock/es/index.md
Cada vez que pospones la alarma, te levantas más tarde. Esta página muestra la fórmula, un ejemplo resuelto y una calculadora pequeña para que veas lo que te cuesta de verdad posponer.

## La fórmula

El tiempo extra que pierdes sigue esta fórmula:

**Retraso total = intervalo de posposición × número de posposiciones**

La última alarma suena a las:

**Última alarma = hora de la alarma + retraso total**

Estos puntos importan en la práctica:

- El intervalo cuenta desde el momento en que tocas Posponer.
- Si dejas sonar la alarma un rato antes de tocar, el retraso real es algo mayor que el de la fórmula.
- La fórmula da el retraso mínimo. Es exacta cuando tocas Posponer enseguida.

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/alarm-clock/es/snooze-time-calculator/

## Ejemplo resuelto

Programas una alarma a las 6:30 con un intervalo de 5 minutos y tocas Posponer 3 veces.

1. Retraso total = 5 min × 3 = 15 min.
2. Última alarma = 6:30 + 15 min = 6:45.
3. Te levantas a las 6:45 como pronto.

La misma alarma con un intervalo de 10 minutos y 4 posposiciones:

1. Retraso total = 10 min × 4 = 40 min.
2. Última alarma = 6:30 + 40 min = 7:10.

El retraso para algunos ajustes habituales:

| Intervalo | Posposiciones | Retraso total |
| --- | --- | --- |
| 5 min | 1 | 5 min |
| 5 min | 3 | 15 min |
| 9 min | 3 | 27 min |
| 10 min | 4 | 40 min |
| 15 min | 5 | 75 min |
| 30 min | 10 | 300 min (5 h) |

## Lee el resultado como un presupuesto

Si tienes que estar fuera de la cama a las 7:00 y piensas posponer, calcula hacia atrás:

1. Elige tu intervalo y el número de posposiciones que esperas.
2. Multiplícalos para obtener el retraso total.
3. Resta ese retraso a las 7:00 para obtener la hora de la alarma.

Con un intervalo de 5 minutos y 3 posposiciones, el retraso es de 15 minutos, así que la alarma suena a las 6:45. La última alarma cae a las 7:00. Añade un pequeño margen para el tiempo entre alarmas, porque no tocarás Posponer en el segundo exacto en que empieza a sonar.

## Fija un límite con el que puedas vivir

Posponer sin límite no tiene tope, y el retraso total tampoco. Un límite hace que el coste se conozca de antemano. Cuando se alcanza el límite, la alarma deja de ofrecer Posponer y tienes que levantarte.

## Ajustes para posponer en Despertador

Despertador te deja fijar los dos valores en cada alarma:

- **Intervalo:** de 1 a 30 minutos. Por defecto, 5 minutos.
- **Máximo de posposiciones:** de 0 a 10, o ilimitado. Por defecto, 3.
- **0 posposiciones** desactiva posponer en esa alarma.
- Un chip en la pantalla de la alarma muestra cuántas veces has pospuesto.
- Posponer está siempre disponible en la pantalla de la alarma hasta que llegas a tu límite.
- Una vez iniciada una misión para despertar, ya no se puede posponer. Primero terminas la misión.

Con los valores por defecto, lo peor son 5 × 3 = 15 minutos de sueño extra, igual que en el primer ejemplo de arriba.

## Combina posponer con una misión

Si posponer es el hábito que quieres quitarte, pon el máximo en un número pequeño y añade una misión. Despertador ofrece cuatro: problemas de matemáticas, agitar el teléfono, escanear un código QR o de barras y caminar un número de pasos. La misión no se puede saltar. Si fallas tres veces, la app ofrece una operación más fácil para que nunca te quedes atascado.

Despertador suena en el minuto exacto con la API de despertador del sistema, usa el volumen de alarma para sonar también en silencio y no tiene permiso de internet. Es de código abierto bajo la licencia GNU GPL v3 o posterior. La app está en inglés y alemán. Fija el intervalo y el límite de posposiciones en el editor de alarmas.
