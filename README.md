**🇬🇧 English | 🇮🇷 [فارسی](README.fa.md)**

# Solar Panel Management System - Database Project

**Team:** E. Nima, P. Ali, S. Amir

## Project Phases
- [x] Phase 1 — Requirements
- [x] Phase 2 — ER Model
- [ ] Phase 3 — Relational Schema
- [ ] Phase 4 — Normalization
- [ ] Phase 5 — SQL Implementation
- [ ] Phase 6 — Testing & Queries

## Phase Documents

### Phase 1 — Requirements

| Format | 🇬🇧 English | 🇮🇷 Persian |
|:--|:--|:--|
| 📝 Markdown | [`01-requirements.md`](docs/01-requirements.md) | [`01-requirements.fa.md`](docs/01-requirements.fa.md) |
| 📄 PDF | [`Helios-db-RC.pdf`](docs/source/Helios-db-RC.pdf) | [`Helios-db-RC-fa.pdf`](docs/source/Helios-db-RC-fa.pdf) |
| 📦 Source (`.docx`) | [`Helios-db-RC.docx`](docs/source/Helios-db-RC.docx) | [`Helios-db-RC-fa.docx`](docs/source/Helios-db-RC-fa.docx) |

### Phase 2 — ER Model

| Format | 🇬🇧 English | 🇮🇷 Persian |
|:--|:--|:--|
| 📝 Markdown | [`02-er-diagram.md`](docs/02-er-diagram.md) | [`02-er-diagram.fa.md`](docs/02-er-diagram.fa.md) |
| 🎨 Diagram source (`.drawio`) | [`Helios-db-ER.drawio`](diagrams/Helios-db-ER.drawio) | [`Helios-db-ER-fa.drawio`](diagrams/Helios-db-ER-fa.drawio) |
| 🖼️ Diagram (SVG) | [`Helios-db-ER.drawio.svg`](diagrams/Helios-db-ER.drawio.svg) | [`Helios-db-ER.fa.drawio.svg`](diagrams/Helios-db-ER-fa.drawio.svg) |

## Repository Structure

```
Helios-DB/
├── README.md
├── README.fa.md
├── .gitignore
├── .gitattributes
├── docs/
│   ├── requirements.md
│   ├── requirements.fa.md
│   ├── 02-er-diagram.md
│   ├── 02-er-diagram.fa.md
│   └── source/
│       ├── Helios-db-RC.docx
│       ├── Helios-db-RC.pdf
│       ├── Helios-db-RC-fa.docx
│       └── Helios-db-RC-fa.pdf
├── diagrams/
│   ├── Helios-db-ER.drawio
│   ├── Helios-db-ER.drawio.svg
│   ├── Helios-db-ER-fa.drawio
│   └── Helios-db-ER-fa.drawio.svg
└── sql/
    └── queries/
```

## How to Run the SQL
_TBD_


## Notes
- PDFs in `docs/source/` are generated from the `.docx` files. Regenerate if the `.docx` changes.
- If the inline PDF viewer fails on GitHub, use the **Download** button, or append `?raw=true` to the PDF URL to open it in the browser's native viewer.

---

> This README is also available in [Persian](README.fa.md). Any change to project status, structure, or phase list will be applied to **both** files.

---

## Tags

Annotated tags mark each completed phase. Use them to jump back to a finished phase or to diff two phases.

| Tag | Phase | Status |
|---|---|---|
| `v0.1-requirements` | Phase 1 — Requirements | ✅ done |
| `v0.2-er-model` | Phase 2 — ER Model | ✅ done |
| `v0.3-relational-schema` | Phase 3 — Relational Schema | ⏳ planned |
| `v0.4-normalization` | Phase 4 — Normalization | ⏳ planned |
| `v0.5-sql` | Phase 5 — SQL Implementation | ⏳ planned |
| `v1.0-final` | Phase 6 — Testing & Final Submission | ⏳ planned |

**Useful commands**
```bash
git tag -n                                   # list tags with messages
git checkout v0.1-requirements               # inspect a finished phase (detached HEAD)
git switch -                                 # go back to where you were
git diff v0.1-requirements..v0.2-er-model    # what changed between two phases
```
