# Author Voice

Use author profile data when available. Do not mimic private details or invent personal experience.

Supported profile fields:

```json
{
  "tone": {
    "formality": 5,
    "opinionated": 5
  },
  "phrases": {
    "signature": [],
    "avoid": []
  },
  "vocabulary": {
    "use_freely": [],
    "always_explain": []
  },
  "voice_analysis": {
    "sentence_structure": {
      "avg_length": 16,
      "variety": "short | moderate | long"
    },
    "communication_style": [],
    "characteristic_expressions": [],
    "sentence_starters": [],
    "signature_vocabulary": []
  }
}
```

Apply voice by:

- matching formality and confidence
- using signature phrases sparingly
- avoiding forbidden phrases completely
- explaining required vocabulary on first use
- keeping sentence rhythm close to the profile
- preserving the author's known opinions only when provided

Do not overfit. The article should still read naturally and prioritize clarity.
