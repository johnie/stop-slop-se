# Stop Slop SE

A skill for removing Swedish AI tells from prose, with a focus on corporate and Linkedin Swedish.

<img width="3840" height="2160" alt="G-Yg4RVbIAAhVxW" src="https://github.com/user-attachments/assets/902afc15-1f40-4a9d-af24-8cd67afb8ebf" />

## What this is

Swedish AI prose has its own habits: consultant jargon, employer-branding floskler, translated-English scaffolding, vague uplift language, actor-hiding passives, and polished LinkedIn cadence.

`stop-slop-se` keeps the core anti-slop workflow from the original skill, but rewrites the heuristics for native Swedish use. The frontmatter and README stay in English for trigger reach. The skill body and reference material are in Swedish.

## Skill structure

```
stop-slop-se/
├── SKILL.md              # Core instructions (Swedish body, English frontmatter)
├── references/
│   ├── phrases.md        # Swedish phrases and jargon to cut
│   ├── structures.md     # Swedish structural patterns to avoid
│   └── examples.md       # Native Swedish before/after examples
├── README.md
└── LICENSE
```

## Quick start

**Claude Code:** Add this folder as a skill.

**Claude Projects:** Upload `SKILL.md` and the reference files to project knowledge.

**Custom instructions:** Copy the core rules from `SKILL.md`.

**API calls:** Include `SKILL.md` in your system prompt. Load the reference files on demand.

## What it catches

**Swedish floskler** - Throat-clearing openers, meta-signposting, vague uplift, boosters, and corporate filler. See `references/phrases.md`.

**Corporate/LinkedIn jargon** - Consultant vocabulary, employer-branding clichés, and unnecessary English that signals status more than meaning. See `references/phrases.md`.

**Structural clichés** - Negation pivots, actor-hiding passives, abstract-subject fog, noun-heavy abstraction, polished triads, and LinkedIn sermon rhythm. See `references/structures.md`.

**Sentence-level rewrites** - Name the actor, cut translated-English cadence, and replace vague claims with concrete Swedish prose.

## Scoring

Rate 1-10 on each dimension:

| Dimension | Question |
|-----------|----------|
| Idiomatic Swedish | Does it sound like natural Swedish prose? |
| Concreteness | Are the people, actions, and decisions clear? |
| Agency | Can you tell who did what? |
| Jargon load | How much consultant fog is left? |
| LinkedIn salesiness | Does it read like a person or a brand post? |

Below 35/50: revise.

## Design choice

This skill is not a literal translation of the English version. Swedish needs different pressure points. The biggest tells are usually not English-style adverbs or em dashes; they are jargon, abstract nouns, passive responsibility-dodging, and translated-English cadence.

## Author

[Johnie Hjelm](https://johnie.se)

## License

MIT. Use freely, share widely.
