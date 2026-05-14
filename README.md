# Modelo BML de tráfico: transiciones de fase y umbrales de congestión

Proyecto académico — Modelado de sistemas complejos · Universidad Nacional de
Colombia (Ago 2023 – Nov 2023)

## El problema

El modelo de Biham-Middleton-Levine (BML) es un autómata celular simple que
representa tráfico vehicular en una grilla con dos sentidos. A pesar de su
simplicidad, presenta una **transición de fase abrupta**: por debajo de cierta
densidad de vehículos el flujo es libre; por encima, el sistema colapsa
súbitamente en gridlock global. La pregunta es **dónde está el umbral** y cómo
caracterizarlo cuantitativamente.

## Qué hice?

- Implementé el modelo BML desde cero en Python sobre grillas configurables.
- Automaticé experimentos numéricos haciendo **barridos sistemáticos de
  densidad** (parámetro de control).
- Generé datasets agregados del comportamiento del sistema (flujo, fracción de
  vehículos bloqueados, tiempo hasta gridlock) bajo múltiples condiciones
  iniciales.
- Caractericé la transición de fase identificando umbrales operativos y
  extrayendo métricas comparativas entre regímenes.

## Lo que aporta

- Pipeline reproducible para experimentación numérica sobre sistemas dinámicos
  discretos.
- Práctica concreta en **detección de transiciones de fase** y caracterización de
  regímenes a partir de simulaciones — técnica transferible al estudio de
  cualquier sistema con comportamiento crítico (mercados, redes eléctricas,
  congestión de cualquier tipo).

## Stack técnico

`Python` · `NumPy` · `Matplotlib` · `Jupyter` · autómatas celulares · análisis
de transiciones de fase
