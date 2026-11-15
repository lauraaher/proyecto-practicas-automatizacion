# Diseño de la solución — Avance 2

## Estado al 14 de noviembre de 2026

El prototipo vigente contempla:

- Excel `Solicitudes_Vacantes` como fuente principal simulada.
- Excel `Vacantes_VP` como fuente de control simulada.
- UiPath para lectura, estructuración, validación, control de flujo y automatización.
- Reglas implementadas para campos obligatorios, tipo de vacante, centro de costo y formato salarial.
- Clasificación `VALIDO PARA REGISTRO SIMULADO` / `REQUIERE REVISION`.
- Salida `ResultadosValidacion.xlsx`.
- Persistencia SQLite de ejecuciones y errores de validación.
- Simulador académico local para Posición y Requisición basado en las interfaces observadas del proceso real.
- Control previo al simulador: un caso inválido no continúa.
- Persistencia SQLite del resultado simulado de Posición y Requisición.
- Aprobaciones humanas fuera de la automatización.

## Alcance

La solución no es una integración productiva con SuccessFactors. El prototipo demuestra lectura, validación, preparación y transferencia de información a una interfaz simulada, utilizando datos sintéticos y sin credenciales corporativas.

## Estado de componentes

| Componente | Estado |
|---|---|
| AS-IS | Actualizado |
| TO-BE | Actualizado |
| Arquitectura | Actualizada |
| Mapeo de campos v2 | Formalizado |
| Reglas de validación | Parcialmente implementadas y documentadas |
| Criterios de aceptación | Formalizados y probados en alcance actual |
| Plan de pruebas | Formalizado |
| UiPath lectura/validación | PROBADO |
| Salida Excel | PROBADO |
| SQLite ejecuciones/errores | PROBADO |
| Simulación Posición | PROBADO |
| Simulación Requisición | PROBADO |
| Bloqueo de casos inválidos | PROBADO |
| SQLite resultado web | PROBADO |
