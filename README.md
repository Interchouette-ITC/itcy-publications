# Publications - Interchouette ITC / ITCy

**Branch = kind.** Artefact trees sit at the **branch root** (no kind folders).

| Mode | Remote | Branches |
| --- | --- | --- |
| **Playground (now)** | [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications) | `drafts`, `posts` |
| **Production (later)** | [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications) | `publications` only |

Drafts never live on the org. Org holds real Publications only.

## Layout

```text
# fork branch `drafts`
DRAFT-YYYYMMDD-NNNNNN/body.md
DRAFT-YYYYMMDD-NNNNNN/meta.toml

# fork branch `posts` (playground) or org branch `publications` (production)
POST-YYYYMMDD-NNNNNN/body.md
POST-YYYYMMDD-NNNNNN/meta.toml
```

Shared scaffolding: `LICENSE`, `NOTICE`, `README.md`, `.github/`.

## BAT

**gRoussac Approve** on the Draft PR (base = fork `drafts`) is the only gate. PR comments = babysit only.

```text
/accept_draft → fork PR into drafts (`<DRAFT-id>/`)
  → gRoussac Approve (BAT)
  → ITCy writes `<POST-id>/` on fork `posts` (mock) or org `publications` (live) + ships
```

Soft/mock never writes the org.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE) and [NOTICE](NOTICE). No SPDX inside publish-ready `body.md`.
