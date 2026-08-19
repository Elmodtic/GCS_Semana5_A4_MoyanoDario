# Changelog

Formato basado en [Keep a Changelog](https://keepachangelog.com/) y [SemVer](https://semver.org/).

## [Unreleased]
- (pendiente) REQ-003 (filtro de productos por fecha): permanece **En revisión**, sin criterios de aceptación definidos. No forma parte del alcance liberado hasta que se documente formalmente.

## [v1.1.0] - 2026
### Seguridad / Gobernanza (ISSUE-21)
- **Corregido**: se removió `config/.env` del control de versiones (contenía una credencial de ejemplo). Se agregó `config/.env.example` como plantilla segura.
- **Agregado**: `.gitignore` para evitar que vuelvan a versionarse archivos de configuración sensibles.
- **Agregado**: plantilla de Pull Request (`.github/pull_request_template.md`) que exige referencia a ISSUE-xx y checklist de evidencia.
- **Agregado**: `docs/CM/CM_PLAN.md` con las reglas de control de cambios del proyecto.
- **Completado**: `CM_STATUS_REGISTER.md` con el registro de estados de los 8 elementos de configuración (EC) del proyecto.
- **Documentado**: auditoría de versionado (tags `v1.0` y `release-1.1` no cumplían SemVer) — ver ISSUE-21.

## [v1.0.1] - 2026
### Corregido
- `fix: hotfix pagos 1%` — corrección menor sobre el procesamiento de pagos simulado.
### Hallazgo de auditoría
- Este commit no referenciaba ningún ISSUE al momento de su creación. Documentado como hallazgo en ISSUE-21; a partir de esta versión todo commit debe referenciar un ISSUE-xx (ver `README.md`, sección Convención).
- El historial de esta versión incluye el commit `feat: add filter date (no docs)` (REQ-003), pero esa funcionalidad **no** se considera parte del alcance oficialmente liberado (ver sección [Unreleased]).

## [v1.0.0] - 2026
- Baseline: estructura del repositorio + SRS v1 (REQ-001, REQ-002, RNF-001, RNF-002) + código mínimo (`src/app.py`) + prueba mínima (`tests/test_app.py`).

## Hallazgos históricos (no remediables sin reescribir historial)
- Commit `ab20032` ("update stuff", 2026): mensaje no descriptivo y versionó `config/.env` con una credencial de ejemplo. Se decidió **no reescribir el historial** (no hacer `git commit --amend` / force-push) para conservar evidencia auditable del hallazgo. La remediación real se aplicó hacia adelante en la v1.1.0 (ISSUE-21).
