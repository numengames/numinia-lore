# numinia-lore — the seminal corpus

Private repository. **All rights reserved — Numen Games S.L.** No license is
granted by making this content available to collaborators.

Extracted from `numinia-web` on 2026-08-16 by Oracle order (ADR-020 there):
lore does not belong in the code repository. Provenance preserved — both
lineages travel with their git history.

## Contents

- `seminal/` — the seven founding documents of the rebuild era, including the
  unpublished RPG manual (`Numinia__El_juego_de_rol__manual_completo_.md`),
  canonical source of the domain model.
- `seminal-legacy/` — the pre-rebuild corpus (`docs/seminal-documents/` in the
  legacy lineage, razed 2026-08-15): same texts in earlier form plus
  `Platform Role System.md` and the manual as `.txt`. Kept for the record;
  `seminal/` is canonical.

## Consumers

- `numinia-web` fetches the manual at build time (`npm run lore:fetch`) for
  the Codex reader (`/lap/codex/`, session-gated). CI builds use a synthetic
  fixture instead — this content never re-enters that repository's git tree.

## Future opening (DEBT-002 in numinia-web/LEGAL_DEBT.md)

Opening the lore is deferred, not discarded. Conditions: updated manual +
third-party rights review (Jung, Eco, Blavatsky and Steiner citations must be
verified as quotations, not long reproductions) + signed amendment of D-03.
Likely license then: CC BY-SA 4.0 — adoption with reciprocity.
