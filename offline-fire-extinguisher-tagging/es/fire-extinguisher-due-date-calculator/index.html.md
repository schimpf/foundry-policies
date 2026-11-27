# Calculadora de fechas de revisión de extintores (NFPA 10)

> Indica el tipo de extintor y sus últimas revisiones para calcular la próxima revisión mensual, anual, de 6 años y la prueba hidrostática.

- Web: https://apps.schimpf.es/offline-fire-extinguisher-tagging/es/fire-extinguisher-due-date-calculator/
- App: Inspección de extintores, https://apps.schimpf.es/offline-fire-extinguisher-tagging/es/index.md
## Calcula las próximas fechas de revisión

Elige el tipo de extintor e introduce las fechas que tengas. Deja un campo vacío si no hay registro. La calculadora usa las mismas reglas que la app y se basa en NFPA 10, Standard for Portable Fire Extinguishers (edición de 2022).

An interactive calculator is on the web page: https://apps.schimpf.es/offline-fire-extinguisher-tagging/es/fire-extinguisher-due-date-calculator/

## Las fórmulas

Cada próxima fecha parte de la última fecha registrada.

| Concepto | Próxima fecha | ¿Usa la fecha de fabricación si falta? |
|---|---|---|
| Mensual | última revisión mensual + 31 días | no |
| Anual | último mantenimiento anual + 12 meses | no |
| Mantenimiento de 6 años | último de 6 años + 6 años | sí |
| Prueba hidrostática | última prueba + 5 o 12 años | sí |

- El mantenimiento de 6 años se aplica a los extintores de polvo químico ABC, de polvo químico BC y de agente limpio. Para los demás tipos, la fila dice "no requerido".
- El intervalo de la prueba hidrostática es de 12 años para ABC, BC, agente limpio y polvo para fuegos de clase D, y de 5 años para CO2, agua, espuma y agente húmedo de clase K.
- Las fechas mensual y anual no tienen alternativa. Si no hay última fecha mensual o anual, el resultado es "sin registrar".

La lista completa por tipo está en la [tabla de intervalos](../fire-extinguisher-maintenance-and-hydrostatic-test-intervals/).

## Cómo se calcula el estado

La calculadora cuenta los días entre hoy y la fecha de vencimiento.

- **Vencido:** quedan menos de 0 días.
- **Próximo a vencer:** de 0 a 7 días en la revisión mensual, de 0 a 30 días en los demás conceptos.
- **Correcto:** más días que eso.

## Ejemplo resuelto

Un extintor de agua se fabricó el 14 de mayo de 2019. La última revisión mensual fue el 1 de noviembre de 2026, el último mantenimiento anual el 20 de diciembre de 2025 y no hay ninguna prueba hidrostática registrada. Hoy es 27 de noviembre de 2026.

1. **Mensual:** 1 de noviembre de 2026 + 31 días = 2 de diciembre de 2026. Faltan 5 días, así que está próximo a vencer (7 días o menos).
2. **Anual:** 20 de diciembre de 2025 + 12 meses = 20 de diciembre de 2026. Faltan 23 días, así que está próximo a vencer (30 días o menos).
3. **6 años:** el agua no lo necesita, así que no es requerido.
4. **Prueba hidrostática:** no hay fecha, así que 14 de mayo de 2019 + 5 años = 14 de mayo de 2024. Ya pasó, por lo que lleva 927 días vencido.

El equipo aparece como vencido, por la prueba hidrostática, porque "vencido" tiene prioridad sobre "próximo a vencer".

## Casos límite

- **Fin de mes:** 31 de agosto + 6 meses da el último día del mes de destino, el 28 de febrero o el 29 en año bisiesto. El 29 de febrero + 1 año da el 28 de febrero.
- **Una inspección con fallo:** en la app, si la última inspección tuvo fallo, el estado del equipo queda por encima de vencido. La calculadora de esta página solo muestra fechas.
- **Normas locales más estrictas:** la autoridad competente puede exigir intervalos más cortos. Usa el más corto. En España rige el Reglamento de instalaciones de protección contra incendios (RIPCI, Real Decreto 513/2017), con sus propios plazos. La app calcula según NFPA 10.

## Para una instalación completa

Escribir fechas en una calculadora sirve para un solo equipo. En una instalación con 40 extintores, Offline fire extinguisher tagging guarda las fechas en el móvil, calcula cada próxima fecha según el tipo con estas fórmulas y muestra primero los equipos vencidos. Escaneas el código QR o de barras de la etiqueta para abrir un equipo. Funciona sin cobertura y sin cuenta. La versión gratuita admite 25 extintores, así que una instalación de 40 necesita Pro.

La [lista de comprobación NFPA 10](../nfpa-10-monthly-annual-inspection-checklist/) explica las revisiones mensual y anual que actualizan estas fechas.
