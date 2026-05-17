# Founder Wiki

A structured knowledge base for founders — market research, business analysis, and decision-making frameworks. Comes pre-populated with guardrails, frameworks (Porter, JTBD, TAM/SAM/SOM), and concepts (CAC, LTV, ICP, PMF). Add your own sources and use an LLM to grow the knowledge base over time.

Instead of running RAG over raw documents on every question, an LLM **builds and maintains a persistent wiki** — a structured, interlinked collection of Markdown files that gets richer with every source you add and every question you ask.

---

## How it works

```
raw/          ← drop your sources here (articles, PDFs, transcripts)
wiki/         ← the LLM writes and maintains everything here
CLAUDE.md     ← tells the LLM how to operate the wiki
```

You handle the sources and the questions. The LLM handles everything else.

---

## Getting started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/founder-wiki
cd founder-wiki
```

### 2. Open with your LLM agent

**Claude Code:**
```bash
claude
```

Any other agent that supports local file access also works (Cursor, Codex CLI, Gemini CLI).

### 3. Tell the LLM to read the schema

```
Read CLAUDE.md and confirm you understand how to operate this wiki.
```

### 4. Ingest your first source

Drop an article, PDF or text file into `raw/` and ask:

```
Ingest the source at raw/filename.md following the instructions in CLAUDE.md.
```

### 5. Ask questions

```
Based on the wiki, what are the most common mistakes when defining ICP?
```

If the answer is valuable, ask the LLM to archive it:

```
This answer is useful. Save it as a synthesis page under wiki/sinteses/.
```

---

## Wiki structure

| Folder | What goes here |
|---|---|
| `wiki/frameworks/` | Actionable methodologies — Porter, JTBD, TAM/SAM/SOM |
| `wiki/guardrails/` | What **not** to do — biases, common mistakes |
| `wiki/conceitos/` | Core definitions — PMF, ICP, CAC, LTV |
| `wiki/entidades/` | Markets, segments and players you research |
| `wiki/sinteses/` | Cross-analyses and archived conclusions |
| `raw/` | Your raw sources (immutable — LLM reads only) |

---

## The 3 operations

**Ingest** — a new source comes in, the LLM integrates it into the wiki
**Query** — you ask a question, the LLM answers from the accumulated wiki
**Lint** — periodic maintenance: contradictions, gaps, orphan pages

See `CLAUDE.md` for the full protocol for each operation.

---

## Using with Obsidian

Obsidian is the recommended way to browse and navigate the wiki. The `wiki/` folder is a valid Obsidian vault — open it directly and all wikilinks, graph view and search work out of the box.

### Setup

1. Download [Obsidian](https://obsidian.md) (free)
2. Open Obsidian → **Open folder as vault**
3. Select the `wiki/` folder inside this repository
4. Done — all `[[wikilinks]]` are clickable, the graph view shows connections between pages

### Recommended workflow

Keep two windows open side by side: your LLM agent on one side, Obsidian on the other. The LLM edits files, you browse the results in real time — following links, checking the graph, reading updated pages.

### Recommended plugins

Install from **Settings → Community plugins**:

| Plugin | Why |
|---|---|
| **Dataview** | Queries over page frontmatter — generates dynamic tables of all `guardrails`, all pages with `status: draft`, etc. |
| **Obsidian Web Clipper** | Browser extension that converts web articles to Markdown — the fastest way to get sources into `raw/` |

### Clip articles directly to raw/

With Web Clipper installed, set the default save folder to `raw/` in the plugin settings. Any article you clip lands directly in your sources folder, ready to ingest.

### Graph view

Use **Graph view** (Ctrl/Cmd + G) to see the shape of your wiki — which pages are hubs, which are orphans, and how concepts connect. A well-maintained wiki shows tight clusters around core concepts like `icp`, `unit-economics` and `product-market-fit`.

### Keeping Obsidian settings out of git

The `.gitignore` already excludes `.obsidian/workspace` so your personal layout preferences don't get committed. The vault configuration (plugins, hotkeys) is not ignored — leave it if you want to share your setup with collaborators.

---

## Contributing

This repository is a template. Pull requests with new framework, guardrail or concept pages are welcome.

Contribution guidelines in [CONTRIBUTING.md](CONTRIBUTING.md).
