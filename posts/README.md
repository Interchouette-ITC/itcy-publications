# Posts layout (org Publications)

**Post** (= Publication) artefacts on **Interchouette-ITC/itcy-publications** live under `posts/<POST-id>/`.

Drafts do **not** live here. Drafts are on the Interchouette fork under `drafts/<DRAFT-id>/`. After **gRoussac Approve** (BAT) on the fork Draft PR, ITCy promotes here.

**License:** Post bodies are (c) Interchouette-ITC, BUSL-1.1 - see [NOTICE](NOTICE) and root [LICENSE](../LICENSE). Do not add SPDX inside `body.md`.

## Path

```text
posts/<POST-id>/
  body.md      # Post body (header: Post ID: POST-YYYYMMDD-NNNNNN)
  meta.toml    # kind = "post", post_id, draft_id, subject, model, tokens, sources
```

`<POST-id>` = `POST-YYYYMMDD-NNNNNN` (same date+seq as the source `DRAFT-…`).

## Do not

- Open Draft PRs against the org (fork only).
- Commit secrets or LinkedIn export dumps.
- Merge without the BAT promote path (Approve on fork Draft PR).
