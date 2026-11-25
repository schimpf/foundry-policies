# Calculadora de pulsos binaurales: frecuencia y fórmula

> Calcula el tono izquierdo y derecho de cualquier pulso binaural con fórmula, ejemplo y calculadora. Incluye cómo cambia el pulso con el tiempo.

- Web: https://apps.schimpf.es/binaural-beats/es/binaural-beat-frequency-calculator/
- App: Binaural Beats, https://apps.schimpf.es/binaural-beats/es/index.md
Un pulso binaural se forma con dos tonos puros, uno por oído. El pulso que percibes es la diferencia entre ambos. Esta página da la fórmula, un ejemplo resuelto y una calculadora, y después explica cómo deslizar un pulso de una frecuencia a otra.

## La fórmula del pulso binaural

- Tono izquierdo = frecuencia portadora
- Tono derecho = frecuencia portadora + frecuencia del pulso
- Frecuencia del pulso = tono derecho − tono izquierdo

Todos los valores están en hercios (Hz). La portadora es el tono base que oyes de verdad. El pulso es el latido lento que percibes por la diferencia.

Así funciona la app Binaural Beats: a la izquierda va la portadora y a la derecha la portadora más el pulso.

## Ejemplo resuelto

Quieres un pulso de 10 Hz sobre una portadora de 400 Hz.

1. Oído izquierdo: 400 Hz.
2. Oído derecho: 400 + 10 = 410 Hz.
3. Comprobación: 410 − 400 = 10 Hz, así que percibes 10 pulsos por segundo.

A 10 Hz el pulso cae en la banda alfa (de 8 a menos de 12 Hz). El ajuste predefinido de la app, Concentración tranquila, usa justo estos números.

Otro ejemplo: un pulso de 4 Hz sobre una portadora de 250 Hz da 250 Hz a la izquierda y 254 Hz a la derecha. 4 Hz es theta (de 4 a menos de 8 Hz).

## Calculadora

An interactive calculator is on the web page: https://apps.schimpf.es/binaural-beats/es/binaural-beat-frequency-calculator/

## Elegir los números

### Frecuencia portadora

Los pulsos binaurales suelen hacerse con portadoras por debajo de unos 1000 Hz. La app admite de 100 a 1000 Hz y sugiere de 200 a 500 Hz como rango cómodo. Las portadoras graves suenan más profundas y las agudas más brillantes. La portadora fija el tono que oyes y deja intacta la frecuencia del pulso.

### Frecuencia del pulso

La app admite de 0,25 a 45 Hz. Por encima de unos 30 Hz los pulsos binaurales cuesta percibirlos, así que con valores mayores la app sugiere un pulso monoaural o isocrónico.

| Pulso (Hz) | Banda |
|---|---|
| menos de 4 | Delta |
| de 4 a menos de 8 | Theta |
| de 8 a menos de 12 | Alfa |
| de 12 a menos de 30 | Beta |
| 30 o más | Gamma |

### Auriculares

Un pulso binaural solo existe si cada oído oye su propio tono. Usa auriculares estéreo o de botón. Con altavoces los dos tonos se mezclan en el aire y oyes un pulso monoaural. Es otro efecto, pero también un pulso real.

## Otros tipos de pulso, la misma frecuencia

La frecuencia del pulso significa lo mismo en los cuatro modos:

- **Monoaural:** los dos tonos, la portadora y la portadora más el pulso, se suman y suenan en ambos oídos. El pulso está en el propio sonido.
- **Isocrónico:** un tono a la frecuencia de la portadora, que se enciende y se apaga al ritmo del pulso.
- **Bilateral:** un tono a la frecuencia de la portadora que cambia de oído una vez por ciclo del pulso.

En los pulsos isocrónicos y bilaterales la forma del pulso puede ser una senoidal suave o una cuadrada suave con bordes más marcados.

## Deslizar un pulso en el tiempo

Una sesión con varios pasos puede cambiar el pulso poco a poco. La app desliza la frecuencia en escala geométrica: cada tramo de tiempo igual multiplica la frecuencia por el mismo factor.

Fórmula: pulso en el instante t = inicio × (final ÷ inicio)^t, donde t va de 0 a 1 a lo largo del paso.

Ejemplo resuelto: un paso desliza de 12 Hz a 6 Hz.

1. A mitad del paso, t = 0,5.
2. La razón final ÷ inicio = 6 ÷ 12 = 0,5.
3. 0,5 elevado a 0,5 es aproximadamente 0,707.
4. Pulso = 12 × 0,707 ≈ 8,49 Hz.

Un deslizamiento lineal daría 9 Hz a mitad del paso. La versión geométrica dedica el mismo tiempo a cada duplicación o reducción a la mitad, así que pasar de 12 a 6 Hz dura lo mismo que pasar de 6 a 3 Hz. Por eso el control del pulso en la app también es logarítmico.

Si los dos extremos de un paso son iguales, el pulso se mantiene. Después del último paso, los valores finales se mantienen hasta que termina la sesión.

## Qué dice la investigación

La evidencia de que los pulsos binaurales cambian el ánimo, la concentración o el sueño es mixta. El metaanálisis de 2019 de Garcia-Argibay, Santed y Reales («Efficacy of binaural auditory beats in cognition, anxiety, and pain perception: a meta-analysis», Psychological Research) encontró efectos de pequeños a moderados, con grandes diferencias entre estudios. Trata los pulsos como una ayuda para relajarte. Mantén el volumen bajo y no escuches mientras conduces. Consulta antes con tu médico si tienes epilepsia, marcapasos u otra enfermedad.

## Pruébalo en la app

Binaural Beats para Android genera estos tonos en tiempo real, así que puedes probar cualquier portadora y pulso de los ejemplos anteriores.

1. Elige el modo binaural, ajusta la portadora y el pulso y lee la indicación de la banda.
2. Añade, si quieres, ruido blanco, rosa o marrón con su propio volumen.
3. Empieza una sesión de 5 a 90 minutos, o crea una sesión con pasos y mira el pulso en un gráfico.

La app suena en segundo plano, con controles en la pantalla de bloqueo, y funciona sin conexión. También puedes guardar una sesión como archivo WAV.
