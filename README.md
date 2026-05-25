# no-ai-slop-writing-rules

> # 👋 Hi, you were probably sent here.
>
> ## If someone handed you a link to this repo, it is because you sent them AI-generated shit so obviously AI-generated that they stopped reading partway through and went looking for a polite way to say "run it through a human first."
>
> Pasting raw Gemini or ChatGPT output with zero editing, or running a project with no anti-slop rules at all, is the 2026 equivalent of handing out a business card with an `@aol.com` email on it. The tool is fine. Shipping its first draft with your name on it is the part people notice.
>
> Nobody is mad that you used a model. Everybody can tell the em dashes, the "it's important to note," the "in today's fast-paced world," and the three identical paragraphs that each say nothing were not yours. Read your own output before you send it. That is the whole ask.
>
> The rules below are what "read it first" looks like written down. Steal them.

---

A portable Claude Code reference for writing in Louis Rossmann's voice without AI slop. It is general-purpose: essays, scripts, posts, documentation, emails, anything made of sentences. It is not tied to any wiki, CMS, or publishing system.

## What it does

It gives Claude two things. First, a hard rule set that strips the patterns marking machine-generated text: emdashes, intensifiers, filler phrases, hollow statements, fabricated facts, AI transition words, dramatic headings, and the rest. Second, a data-driven voice profile built from corpus analysis of 513,683 words of Rossmann's writing: testable-number density, high sentence-length variance, claim-then-proof paragraph structure, contractions, the ampersand habit, and contempt shown through precision rather than adjectives.

## How to use it

Drop this folder next to a project, or point Claude Code at it. When you ask Claude to write or edit prose, it reads `CLAUDE.md` and the two skills, writes against the rules, then self-checks the output against the banned-words reference before returning it.

You can also read the files yourself as a style guide. Every file here obeys its own rules, so they double as worked examples.

## What each file does

| File | Contents |
|---|---|
| `CLAUDE.md` | The entrypoint. States the purpose, summarizes the voice, sets the operating rules, and lists all 24 anti-slop rules. |
| `.claude/skills/no-ai-slop/SKILL.md` | The anti-slop rules as actionable guidance, with WRONG/RIGHT worked examples and a self-check pass. |
| `.claude/skills/no-ai-slop/references/ai-writing-detection.md` | The full banned-words reference: verbs, adjectives, transitions, phrases, intensifiers, heading anti-patterns, academic tells, hedging markers, and structural and statistical patterns. |
| `.claude/skills/rossmann-voice/SKILL.md` | The voice profile: sentence-level rules, paragraph structure, drift prevention, the Claim-Mechanism-Reality argument pattern, a vocabulary guide, a DO/DON'T table, and the statistical fingerprint. |

## Scope

The examples in the voice skill are repair-themed because that is what the source corpus covers. The traits themselves are structural, so the voice applies to any subject. Write about anything in it; the rules hold.
