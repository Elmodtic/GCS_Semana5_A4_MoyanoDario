# Plan de Gestión de Configuración (CM) — mínimo

## Elementos de Configuración (EC) bajo control
- Documentación (SRS, README, CHANGELOG)
- Código fuente (src/)
- Pruebas (tests/)
- Configuración (config/)
- Procesos (.github/)

## Reglas de control de cambios
1. Todo cambio a un EC debe referenciar un ISSUE-xx.
2. Todo cambio se integra mediante Pull Request (no push directo a main para features).
3. El estado de cada EC se registra en `CM_STATUS_REGISTER.md`.
4. El versionado del producto sigue SemVer (vMAJOR.MINOR.PATCH) y se documenta en `CHANGELOG.md`.

## Estados posibles de un EC
Registrado · En revisión · Aprobado · Baselined · En implementación · Integrado · Verificado · Liberado · Retirado.
