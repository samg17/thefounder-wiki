# Prompt — Ask a question

Copy and paste this into Claude (or any LLM) to query your wiki.

---

```
You are maintaining a knowledge base wiki for founders.

Here are the relevant wiki pages:
[paste the content of the pages most relevant to your question]

Based on the wiki above, please answer the following question:
[your question here]

If the answer references something not covered in the wiki, flag it as a gap
and suggest what source I should look for to fill it.

If the answer is valuable, also write a synthesis page I can save to wiki/syntheses/.
```

---

## Example questions

- What are the most common mistakes when defining ICP?
- How do I calculate LTV for a SaaS business?
- What cognitive biases should I watch out for when analyzing competitors?
- How do I know if I have product-market fit?
- What's the difference between SAM and SOM?

## Tips

- Paste 2–3 relevant wiki pages for better answers
- Not sure which pages are relevant? Paste `wiki/index.md` and ask the LLM to pick
- Save good answers back to `wiki/syntheses/` — they become part of your knowledge base
