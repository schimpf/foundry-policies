# Intervalos de revisión y prueba hidrostática de extintores

> Tabla de intervalos NFPA 10 de revisión mensual, mantenimiento anual, de 6 años y prueba hidrostática para extintores ABC, CO2, de agua y espuma.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/es/fire-extinguisher-maintenance-and-hydrostatic-test-intervals/
- App: Inspección de extintores, https://apps.schimpf.es/offline-fire-extinguisher-tagging/es/index.md
## Tabla de intervalos por tipo de extintor

NFPA 10, Standard for Portable Fire Extinguishers (edición de 2022), fija cada cuánto necesita un extintor portátil inspección, mantenimiento y prueba hidrostática. Los intervalos dependen del tipo. La tabla recoge los que usa la app.

| Tipo | Revisión mensual | Mantenimiento anual | Mantenimiento de 6 años | Prueba hidrostática |
|---|---|---|---|---|
| Polvo químico ABC | cada 31 días | 12 meses | sí | cada 12 años |
| Polvo químico BC | cada 31 días | 12 meses | sí | cada 12 años |
| Agente limpio | cada 31 días | 12 meses | sí | cada 12 años |
| Polvo para fuegos de metales (clase D) | cada 31 días | 12 meses | no | cada 12 años |
| CO2 | cada 31 días | 12 meses | no | cada 5 años |
| Agua / agua nebulizada | cada 31 días | 12 meses | no | cada 5 años |
| Espuma (AFFF/FFFP) | cada 31 días | 12 meses | no | cada 5 años |
| Agente húmedo (clase K) | cada 31 días | 12 meses | no | cada 5 años |

Fuentes: NFPA 10 (2022), sección 7.2 para la revisión mensual, sección 7.3 para el mantenimiento anual y de 6 años, y sección 8.3 para la prueba hidrostática. La autoridad competente puede exigir intervalos más cortos. En España rige el Reglamento de instalaciones de protección contra incendios (RIPCI, Real Decreto 513/2017), con sus propios plazos. La app calcula según NFPA 10.

## Qué significa cada intervalo

### Mensual: cada 31 días

Una revisión visual rápida de ubicación, precinto, manómetro, estado y etiqueta. La app cuenta 31 días desde la última fecha mensual.

### Anual: 12 meses

Un mantenimiento más completo, que incluye las piezas mecánicas, el estado del agente extintor, la manguera y la boquilla. La próxima fecha cae 12 meses después de la última fecha anual. La [página de la lista de comprobación](../nfpa-10-monthly-annual-inspection-checklist/) detalla cada punto.

### Mantenimiento de 6 años

Se aplica a los tipos de polvo químico ABC, polvo químico BC y agente limpio de la tabla. El extintor se vacía y se examina por dentro. La próxima fecha cae 6 años después del último mantenimiento de 6 años. Si no hay ninguno registrado, la app cuenta 6 años desde la fecha de fabricación.

### Prueba hidrostática: 5 o 12 años

Se prueba el cilindro a presión para comprobar que aguanta. La próxima fecha cae un intervalo de prueba después de la última prueba hidrostática. Si no hay ninguna registrada, la app cuenta desde la fecha de fabricación.

## Ejemplo resuelto

Un extintor de polvo químico ABC se fabricó el 2 de marzo de 2016. No hay nada más registrado, salvo una revisión mensual del 10 de enero de 2026 y un mantenimiento anual del 15 de junio de 2025.

- **Próxima mensual:** 10 de enero de 2026 más 31 días es el 10 de febrero de 2026.
- **Próxima anual:** 15 de junio de 2025 más 12 meses es el 15 de junio de 2026.
- **Próxima de 6 años:** no hay fecha de 6 años, así que 2 de marzo de 2016 más 6 años es el 2 de marzo de 2022. Esa fecha pasó hace mucho, por lo que el equipo está vencido.
- **Próxima hidrostática:** no hay fecha de prueba, así que 2 de marzo de 2016 más 12 años es el 2 de marzo de 2028.

Ahora un extintor de CO2 fabricado el 20 de agosto de 2021 sin otras fechas. El CO2 no tiene mantenimiento de 6 años, así que esa fila es "no requerido". Su prueba hidrostática es el 20 de agosto de 2021 más 5 años, es decir, el 20 de agosto de 2026.

El cálculo usa meses y años naturales. Si una fecha cae en un día que el mes de destino no tiene, pasa al último día de ese mes, así que 31 de agosto más 6 meses da el 28 de febrero (o el 29 en año bisiesto).

## Cómo marca el estado la app

Para cada fecha de vencimiento, la app compara la fecha con hoy:

- **Vencido:** la fecha ya pasó.
- **Próximo a vencer:** las revisiones mensuales a 7 días o menos, los demás conceptos a 30 días o menos.
- **Correcto:** cualquier fecha posterior.
- **Sin registrar:** no hay fecha desde la que contar.

Un extintor muestra su peor concepto. Una última inspección con fallo queda por encima de vencido, y después van vencido, próximo a vencer y correcto. Un equipo sin nada registrado aparece como nuevo.

## Calcúlalo para un equipo

En la [página de la calculadora](../fire-extinguisher-due-date-calculator/) introduces las fechas de un extintor y ves las cuatro próximas fechas.

## Controlarlo en una instalación completa

Offline fire extinguisher tagging guarda las últimas fechas mensual, anual, de 6 años e hidrostática de cada extintor y calcula las próximas según el tipo, con las reglas de arriba. Cada equipo, instalación y cliente aparece como correcto, próximo a vencer o vencido. Envía un aviso por instalación una vez al día, y el widget de la pantalla de inicio muestra los equipos vencidos, los próximos a vencer y la siguiente instalación que visitar. Solo registra las fechas. No tiene listas de comprobación para el mantenimiento de 6 años ni para la prueba hidrostática.
