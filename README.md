# Publications - Interchouette ITC / ITCy

**Branch = kind.** Artefact trees sit at the **branch root** (no kind folders).

Same branch names on both remotes; the **remote** is playground vs production:

| Mode | Remote | LinkedIn | X |
| --- | --- | --- | --- |
| **Playground (now)** | [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications) | `drafts` / `posts` | `drafts_tweet` / `tweets` |
| **Production (later)** | [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications) | `drafts` / `posts` | `drafts_tweet` / `tweets` |

## Layout

```text
# on branch `drafts` (fork playground or org production)
DRAFT-YYYYMMDD-NNNNNN/body.md
DRAFT-YYYYMMDD-NNNNNN/meta.toml

# on branch `posts` (fork playground or org production)
POST-YYYYMMDD-NNNNNN/body.md
POST-YYYYMMDD-NNNNNN/meta.toml

# on branch `drafts_tweet`
TWEET-YYYYMMDD-NNNNNN/body.md
TWEET-YYYYMMDD-NNNNNN/meta.toml

# on branch `tweets`
XPOST-YYYYMMDD-NNNNNN/body.md
XPOST-YYYYMMDD-NNNNNN/meta.toml
```

`kind` in meta: `"draft"` / `"post"` / `"tweet"` / `"xpost"`. Tweet meta holds `cite` and optional `quote_tweet_id` (X status cite ships as a quote tweet).

Shared scaffolding: `LICENSE`, `NOTICE`, `README.md`, `.github/`.

## BAT

**gRoussac Approve** on the PR (base = `drafts` or `drafts_tweet` on the active remote) is the only gate. PR comments = babysit only.

```text
/accept_draft → PR into drafts (`<DRAFT-id>/`)
  → gRoussac Approve (BAT)
  → ITCy writes `<POST-id>/` on posts + ships LinkedIn

/accept_tweet → PR into drafts_tweet (`<TWEET-id>/`)
  → gRoussac Approve (BAT)
  → ITCy writes `<XPOST-id>/` on tweets + ships X
```

Soft/mock uses the **fork** only. Live / cutover uses the **org**.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE) and [NOTICE](NOTICE). No SPDX inside publish-ready `body.md`.
