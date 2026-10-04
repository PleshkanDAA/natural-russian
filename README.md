# Natural Russian

A skill for AI agents that write Russian. It makes the text read like a careful person wrote it: plain connected sentences, no em dashes, no bold lead-ins, no advice tacked on at the end.

## When it helps

Without the skill, current models write Russian with habits that readers now take as signs of machine text. We counted them in 99 texts from three Claude models:

- An em dash in almost every file, 20 to 29 per 1,000 words.
- Bold lead-ins on list items and paragraphs in two texts out of three, and headings over a single sentence.
- Two independent statements glued into one sentence with a comma and "and" or "but", about nine times per 1,000 words from Sonnet and Opus and about five from Haiku.
- Advice to the reader at the end that nobody asked for, in about a third of the texts.
- Overloaded sentences in articles and reports.

A one-line rule such as "short sentences, no em dashes" removes most dashes but chops the text. The average sentence drops from about ten words to six or seven, and empty teasers like "The reason is simple." appear. Formatting and made-up details stay as they were.

The skill loads when the agent writes or rewrites Russian prose for people: docs, README files, articles, site pages, reports, letters and posts. It gives a rewrite for each job an em dash usually does and keeps sentences simple without chopping them. It changes the form of the text, not the task: content, facts and length stay as the user asked.

The skill works best with Sonnet and Opus. Haiku 4.5 follows it only in part: in our tests it still left em dashes in some texts and made up details in articles.

It does not touch code, commit messages, data files, quotes or text in other languages. The skill body is in Russian because the rules and examples are about Russian.

If you also use a typography skill that inserts em dashes into Russian text, the two will disagree. Pick one rule for dashes.

## Install

In Claude Code:

```
/plugin marketplace add PleshkanDAA/natural-russian
/plugin install natural-russian@pleshkan-natural-russian
```

Background auto-update is off for third-party marketplaces. To get new versions automatically, open `/plugin`, go to Marketplaces, select pleshkan-natural-russian and choose Enable auto-update.

In other agents that support the open [Agent Skills](https://agentskills.io) format:

```
npx skills add PleshkanDAA/natural-russian
```

## If the skill does not load

An agent picks skills by their description, so now and then it may write Russian text without loading this one. If you see that, add a line to your global `CLAUDE.md` or `AGENTS.md`:

```
Before writing Russian text for people (docs, README files, articles, site pages, reports, letters), load the natural-russian skill.
```

## Features that work only in Claude Code

None.

## Scripts and network access

None.

## License

MIT
