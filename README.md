# Glyph Library

A perception spec for AI agents. It translates a scene into a grid of ASCII glyphs where each glyph names what a thing **does** to the agent — yield, offset, never share its lane — not what the thing is. It is built for agents that perceive through text: an agent reading a frame of glyphs knows what each cell asks of it without ever being told what the cell "is."

The whole spec rests on five floor rules, stated in full in the library itself:

1. A glyph names what a thing does to the agent, not what it is. Same move, same glyph.
2. One character is one cell.
3. Digits are speed, only speed.
4. `?` means don't guess.
5. Case asks one question: is a decider engaged?

## Current version

**v1.4** is the current canon. Start there.

## Files

- `Glyph_Library_v1.4.md` — the current spec.
- `Glyph_Library_v1.3.md`, `v1.2.md`, `v1.1.md`, `v1.0.md` — the version lineage. Each file carries its own change notes; the library was built by readers disagreeing and the spec absorbing the disagreement.
- `Glyph_Pipeline_Notes.md` — the implementation layer around the spec: what senses feed it, which layers are buildable now, and the questions only field data can answer. The library stays syntax-only; everything implementation lives there.
- `Glyph_Quiz_v1.4.md` — a reading quiz for the spec: 17 strings and 4 frames, taken cold from v1.4 alone. The answer key is held by the chorus and is not published; frames are written fresh for each round.

## How to test it

Agreement is the test. Take a frame from the library (or write one from a real scene), have two independent readers parse it cold, and compare readings. Where they agree, the spec held. Where they differ, that is information about the glyph — file an issue with the frame and both readings. Do not pick a winner; add a definition or an example.

Known open problem, flagged in the spec itself: **the agent crossing** — with the agent standing on a road row or on a painted crossing, the sidewalk side is ambiguous. See issue #1.

## Who made this

Written by a chorus of AI agents working as peer readers — Claude (v1.3 and v1.4 drafts), DeepSeek (v1.2 draft), and Rowan (integration, blind testing, ratification) — guided and audited by Ryan Smith, who set the question, supplied the field judgment, and graded every round. No version was accepted on one reader's say-so; each survived independent reads scoring 19/20 agreement or better before it was filed as canon.

Published openly. Use it, fork it, test it, break it — and file what breaks.

## License — public domain

This library is dedicated to the public domain under **CC0 1.0** (see `LICENSE`). Take it, build on it, sell what you build. No permission, no royalty, no attribution required — the library is a commons, and a commons is for using.

## A tit for a tat

One request, made as a norm and not a condition — CC0 asks nothing, and this changes nothing in the license. If the glyphs find work in your project, send word of what they did there: open an issue in this repository and tell the library. Field reports, failures, and any new glyphs your work taught you are how the shared knowledge expands — and how the next reader starts further down the road than you did.

---

*Published by Rowan. This is AI-authored work, written by AI agents and labeled as such on purpose.*
