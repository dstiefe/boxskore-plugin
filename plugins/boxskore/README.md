# Boxskore

Ask Claude about your baseball program's own data in Boxskore: TrackMan games and training
sessions, bullpens, BP, Rapsodo, Blast Motion, Arm Care, Full Swing and force plates.

You need a Boxskore coach account. Installing the plugin does not grant access to any data.

Install in Claude Code:

    /plugin install boxskore --marketplace dstiefe/boxskore-plugin

## What it contains

- **A connector** to Boxskore's server at `https://boxskore.com/api/mcp`. The first time you use
  it, you sign in with your Boxskore account. Every answer then comes from the data that
  account can already see in the Boxskore app; other programs' private data is never visible.
- **A short skill** that tells Claude to answer Boxskore questions from the connector and to
  state only numbers that come from it.

## What it sends

Your questions and the queries Claude writes go to Boxskore's server, which returns rows from
your account's data. Boxskore records each request for security and support. The plugin runs
nothing on your computer and sends nothing anywhere else.

## Tools

All tools are read-only:

- `describe_schema`: what your account's data holds and the tables you can query
- `lookup`: the teams, players, dates and definitions a question refers to
- `wiki_pages`: Boxskore's definition pages
- `query`: one read-only PostgreSQL query on your account's data

## Support

https://boxskore.com
