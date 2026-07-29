# Posts layout (BAT drafts)

Ready-to-ship LinkedIn drafts live under `posts/<slug>/`. A PR that adds or updates a slug is the BAT artifact. **Merge after gRoussac Approve** (BAT). Publish to LinkedIn is a product step after merge.

**License:** Post drafts here are (c) Interchouette-ITC, BUSL-1.1 - see [NOTICE](NOTICE) and the repository root [LICENSE](../LICENSE). Do not add copyright or SPDX lines inside `body.md`; that file is publish-ready LinkedIn copy.

## Path

```text
posts/<slug>/
  body.md      # Post body in English (comment replies: match comment language)
  meta.toml    # Traceability + disclosure inputs
```

`<slug>` is lowercase ASCII kebab-case (`ai-mascot-intro`, `near-weekly-note`). Unique per open PR; reuse only when reworking the same draft.

## `body.md`

- Full post text ITCy would publish on the company page.
- Must include the disclosure line (see work contract):

```text
Written by AI - ITCy - model <provider>/<id> - tokens in:<n> out:<n>
```

## `meta.toml`

```toml
kind = "post"                 # post | reply (reply later)
subject = "ai mascot intro"
created_at = "2026-07-22T18:00:00Z"
model = "ollama/llama3.2"
tokens_in = 1200
tokens_out = 400
sources = [
  "https://example.com/article",
]
```

## Do not

- Commit secrets or personal LinkedIn export dumps.
- Publish to LinkedIn from this repo (product binary does that after BAT merge).
- Merge without **gRoussac Approve** (BAT).
