# macOS phrase dictionary

This optional Rime table adds Taiwan Traditional Chinese phrase rankings to the existing Dayi2 schema. It does not change the Windows root dictionaries.

## Install

1. Copy [`wiki_phrase_weights.dict.yaml`](wiki_phrase_weights.dict.yaml) into `~/Library/Rime/` as `wiki_phrase_weights.dict.yaml`.
2. In `~/Library/Rime/dayi2.dict.yaml`, add `- wiki_phrase_weights` under `import_tables`, keeping existing imports.
3. Redeploy Squirrel.

This is a supplementary table; do not replace your existing `dayi2.dict.yaml` with it.

## Evaluation

The table was evaluated with Squirrel's bundled librime 1.17.0 and the repository's public Dayi2 schema/dictionaries, in a fresh isolated user-data directory with no userdb. The measure is exact first-candidate match for a segmented 2–4 Han-character word.

- Main holdout: 35,903/37,247 (**96.39%**), compared with 33,158/37,247 (89.02%) before the phrase table.
- Extra holdout: 638/648 (**98.46%**), compared with 623/648 (96.14%) before the phrase table.
- Both sets had 100% supported-code coverage. See [`phrase_level_evaluation.json`](phrase_level_evaluation.json) for counts and reproducibility notes.

Sources and attribution: [`SOURCES.md`](SOURCES.md).
