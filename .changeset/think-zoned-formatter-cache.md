---
"@cloudflare/think": patch
---

Reuse one `Intl.DateTimeFormat` per timezone when resolving wall-clock scheduled tasks, cutting the CPU cost of each occurrence from ~100ms to a few ms. See [Scheduled Tasks](https://github.com/cloudflare/agents/blob/main/docs/think/index.md#scheduled-tasks).
