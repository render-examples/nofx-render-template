# Sanity submission: NOFX

Use when filing a **production** catalog entry for [render.com/templates](https://render.com/templates).

**Source repo:** https://github.com/ojusave/nofx (branch `dev`)  
**Gallery repo (Sanity GitHub field + one-click fork):** https://github.com/render-examples/nofx-render-template  
**One-click deploy:** `https://render.com/deploy-template/api/github/start?template_repo=nofx-render-template`  
**Gallery URL (target):** `https://render.com/templates/nofx`

---

## Blockers before submit

- [x] **`assets/hero.png`** — sign-in screenshot (catalog card; copy of `sign-in.png`)
- [x] **`assets/sign-in.png`**, **`assets/config.png`**, **`assets/agent.png`** — live deploy screenshots for README / detail page
- [x] Repo published under **`render-examples/nofx-render-template`** with `is_template: true`
- [ ] Smoke deploy from an account that does not own the template repo
- [ ] Sanity **development** draft in Studio (see [`../sanity-drafts/STUDIO-WALKTHROUGH.md`](../sanity-drafts/STUDIO-WALKTHROUGH.md))

---

## Sanity Studio fields

Create document: **Templates** → new document

| Field | Value |
|-------|--------|
| **Title** | `NOFX on Render` |
| **Slug** | `nofx` |
| **Description** | Self-host NOFX with one click: an AI trading terminal that connects to 10+ exchanges and LLM providers. Single Render web service with SQLite on a persistent disk. |
| **GitHub Repository** | `https://github.com/render-examples/nofx-render-template` *(required for Deploy button; synced from `ojusave/nofx` `dev`)* |
| **Demo URL** | *(optional)* After smoke deploy from `dev` |
| **Image** | Upload `assets/hero.png` (sign-in page; same as `sign-in.png`) |
| **Stack** | `docker`, `go`, `react`, `sqlite` |
| **Tags** | `ai`, `trading`, `llm`, `crypto`, `fintech` |
| **Sort Order** | *(optional)* |
| **Body (Markdown)** | Paste full contents of this repo's `README.md` |

---

## gallery-metadata.json

Already at [`gallery-metadata.json`](./gallery-metadata.json). Attach to the handoff email/ticket.

---

## Production checklist

- [ ] Document published on Sanity **`production`** dataset
- [ ] `https://render.com/templates/nofx` returns 200
- [ ] Catalog card shows hero image and description
- [ ] **Deploy this template** forks repo and Apply succeeds
- [ ] First-time registration works; `/api/config` returns JSON
