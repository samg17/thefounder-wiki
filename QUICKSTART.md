# Quickstart

Three steps to get your wiki running.

---

## Step 1 — Get the wiki

Click **Use this template** → **Create a new repository** → clone it to your computer.

```bash
git clone https://github.com/your-username/thefounder-wiki
cd thefounder-wiki
```

---

## Step 2 — Open it

**With Obsidian (recommended for browsing):**
1. Download [Obsidian](https://obsidian.md) — free
2. Open Obsidian → **Open folder as vault** → select the `wiki/` folder
3. Done — all pages and links are navigable

**With an LLM agent (recommended for adding knowledge):**

Option A — Claude Code (terminal):
```bash
claude
```
Then say: `Read CLAUDE.md and confirm you understand how to operate this wiki.`

Option B — Claude.ai (no terminal needed):
1. Go to [claude.ai](https://claude.ai)
2. Upload the files from the `wiki/` folder
3. Copy the prompt from `prompts/ingest.md` and paste it with your source

---

## Step 3 — Add your first source

Drop any article, PDF or text into the `raw/` folder. Then use the prompt in `prompts/ingest.md`.

That's it. The wiki grows every time you add a source or ask a question.

---

## What's already in the wiki

| Topic | Pages |
|---|---|
| Frameworks | Porter 5 Forces, Jobs to Be Done, TAM/SAM/SOM |
| Guardrails | Market research mistakes, Competitive analysis pitfalls, Cognitive biases |
| Concepts | Unit Economics, ICP, Product-Market Fit |

Browse them in Obsidian or ask the LLM: `What are the most common mistakes in market research?`
