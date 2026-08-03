# Publications - Interchouette ITC / ITCy

**Branch = kind.** Artefact trees sit at the **branch root** (no `drafts/` or `posts/` folders).

| Mode | Remote | Branches |
| --- | --- | --- |
| **Playground (now)** | [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications) | `drafts`, `posts` |
| **Production (later)** | [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications) | `drafts`, `publications` |

## Layout

```text
# on branch `drafts`
DRAFT-YYYYMMDD-NNNNNN/body.md
DRAFT-YYYYMMDD-NNNNNN/meta.toml

# on branch `posts` (playground) or `publications` (org)
POST-YYYYMMDD-NNNNNN/body.md
POST-YYYYMMDD-NNNNNN/meta.toml
```

Shared scaffolding on every branch: `LICENSE`, `NOTICE`, `README.md`, `.github/`.

## BAT

**gRoussac Approve** on the Draft PR (base = `drafts`) is the only gate. PR comments = babysit only.

```text
/accept_draft → PR into drafts (`<DRAFT-id>/`)
  → gRoussac Approve (BAT)
  → ITCy writes `<POST-id>/` on posts (playground) or publications (live) + ships
```

Soft/mock never writes the org. Live / cutover uses org `publications`.

Worker remote: **`interchouette`** (fork); **`upstream`** = org. Never `git push upstream`.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE) and [NOTICE](NOTICE). No SPDX inside publish-ready `body.md`.
