# Sundara-commentaries

_Created: 16-09-2026 · Last updated: 20-09-2026_

> **AI/data stance:** n/a: data-only, not a drain pick (H5173, 20-09-2026).

Canonical home for the Sundarakāṇḍa commentary apparatus — the sarga-level reviewer
manifests, gate ledger, commentary-to-add layers, and typed-link concordance that
previously lived under [`CommentaryStrategies/data/`](https://github.com/gasyoun/CommentaryStrategies).

Rehomed per [H4849](https://github.com/gasyoun/Uprava/blob/main/handoffs/archive/H4849-OxAlpha_Sundara-commentaries_sundara-apparatus-rehome-move_14.09.26.md)
(MG ruling 14-09-2026, census B4: "razlozhit soderzhimoe po korobkam" — move the data,
keep the scaffold). Every file below moved byte-identical (sha256 parity verified,
428/428 files) from `CommentaryStrategies/data/`.

## Contents

- `data/sundara_ch*_commentary_to_add.json` (68 files, ch1–ch68) — per-chapter commentary layer
- `data/sundara_commentary_to_add.json` — merged commentary layer
- `data/leonov_sundara_ch1_candidates.json` — Leonov ch1 candidate notes
- `data/sundara1_pilot_c3_20.json` — pilot c3/20 sample
- `data/sundara_book_stats.json` — book-level stats
- `data/typed_link_sundara_concordance.*` (README/jsonl/tsv/confirmed variants) — typed-link concordance
- `data/apparatus/` — sarga reviewer manifests, HTML review portal, `gate_ledger.json`, `gate_disagreements.*`, `adjudication_policy.json`
- `data/valmiki_shlokas/kanda_5_sundarakanda/` — per-sarga Sundarakāṇḍa śloka text

## Consumer

[`CommentaryStrategies`](https://github.com/gasyoun/CommentaryStrategies) still reads
this apparatus family — ~70 scripts under `scripts/` and `tests/` have hard build
dependencies on the original `data/` paths. Per H4849's own escape clause ("only if a
hard build dependency blocks, vendored read-only copy marked vendored"), the original
files stay in `CommentaryStrategies/data/` as a **vendored read-only copy** — this repo
is the source of truth; `CommentaryStrategies/data/SUNDARA_APPARATUS_VENDORED.md` marks
that copy and points back here. Edge registered in
[Uprava interlinks_edges.tsv](https://github.com/gasyoun/Uprava/blob/main/interlinks_edges.tsv).
