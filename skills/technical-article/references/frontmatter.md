# Frontmatter

Adapt frontmatter to the publishing platform. Default:

```yaml
---
title: ""
description: ""
date: "YYYY-MM-DD"
author: ""
language: "en"
tags: []
canonical_url: ""
translations: []
sources: []
example:
  path: "code/"
  verified: true
---
```

Rules:

- Keep title specific and searchable.
- Description should state reader value, not repeat the title.
- Tags should be few and relevant.
- Do not mark `example.verified: true` unless verification actually ran and passed.
