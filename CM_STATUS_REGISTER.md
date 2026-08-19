# CM_STATUS_REGISTER.md — Registro de Estados de Configuración

Repositorio: https://github.com/Elmodtic/GCS_Semana5_A4_MoyanoDario
Última actualización: ISSUE-21 (auditoría de versionado), rama `fix/issue-21-audit-versionado`.

| EC-ID | Elemento de Configuración | Tipo | Versión/Ref | Estado | Responsable | Evidencia (link/captura) |
|------:|---------------------------|------|-------------|--------|------------|---------------------------|
| EC-01 | docs/SRS/SRS_v1.md | Doc | v1.0.0 (commit c1868fe) | Baselined | Analista | Tag `v1.0.0` + commit `c1868fe` |
| EC-02 | src/app.py | Code | commit c1868fe | Integrado | Dev | Commit `c1868fe` (baseline) |
| EC-03 | tests/test_app.py | Test | commit c1868fe | Verificado | QA | `tests/test_app.py::test_add_and_list` (pasa localmente) |
| EC-04 | CHANGELOG.md | Doc | v1.1.0 | Aprobado | PM | Commit de esta rama + tag `v1.1.0` tras merge de PR (ISSUE-21) |
| EC-05 | .gitignore | Config | commit b6ea420 | Aprobado | DevOps | Commit `b6ea420` "chore: remove secrets from repo, add env example (ISSUE-21)" |
| EC-06 | config/.env.example | Config | commit b6ea420 | Integrado | DevOps | Commit `b6ea420`, PR de ISSUE-21 |
| EC-07 | .github/pull_request_template.md | Process | rama fix/issue-21-audit-versionado | Aprobado | Líder | Commit en PR de ISSUE-21 (ver Pull Request vinculado) |
| EC-08 | README.md | Doc | v1.0.0 (commit c1868fe) | Baselined | Equipo | Tag `v1.0.0` + release inicial |

## Notas de auditoría
- **EC-09 (informativo, no forma parte del mínimo de 8):** `config/.env` — Tipo: Config — Estado: **Retirado** (removido del tracking en el commit `b6ea420`, ISSUE-21) — Evidencia: `git log --diff-filter=D -- config/.env`.
- Estados sugeridos utilizados en esta tabla: Registrado · En revisión · Aprobado · Baselined · En implementación · Integrado · Verificado · Liberado · Retirado.
- El estado **Liberado** se reserva para EC ya publicados en un tag/release firmado y comunicado formalmente (aplica a EC-01, EC-02, EC-03 y EC-08 en cuanto se publique el Release `v1.0.0` en GitHub; ver sección Releases del repositorio).
