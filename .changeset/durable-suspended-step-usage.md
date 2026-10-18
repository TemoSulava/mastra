---
'@mastra/core': patch
---

Fixed missing token usage on durable and evented engines when a tool call suspends or waits for approval. Suspended `stream()` and `generate()` results and suspension chunks now include the suspended step's token usage. See #27440.
