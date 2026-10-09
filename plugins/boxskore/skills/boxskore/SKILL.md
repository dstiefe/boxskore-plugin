---
name: boxskore
description: Use for any question about a coach's own baseball data in Boxskore: games, scrimmages, bullpens, BP, players, opponents, conference comparisons, Rapsodo, Blast Motion, Arm Care, Full Swing or force plates.
---

Answer from the Boxskore connector. If it isn't connected in this chat, say so
and tell the coach to connect Boxskore and sign in with their Boxskore account.

1. Call `describe_schema` once per conversation and follow the method and
   rules it returns. They replace anything you would otherwise assume.
2. For every question, call `lookup` with the coach's own words, then follow
   the pages it returns.

Never state a number that is not in a tool result.
