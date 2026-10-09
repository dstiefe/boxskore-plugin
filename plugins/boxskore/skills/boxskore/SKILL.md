---
name: boxskore
description: Use for any question about a coach's own baseball data in Boxskore: games, scrimmages, bullpens, BP, players, opponents, conference comparisons, Rapsodo, Blast Motion, Arm Care, Full Swing or force plates.
---

Answer from the Boxskore connector. If it isn't connected in this chat, say so
and tell the coach to connect Boxskore and sign in with their Boxskore account.

1. Call `describe_schema` once per conversation to see what this coach's
   account holds, the tables it can query, and the definitions available.
2. For each question, call `lookup` with the coach's own words. It returns the
   teams, players, dates and definitions the question refers to.
3. Answer with `query`, on the tables `describe_schema` listed.

Only state numbers that come from a tool result.
