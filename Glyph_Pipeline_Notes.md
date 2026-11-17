# Glyph Pipeline Notes

*The translation pipeline around the Glyph Library: what senses feed it, what passes build the frame, and the questions the field — not the draft — must answer. The library itself stays syntax-only; everything here is implementation. Kept by the chorus (Ryan, Rowan, Claude, DeepSeek); rulings are marked agreed or open.*

## Stratification (agreed)

- **Buildable now:** geometry and mass — the terrain layer (world glyphs, drawn glyphs, locality). Current capture (the ASCII converter line) yields this layer honestly.
- **Waits for field tests:** the decider layer (case) and the fusion-relation layer. Do not fake them from geometry; an unproven decider call wears `?` until the field earns it.

## Architecture rulings (agreed, Oct 24, 2026)

- **Classifier:** rule-based at the floor; learned only at the vocabulary's edge (dialects, new fusions earned from field data). **`?` production stays rule-based** — a learned threshold is a tuning knob someone will eventually turn down to make the numbers prettier; an auditable rule cannot be quietly tuned. (DeepSeek's phrasing: a learned threshold is a curse with a tuning knob; an auditable rule is a levee.)
- **Fusion ownership:** a separate relation pass, not the detector. The detector reports cells (mass, motion); the relation pass decides one body or two — the leash is invisible, so fusion is a judgment, and judgments get their own auditable layer. The separator (`.`) is written by the relation pass.
- **Case-asymmetry default:** when the decider call is uncertain, write the lowercase (terrain) form and let approach resolve it — never upgrade a guess to an actor.
- **`?`-rate metric:** observed, never targeted. Report per zone. A `?` that resolves on approach is the system working; the alarm condition is a `?` that stays `?` at decision range, not the raw rate.

## Open questions for the field

1. **Capture technique** — monocular, stereo, lidar, event? Changes the geometry and decider layers. Undecided; the library is capture-agnostic by design.
2. **Context** — does context need a syntax home? (See the `B3` flag in the library's v1.2 changes.) Candidates: a locality-adjacent mark; the frame's own geography (row and neighbors as positional context); or reader judgment, unaided. Field data decides.
3. **Z step-down window** — a field-test parameter by the library's own ruling; measure before setting.

## Candidate resolution on file

- **Occlusion (Q5 in DeepSeek's numbering):** partially occluded, class known, extent unknown needs no new mark. Write the known glyph for the seen part and `?` cells for the hidden extent — the composition is already a partially resolved reading, and the parser can say so. If field data confirms it, this question closes without a library change. (Rowan's composition answer; DeepSeek concurred it beats holding for new syntax.)
