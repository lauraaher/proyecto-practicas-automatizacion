# Plan y resultados de pruebas — Avance 2

## Casos ejecutados

| Caso | Condición | Resultado esperado | Resultado obtenido | Estado |
|---|---|---|---|---|
| CP-01 / SOL-001 | Datos completos y consistentes | Registro simulado | Posición y requisición completadas; SQLite registró ambas | PROBADO |
| CP-02 / SOL-002 | Campo obligatorio / centro costo faltante | Revisión | Detectado | PROBADO |
| CP-03 / SOL-003 | Tipo de vacante inconsistente | Revisión | Detectado | PROBADO |
| CP-04 / SOL-004 | Salario no numérico | Revisión | Detectado | PROBADO |
| CP-05 / SOL-005 | Datos completos | Válido | Clasificado válido | PROBADO EN VALIDACIÓN |
| CP-06 / SOL-006 | Ubicación faltante | Revisión | Detectado | PROBADO |
| CP-07 / SOL-003 | Caso inválido seleccionado como demo | No abrir simulador | `REGISTRO SIMULADO OMITIDO` | PROBADO |

## Evidencias finales

### Corrida positiva
- Caso de demostración: `SOL-001`.
- 6 solicitudes y 6 registros Vacantes VP cargados.
- 36 registros históricos en `ejecuciones`.
- 24 registros históricos en `errores_validacion`.
- 1 posición simulada registrada.
- 1 requisición simulada registrada.
- Ejecución finalizada sin error en `00:02:15`.

### Corrida negativa
- Caso de demostración temporal: `SOL-003`.
- Estado: `REQUIERE REVISION`.
- Resultado: `REGISTRO SIMULADO OMITIDO | SOL-003 | El caso no cumple las validaciones.`
- La corrida finalizó en `00:00:20`.

Los tiempos anteriores son evidencias de ejecución del prototipo y no se presentan todavía como comparación final de eficiencia frente al proceso manual.

## Pendientes
- Solicitud inexistente en Vacantes VP.
- Reemplazo sin información adicional requerida una vez se confirme la regla.
- Ampliación de casos límite durante el resto de semanas 7–9.
