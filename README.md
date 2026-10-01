# wordsmith

A structured AI writing and editorial skill for drafting, rewriting, critique, clarity, tone, concision, and publication review.

## What this skill does

`wordsmith` helps with:

- creating drafts from ideas or notes;
- building outlines;
- rewriting existing text;
- preserving the author's voice;
- improving grammar and clarity;
- tightening long or repetitive writing;
- changing tone;
- reviewing structure and audience fit;
- identifying unsupported claims;
- preparing content for publication.

## Installation

Copy the following directory into the skills directory supported by your AI agent:

```text
skills/wordsmith/
```

Depending on the agent platform, that may be one of:

```text
.claude/skills/wordsmith/
.agents/skills/wordsmith/
.cursor/skills/wordsmith/
.qoder/skills/wordsmith/
```

Consult the documentation for the agent platform you use to determine the correct location.

## Usage

You can invoke the skill with a command:

```text
/wordsmith draft
/wordsmith rewrite
/wordsmith critique
/wordsmith audit
/wordsmith tighten
/wordsmith polish
/wordsmith final
```

You can also use natural language:

```text
Rewrite this email to sound warm and confident.
```

```text
Check this article for repetition and unsupported claims.
```

```text
Make this explanation easier for a general audience to understand.
```

## Commands

### Build

- `brief` — turn an idea into a clear writing brief;
- `outline` — create a logical structure;
- `draft` — write new content;
- `develop` — expand notes into a complete piece;
- `compose` — combine fragments into one coherent draft;
- `continue` — continue an existing piece;
- `finish` — complete an unfinished draft.

### Evaluate

- `critique` — explain what works and what needs improvement;
- `audit` — perform a structured quality review;
- `diagnose` — identify the main reason a piece is weak;
- `clarity` — identify confusing or ambiguous language;
- `voice` — analyze voice and style;
- `structure` — review organization and flow;
- `audience` — check audience fit;
- `accuracy` — identify claims that require verification;
- `readability` — review complexity and accessibility.

### Refine

- `edit` — improve grammar and wording while preserving the voice;
- `rewrite` — substantially transform the writing;
- `polish` — perform a final refinement pass;
- `tighten` — make the writing shorter and more direct;
- `simplify` — make difficult writing easier to understand;
- `smooth` — improve flow and transitions;
- `strengthen` — improve weak arguments or wording;
- `proof` — correct mechanical errors.

### Adapt

- `tone` — change the emotional or professional tone;
- `formalize` — make writing more formal;
- `humanize` — make writing warmer and less mechanical;
- `shorten` — reduce the length;
- `expand` — add useful detail;
- `summarize` — produce a concise version;
- `headline` — create titles and headings;
- `subject` — create email subject lines;
- `repurpose` — adapt content for multiple channels;
- `translate` — translate while preserving intent;
- `localize` — adapt language and cultural references.

### Prepare

- `factcheck` — identify factual claims that need verification;
- `evidence` — identify where sources or citations are needed;
- `inclusive` — review language for unnecessary exclusion or stereotyping;
- `accessibility` — improve readability and accessibility;
- `consistency` — check names, terms, dates, and formatting;
- `compare` — compare two versions;
- `diff` — explain what changed;
- `final` — prepare content for publication or sending;
- `release` — return only the final copy.

## Common aliases

These aliases map to the main commands:

| Alias | Main command |
|---|---|
| `proofread` | `edit` |
| `grammar` | `edit` |
| `review` | `critique` |
| `check` | `audit` |
| `shorten` | `tighten` |
| `condense` | `tighten` |
| `make-clear` | `clarity` |
| `make-simple` | `simplify` |
| `ready-to-send` | `final` |
| `publication` | `final` |

## Typical workflows

### Write something new

```text
/wordsmith brief
/wordsmith outline
/wordsmith draft
/wordsmith critique
/wordsmith polish
```

### Improve existing writing

```text
/wordsmith critique
/wordsmith rewrite
/wordsmith polish
```

### Prepare an email

```text
/wordsmith rewrite
/wordsmith tone warm and direct
/wordsmith tighten
/wordsmith final
```

### Prepare important content

```text
/wordsmith audit
/wordsmith factcheck
/wordsmith accessibility
/wordsmith final
```

## Design principles

`wordsmith` should:

- preserve the author's intended meaning;
- preserve important facts, names, numbers, and quotations;
- avoid inventing facts, sources, statistics, or experiences;
- match the requested audience and tone;
- use clear and direct language;
- preserve the author's voice unless asked to change it;
- explain substantial changes;
- identify uncertainty instead of pretending to know;
- return the requested writing before lengthy commentary.

`wordsmith` should not:

- silently change dates, numbers, names, or commitments;
- make unsupported claims sound certain;
- replace a personal voice with generic corporate language;
- rewrite everything when the user only requested proofreading;
- claim that content is factually correct without verification;
- add fake citations or sources.

## Development

The source repository is a Copier template.

Generate a new project:

```bash
copier copy https://github.com/arm-pz/agent-skill-template.git wordsmith
```

Update a previously generated project:

```bash
cd wordsmith
copier update
```

Copier stores the original answers in:

```text
.copier-answers.yml
```

## License

Add your chosen license here.
