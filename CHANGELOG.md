# Changelog

All notable changes to this plugin are documented here. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and versions follow [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [0.1.1] - 2026-10-05

### Changed

- README: plainer wording, and the figure for sentences glued with a comma and "and" or "but" now says it holds for Sonnet and Opus, while Haiku does this about half as often.

## [0.1.0] - 2026-10-01

### Added

- First release. The skill loads when an agent writes or rewrites Russian prose for people: docs, README files, articles, site pages, reports, letters and posts. It also loads when the text is one step of a larger task or goes to a subagent.
- A rewrite for every place where models put an em dash, so the sentence keeps its verb instead of turning into a bare "X is Y" with the dash dropped.
- Plain connected sentences: no comma-and glue in every other sentence, no overloaded sentences, no chopped telegram style.
- Formatting by genre, without bold lead-ins, headings over a single sentence, emoji or dividers.
- No filler and no made-up figures, studies, quotes or customer stories when the user gave no material for them.
- A final check the agent runs on the written file before handing it over.
