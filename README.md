# Lexamica Articles — Demo Repo

Proof-of-concept: **articles stored as Markdown in GitHub → synced into the Framer CMS → published as article pages.**

This is the pipeline the CEO wants:
> Calls / Slack / Fathom → Claude drafts article topics & content → stored here in GitHub → auto-published as article pages.

## Structure
- `/articles/*.md` — one Markdown file per article, with frontmatter (title, slug, date, excerpt, author, tags).

## How it syncs to Framer (demo path — no code)
1. In Framer, open (or create) an **Articles** CMS collection.
2. Install the **GitHub Collections Sync** plugin from the Framer marketplace.
3. Connect it to this repo, branch `main`, base path `articles/`.
4. Map the frontmatter fields → your CMS fields.
5. Click **Sync** → articles appear as CMS items → render on the article template.
6. Add/edit a `.md` file here → re-sync → changes appear.

## Frontmatter fields used
| Field | Meaning |
|---|---|
| `title` | Article headline |
| `slug` | URL slug |
| `date` | Publish date |
| `excerpt` | Short summary / meta description |
| `author` | Author name |
| `tags` | Topic tags |
