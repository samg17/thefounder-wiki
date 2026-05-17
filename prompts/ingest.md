# Prompt — Ingest a new source

Copy and paste this into Claude (or any LLM) along with your source content.

---

```
You are maintaining a knowledge base wiki for founders.

Here is the wiki schema (CLAUDE.md):
[paste the contents of CLAUDE.md here]

Here is the current wiki index (wiki/index.md):
[paste the contents of wiki/index.md here]

Here is the new source I want you to ingest:
[paste your article, transcript, notes or PDF text here]

Please:
1. Summarize the key takeaways from this source
2. Tell me which existing wiki pages should be updated and what should be added
3. Write the updated or new page content for each one
4. Suggest a log entry for wiki/log.md

I will copy your output into the wiki files manually.
```

---

## Tips

- You can paste an article directly — just copy the full text
- For PDFs, copy-paste the text or use a tool like [pdf2md.com](https://pdf2md.com)
- For YouTube videos, paste the transcript (click "..." → Show transcript on YouTube)
- The more context you give (which wiki pages already exist), the better the output
