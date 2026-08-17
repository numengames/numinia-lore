# numinia-lore — the seminal corpus

**Public repository, all rights reserved — © 2026 Numen Games S.L.**

Making this content publicly readable grants no license. Every text in
`seminal/` and `seminal-legacy/` carries the express reservation
`LicenseRef-Numen-AllRightsReserved` (see `LICENSES/` and `REUSE.toml`) so
that the absence of an open license can never be mistaken for an oversight
(canon C-005 §1: silence does not declare). Public visibility was decided by
the Oracle on 2026-08-17 (decision D1 of the Codex Reader mission,
`numengames/numinia-nwos` MIS-085); it replaces the deferred-opening plan
recorded as DEBT-002 in `numinia-web/LEGAL_DEBT.md` — *readable* is not
*licensed*, and an open license for the lore remains a separate, future
Oracle act.

Extracted from `numinia-web` on 2026-08-16 by Oracle order (ADR-020 there):
lore does not belong in the code repository. Provenance preserved — both
lineages travel with their git history.

## Contents

- `seminal/` — the founding documents of the rebuild era. The RPG manual
  **`Numinia_Manual_del_juego_de_rol_v0_6_0.md` is the canonical text**
  (v0.6.0, entered 2026-08-17), source of the domain model and payload of
  the Codex reader. `Numinia__El_juego_de_rol__manual_completo_.md` is the
  previous version, kept as diff basis until the consumers migrate.
- `seminal-legacy/` — the pre-rebuild corpus (`docs/seminal-documents/` in
  the legacy lineage, razed 2026-08-15): same texts in earlier form plus
  `Platform Role System.md` and the manual as `.txt`. Kept for the record;
  `seminal/` is canonical.

## Consumers

- `numinia-web` fetches the manual at build time (`npm run lore:fetch`) for
  the Codex reader (`numinia.com/lap/codex/`). CI builds use a synthetic
  fixture instead — this content never re-enters that repository's git tree.
- `numinia-nwos` keeps an older copy of the manual in `canon/` under the
  same reservation; this repository is the canonical home of the current
  text.

## Trademark

Numinia and Numen Games names and marks are addressed separately; see
`TRADEMARKS.md` in `numengames/numinia-nwos`.
