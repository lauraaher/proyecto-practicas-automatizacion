# Requerimientos, reglas y criterios de aceptación

## Requerimientos funcionales

- **RF-01:** Leer solicitudes desde el archivo fuente simulado.
- **RF-02:** Leer `Vacantes_VP`.
- **RF-03:** Relacionar registros mediante `Solicitud_ID`.
- **RF-04:** Validar campos obligatorios priorizados.
- **RF-05:** Comparar información entre fuentes.
- **RF-06:** Validar formato salarial.
- **RF-07:** Clasificar el caso como válido o requiere revisión.
- **RF-08:** Registrar estado y motivo.
- **RF-09:** Impedir que un caso inválido continúe al registro simulado.
- **RF-10:** Diligenciar una posición simulada.
- **RF-11:** Diligenciar una requisición simulada.
- **RF-12:** Persistir trazabilidad de validaciones y resultados simulados.
- **RF-13:** Mantener aprobaciones finales como actividades humanas.

## Requerimientos no funcionales

- **RNF-01:** No usar credenciales reales.
- **RNF-02:** Usar datos sintéticos o anonimizados.
- **RNF-03:** Poder demostrar el prototipo sin acceso productivo a SuccessFactors.
- **RNF-04:** Mantener trazabilidad persistente.
- **RNF-05:** Poder reproducir la demostración en entorno local.

## Reglas implementadas

| ID | Regla | Estado |
|---|---|---|
| RV-01 | Solicitud_ID no vacío | Implementada |
| RV-02 | Campos obligatorios priorizados no vacíos | Implementada |
| RV-03 | Tipo de vacante consistente entre fuentes | Implementada |
| RV-04 | Centro de costo consistente entre fuentes | Implementada |
| RV-05 | Salario con formato numérico | Implementada |
| RV-08 | Aprobaciones fuera de automatización | Aplicada por diseño |
| RV-09 | Datos/credenciales sensibles no utilizados | Aplicada por diseño |

## Criterios de aceptación y estado

| Criterio | Estado |
|---|---|
| CA-01 Carga de ambas fuentes | CUMPLIDO |
| CA-02 Cada solicitud recibe estado | CUMPLIDO |
| CA-03 Inconsistencias del dataset detectadas | CUMPLIDO EN DATASET CONTROLADO |
| CA-04 Caso inválido no continúa | CUMPLIDO |
| CA-05 Caso válido diligencia Posición/Requisición | CUMPLIDO |
| CA-06 Trazabilidad persistente | CUMPLIDO |
| CA-07 Aprobación final humana | CUMPLIDO |
| CA-08 Demostración sin acceso productivo | CUMPLIDO |

## Pendientes

- Existencia de posición como regla explícita.
- Reglas específicas de reemplazo.
- Validaciones salariales que requieran decisión humana.
- Catálogos/fuentes reales para campos no disponibles en los formatos actuales.
