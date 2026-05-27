# Research Standards

Use current sources when technical facts may have changed. Prefer primary sources:

1. Official documentation
2. Release notes and changelogs
3. Standards, RFCs, specifications
4. Source repositories and issue discussions
5. Vendor engineering blogs
6. Reputable community articles
7. Personal blogs and forum posts

Record each source in `sources.json`:

```json
{
  "title": "Source title",
  "url": "https://example.com",
  "publisher": "Publisher",
  "date_published": "YYYY-MM-DD or unknown",
  "date_accessed": "YYYY-MM-DD",
  "type": "official-docs | release-notes | source | article | issue | other",
  "used_for": "What claim or section this source supports"
}
```

Research notes should separate:

- confirmed facts
- version-specific behavior
- claims that need citation
- opinions or interpretation
- unresolved questions

Rules:

- Do not cite outdated docs for current behavior unless explaining history.
- Do not cite AI-generated content as an authority.
- If sources conflict, explain the conflict or use the most authoritative current source.
- Use direct quotes only when wording matters; otherwise paraphrase.
