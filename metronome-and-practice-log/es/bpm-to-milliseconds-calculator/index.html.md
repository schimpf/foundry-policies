# Calculadora de BPM a milisegundos y fórmula

> Convierte BPM a milisegundos por pulso con una fórmula, ejemplos resueltos y una tabla con la duración de las figuras, de redonda a semicorchea.

- Web: https://apps.schimpf.es/metronome-and-practice-log/es/bpm-to-milliseconds-calculator/
- App: Metrónomo y Diario de Práctica, https://apps.schimpf.es/metronome-and-practice-log/es/index.md
Los tiempos de delay, las pistas de clic (click tracks) y los efectos sincronizados con el tempo piden a menudo milisegundos, mientras que la música se escribe en pulsos por minuto (BPM). La conversión es una sola división.

## La fórmula

Un minuto tiene 60 000 milisegundos. Divídelos entre el número de pulsos que caben en ese minuto:

**milisegundos por pulso = 60 000 / BPM**

Y en sentido contrario:

**BPM = 60 000 / milisegundos por pulso**

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/metronome-and-practice-log/es/bpm-to-milliseconds-calculator/

## Ejemplo resuelto

Practicas a 90 BPM y quieres saber el tiempo entre clics.

1. Escribe la fórmula: 60 000 / 90.
2. Divide: 666,67.
3. El intervalo entre pulsos es de unos 667 ms.

Compruébalo: 90 pulsos de 666,67 ms suman 60 000 ms, que es un minuto.

## Tempos habituales

| BPM | ms por pulso |
|---|---|
| 40 | 1500 |
| 60 | 1000 |
| 72 | 833,3 |
| 80 | 750 |
| 100 | 600 |
| 120 | 500 |
| 144 | 416,7 |
| 180 | 333,3 |
| 240 | 250 |
| 300 | 200 |

```
 60 BPM |##########  1000 ms
120 BPM |#####       500 ms
240 BPM |###         250 ms
```

Al duplicar los BPM, el intervalo se reduce a la mitad.

## Duración de las figuras a un tempo dado

El número de BPM cuenta un tipo de pulso, normalmente la negra. Las demás figuras son fracciones de ella. A 100 BPM, con la negra como pulso (600 ms):

| Figura | Parte de una negra | Duración a 100 BPM |
|---|---|---|
| Redonda | 4 | 2400 ms |
| Blanca | 2 | 1200 ms |
| Negra | 1 | 600 ms |
| Corchea | 1/2 | 300 ms |
| Tresillo de corchea | 1/3 | 200 ms |
| Semicorchea | 1/4 | 150 ms |

Para obtener cualquiera de ellas, calcula la negra con la fórmula y multiplica por la fracción. Una figura con puntillo dura 1,5 veces su valor simple. Una negra con puntillo a 100 BPM dura 600 x 1,5 = 900 ms.

## Qué cuenta como pulso

Ten cuidado cuando el pulso no es una negra. En un compás de 6/8, la partitura puede marcar la negra con puntillo como pulso, lo que da dos pulsos por compás. Si un metrónomo hace clic en cada corchea, los BPM que ajustas son las corcheas por minuto, es decir, el triple del tempo de la negra con puntillo. Una negra con puntillo a 60 BPM equivale a corcheas a 180 BPM.

Metrónomo y Diario de Práctica usa la misma regla: los BPM que ajustas son los clics por minuto, y cada tiempo del compás recibe un clic. En 6/8 eso son seis clics por compás. Por defecto, la app acentúa el primer y el cuarto clic, así que oyes dos pulsos de negra con puntillo. Puedes cambiar el acento de cada tiempo.

## Por qué importa la precisión del ritmo

A 120 BPM un pulso dura 500 ms. Un error de 10 ms es el 2 por ciento del pulso, y los errores de los temporizadores comunes se acumulan en un compás o dos. Los metrónomos de móvil que los usan pueden desviarse, sobre todo con la pantalla apagada.

La app cuenta muestras de audio en lugar de usar temporizadores. Cada pulso se escribe en la salida de audio con su duración exacta, y la parte decimal de esa duración pasa al pulso siguiente, así que el tempo no se desvía. Por ejemplo, a 48 000 muestras por segundo y 100 BPM, un pulso tiene 28 800 muestras, un número exacto. A 70 BPM son 41 142,857 muestras, y el resto se arrastra para que la media se quede exactamente en 70 BPM. Los cambios de tempo se aplican desde el pulso siguiente.

## Redondeo

- Para efectos de delay, redondea al milisegundo entero. El error es menor que medio milisegundo.
- Para pistas de clic, conserva dos decimales si la herramienta lo permite.
- No redondees los BPM. 666,67 ms corresponden a 90 BPM, mientras que 667 ms dan 89,96 BPM.

## Pruébalo en la app

Metrónomo y Diario de Práctica es un metrónomo para Android que funciona sin conexión y registra cada sesión de práctica automáticamente. Va de 30 a 300 BPM, es decir, de 2000 ms a 200 ms por pulso. Mantiene el ritmo en segundo plano y con la pantalla apagada, y ofrece destello de pantalla y vibración en cada tiempo. Búscalo en Google Play.
