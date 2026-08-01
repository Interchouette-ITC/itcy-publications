# Drafts layout (Interchouette fork)

**Draft** artefacts on **Interchouette/itcy-publications** live under `drafts/<DRAFT-id>/`.

Org Posts live under `posts/<POST-id>/` on Interchouette-ITC after BAT Approve + promote.

## Path

```text
drafts/<DRAFT-id>/
  body.md      # Draft body (header: Draft ID: DRAFT-YYYYMMDD-NNNNNN)
  meta.toml    # kind = "draft", draft_id, subject, model, tokens, sources
```

Branch: `draft/<DRAFT-id>`. PR base = fork `dev`. Reviewer = gRoussac (BAT gate).
