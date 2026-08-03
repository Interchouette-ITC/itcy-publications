# Publications - Interchouette ITC / ITCy

**Branch = kind.** Artefact trees sit at the **branch root** (no kind folders).

Same branch names on both remotes; the **remote** is playground vs production:

| Mode | Remote | Branches |
| --- | --- | --- |
| **Playground (now)** | [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications) | `drafts` (playground), `posts` (playground) |
| **Production (later)** | [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications) | `drafts` (real), `posts` (real) |

## Layout

```text
# on branch `drafts` (fork playground or org production)
DRAFT-YYYYMMDD-NNNNNN/body.md
DRAFT-YYYYMMDD-NNNNNN/meta.toml

# on branch `posts` (fork playground or org production)
POST-YYYYMMDD-NNNNNN/body.md
POST-YYYYMMDD-NNNNNN/meta.toml
```

Shared scaffolding: `LICENSE`, `NOTICE`, `README.md`, `.github/`.

## BAT

**gRoussac Approve** on the Draft PR (base = `drafts` on the active remote) is the only gate. PR comments = babysit only.

```text
/accept_draft → PR into drafts (`<DRAFT-id>/`)
  → gRoussac Approve (BAT)
  → ITCy writes `<POST-id>/` on posts + ships
```

Soft/mock uses the **fork** only. Live / cutover uses the **org**.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE) and [NOTICE](NOTICE). No SPDX inside publish-ready `body.md`.
