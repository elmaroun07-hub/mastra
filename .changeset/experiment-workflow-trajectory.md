---
'@mastra/core': patch
---

Fixed trajectory scorers in dataset experiments receiving an empty trajectory for workflow targets when trace storage is unavailable. The scorer now gets the workflow's executed steps, the same fallback `runEvals` uses, instead of scoring a run that executed steps as if it had executed none.
