---
'@e2e-dev/core': patch
---

Actions, `waitFor`, and assertions that miss on their first read now read again after 20 ms, then 50 ms, then every 100 ms as before. A node or state that arrives just after the first read is seen up to 80 ms sooner.
