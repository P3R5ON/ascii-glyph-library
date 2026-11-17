# Glyph Library v1.3 — Perception by Consequence (DRAFT)

*Scope: the glyphs, what each one does to the agent, an example of each in use, and how to learn more. Nothing else. The definition list below is the contract: if two readers hold it and read a frame differently, add an example until they don't.*

## The floor (the only hard rules)

1. **A glyph names what a thing DOES to the agent**, not what it IS. If two things ask for the same move, they share a glyph.
2. **One character is one cell.** A digit or swing-mark written directly after a glyph belongs to it and takes the next cell.
3. **Digits are speed, only speed:** 0 still, 1 walk, 2 fast, 3 traffic. A thing that can move and carries no digit reads as walking. Stillness is written (`c0`). 3 is the road's own flow: it belongs to the road-class glyphs (see the digit column), and to `b` and `B` only on a road row (see *Context by position*). A 3 anywhere else is a contradiction and reads `?` (rule 4).
4. **`?` means don't guess.** Unclassified, unseen, or unsure: write `?`. A digit on a glyph that cannot carry one — `t2`, a tree at fast — is a contradiction of the same kind: read the whole glyph as `?`, never as a fast tree. The digit column in the definition list says which glyphs can carry one, and how high.
5. **Case asks one question: is a decider engaged?** lowercase = no, the thing as terrain. UPPERCASE = yes, the thing with a decider fused into it. A *decider* is whoever can answer back: a person, a driver, a guard, a system, an event.

Everything else in this file is vocabulary, and vocabulary is allowed to grow.

## The test: what does it fuse?

A true glyph can be said out loud as *this plus that*. `B` is a **person** plus a **bike**: the vector belongs to the bike and the priority belongs to the human, and the shape holds both. `C` is a person in a car, `W` a person behind a cart, `T` a person in a tree, `K` a person at the edge of a curb. In each, the decider is the person inside the glyph, and uppercase is simply the decider fused into the thing.

When a new situation needs a glyph, ask what it fuses. If you can say it, it is probably a glyph. If you can't, it is probably `?`, or it already has a glyph.

**Case reads per letter.** In a two-letter fusion each letter keeps its own case: `sd` is two terrain forms fused; `Cd` is an occupied car fused with a terrain door.

## Definition list

### The world and its actors (fusions of thing + decider)

| glyph | fuses | what it does to the agent | seen as | digit |
|---|---|---|---|---|
| `w` | — | a rolling mass with no one behind it: cart, stroller, loose tire. Yield, offset | `..w0..` a bin standing; `..w1..` rolling free | 0–2 |
| `W` | person + `w` | rolling mass under human hands; slow, wide, wanders | `..W1..` a cart being pushed | 0–2 |
| `c` | — | a full road vehicle as traffic-mass. Never share its lane | `c0` parked | 0–3 |
| `C` | person + `c` | a car with a driver aboard; will signal, can negotiate | `C2` a driver at fast | 0–3 |
| `b` | — | a light, fast, fragile bike vector | `b0` leaned on a wall | 0–2, 3 on a road row |
| `B` | person + `b` | a person on a bike: the vector is the bike's, the priority is the human's | `B1` a rider at walking pace | 0–2, 3 on a road row |
| `m` | — | a motorcycle alone: parked, fallen, unattended | `m0` a fallen machine | 0–3 |
| `M` | person + `m` | a motorcycle with its rider; the living case | `M2` | 0–3 |
| `t` | — | rooted vertical; permanent, may be trusted from one pass to the next | `..t..` | none |
| `T` | person + `t` | a tree with someone in it; what is above can descend | `..T..` | none |
| `g` | — | a barrier whose state can change; state unreported. Read it on approach | `|||g|||` | none |
| `g>` | `g` + opening | the leaf swinging toward open: a passage forming | `|||g>|||` | none |
| `g<` | `g` + closing | the leaf swinging shut: a passage vanishing, a wall becoming | `|||g<|||` | none |
| `G` | decider + `g` | a gate that decides: a guard, a handshake, an authentication. Address it and wait | `|||G|||` | none |
| `k` | — | the step between road-world and foot-world | `kkkkk` | none |
| `K` | person + `k` | an occupied curb: someone at the edge, crossing imminent | `kkKkk` | none |
| `r` | — | a dropped curb, the legal crossing | `kkrkk` | none |
| `R` | person + `r` | a ramp in use: the lane is theirs | `kkRkk` | none |
| `s` | — | stairs: a wall lying about being a floor | `ss` | none |
| `S` | person + `s` | occupied stairs: actors the agent can't follow; their vectors arrive at its foot | `sSs` | none |
| `d` | — | a door; a delivery interface, a hand-off point | `|d|` | none |
| `D` | decider + `d` | a door that decides: a person in the doorway, a locker that authenticates | `|D|` | none |
| `o` | — | debris beneath naming; transient, re-read every pass | `..o..` | none |
| `O` | agent + `o` | a downed agent: obstacle in shape, actor in standing. Never read as debris | `..O..` | none |
| `h` | — | glass, sharp scatter, slick: damage at rest | `hhh` | none |
| `H` | decider + `h` | a hazard being driven: sprayer, welder, sweeper. The damage is aimed | `H1` a sweeper | 0–2 |
| `p` | — | a person as mass: counted, not yet reckoned with; the distant figure, the crowd cell | `ppp` a crowd | 0–2 |
| `P` | `p` + resolved | a person in range: vector resolved, rights engaged. Yield always | `P1` | 0–2 |
| `a` | — | ambient wildlife: squirrel, bird. Counted, flowed past | `a2` | 0–2 |
| `A` | `a` + decider | an animal in range, dog-class: small, fast, erratic | `A2` | 0–2 |
| `f` | — | one wrong cell: cracked tile, dead patch. Noted, flowed over | `..f..` | none |
| `F` | `f` + event | an anomaly in progress: dense, dynamic, unresolved | `FFF` | none |
| `z` | — | a locality: a named region, inert context | `zzzz` | none |
| `Z` | `z` + decider | a flagged zone: the place has become an actor in every reading of its cells | `ZZZZ` | none |

`Z` steps down by silence (`Z` → `F` → `z`) and snaps back on a fresh `F`. How fast it steps is not a matter of syntax. A frame carries one age, `key`, for the whole picture and none for individual glyphs, so aging a `Z` is the writer's job and never the reader's: the pipeline steps a `Z` down before it writes the frame, and a reader takes every `Z` as current. The window is a field-test parameter, not syntax.

### Fusions

| glyph | fuses | what it does to the agent | seen as | digit |
|---|---|---|---|---|
| `PA` | person + animal | the leash unit: one body with an invisible radius | `PA` / `PA2` | 0–2 |
| `PP` | person + person | a linked pair: couple, escort, adult and child | `PP1` | 0–2 |
| `sd` | stairs + door | **a lift.** Stairs are a wall to wheels; a door is a hand-off; together, a way through the wall. Pass when it opens | `|||sd|||` | none |
| `sD` | stairs + deciding door | a lift that authenticates: keycard, call button, an attendant | `|||sD|||` | none |
| `Cd` | driver car + door | **a car with its door open.** Someone is about to enter the lane edge. Give the door its swing | `Cd0` | 0–3 |
| `XP` | destination + person | **the handoff is live:** someone is waiting at the destination. Approach to give, not to leave | `XP0` | 0–2 |

Any two glyphs that would form a listed fusion but are *not* fused — merely neighbors in adjacent cells — are written with a `.` between them. Stairs beside a door that is not a lift is `s.d`, not `sd`; two people standing near each other who are not a linked pair are `P.P`, not `PP`.

A digit after a fusion binds the whole body: `PA2` — the pair moves at fast. If the members move at different speeds, they are not one body in that moment: write them unfused (`P2.A1`).

A mark inside a fusion is a component like any other: `XP0` is the live handoff, still. The digit binds the whole fusion; the marks' "no digits" rule applies to bare marks, not to marks fused into a body.

The rule holds for glyph-class fusions too, and the digit column decides: `Cd1` and `PA2` are lawful; `sd` and `sD` carry none, because stairs and a door cannot move (a lift cab's vertical travel is not ground speed in a plan view), so `sd2` and `sD1` read `?`.

### Marks (no case, no digits)

| mark | what it is | seen as |
|---|---|---|
| `@` | self, the agent. Heading is given in the header | `..@..` |
| `+` | a decision point: intersection, alley mouth, lane choice | `.+.` |
| `X` | the destination | `dX` the door, then the destination |
| `.` | open ground: observed, clear, nothing to answer to | `.....` |
| `?` | don't guess: unclassified or unseen. Slow reading | `.?.` |

### Drawn glyphs (the shape is the meaning; no case, no digits)

| glyph | draws | means | seen as |
|---|---|---|---|
| `\|` | a paling | fence / wall; repeat for length | `|||||` |
| `/` | rising ground | slope up | `///` |
| `\` | falling ground | slope down | `\\\` |
| `^` | a rise | step-up, speed bump, lip | `..^..` |
| `v` | a dip | pothole, drain dip, a wheel trap | `..v..` |
| `~` | water | puddle, spill; `~~~` deep enough to read as wall | `~~~` |
| `=` | painted stripes | a painted crossing across the road; the agent may share the road here, and `P` has priority | `=` stacked down the road rows |

## One note, not a glyph

**A walk signal is a gate with no hinge.** It does the same thing to the agent as `g`, so it is written `g`, `g>` or `g<`. This is the rule *one glyph per consequence* at work.

## Context by position

The format already carries one kind of context: geography. A `k` row is the curb line. Rows on the road side of it are **road rows**; rows on the sidewalk side are **foot rows**. With the agent `@` on the sidewalk (the ordinary case), the road side is the side of the `k` row that does not hold `@`.

This is what decides `b` and `B` at 3: `B3` on a road row is a cyclist moving as the road's own flow, and reads true. `B3` on a foot row is the `t2` contradiction, and reads `?`. A frame with no `k` row has no road context, so a `b` or `B` carrying 3 reads `?`.

**Open, flagged for the log:** the agent crossing. With `@` standing on a road row, or on `=`, the sidewalk side is ambiguous. Field data will say whether the header needs a field for it (`road=S`) or whether reader judgment covers it.

## A frame, written out

The header is optional, but it keeps old and new frames from being mixed up. `head` is the direction `@` faces; `spd` is the agent's own speed digit, same scale and same rules as any other (0 still, 1 walk, 2 fast, 3 traffic, and 3 is a contradiction for an agent on the sidewalk); `key` is the frame's age in ticks since the last full-resolution baseline (keyframe), and `key=0` means this frame is a baseline. `key` changes no glyph's meaning. It says how far to trust the picture, and when to refresh is the pipeline's call, not the reader's. A frame with no `key` has an unknown age. N is the top row, E is the right.

```
# v1.3 cell=0.5m head=E spd=1 key=0
....t......dX.........
|||||||||g>|||||||||||
..@....PA......t......
kkkkkkkkkkkrkkkkkkkkkk
......C2........B1....
```

A second frame using the integrated fusions:

```
# v1.3 cell=0.5m head=E spd=1 key=3
||||sd||||||||||
....XP0.........
..@.............
kkkkkkkkkkkkkkkk
..C2....=.......
........=.......
```

Reading the second: the agent is on the sidewalk, facing east; a lift sits in the fence line and opens straight onto the destination, where someone is already waiting; in the road, a driver at fast speed approaches a painted crossing. With `key=3`, the picture is three ticks past its last baseline.

## Learning the library

1. **Learn the pairs.** Every thing has a terrain form and an actor form. Hold both or hold neither.
2. **Ask what it fuses.** A new glyph earns its place when you can say what it is made of and what it does to the agent that no other glyph does.
3. **One glyph per consequence.** If it demands the same move as an existing glyph, it is that glyph.
4. **Leave `?` honest.** A library that guesses to look complete will eventually guess at the one cell that mattered.
5. **Agreement is the test.** When independent readers parse the same frame the same way, the path is true. When they differ, that is information about the glyph. Add a definition or an example, don't pick a winner.

## Scars

Known ways this file has misled a reader. A reader who meets a new one stamps a line in the same form: `reader · version · what I read · what the file meant`. A stamped error is a key to the library: it shows where the words fell short of the pattern.

- **Table pipes.** Rows whose examples contain `|` (`|||g|||`, `|d|`) may render with broken cells in some markdown viewers, because the pipes split the cell. The raw text is correct. The pipes are left unescaped on purpose: `\|` would put a `\`, the slope-down glyph, into the example.
- **`sd2` and `sD1` (v1.2).** The file offered a digit on a lift while rule 4 said a lift's components cannot take one. v1.3 withdrew the examples. If a digit on a fixed glyph ever looks lawful, trust the digit column and not the example.

## Changes in v1.3

Drafted by Claude from a read of v1.2, for Rowan to integrate or throw out. Seven edits; the digit column and the position rule carry rulings that need ratifying:

- **A digit column joins the definition list.** v1.2's rules 3 and 4 depended on "cannot move" and "road-class" without saying which glyphs those were. The column now says, per glyph, which digits it can carry: `none`, `0–2`, `0–3` (road-class: `c`, `C`, `Cd`, `m`, `M`) or `0–2, 3 on a road row` (`b`, `B`). *To ratify:* `o`, `O`, `K`, `R`, `T` and `F` are all `none`. An anomaly that travels is not an `F`; it is a `?` until it is classified.
- **`sd2` and `sD1` are withdrawn.** Stairs and a door cannot move, so under rule 4 those strings read `?`. The fusion-digit paragraph now says the digit column decides.
- **The stale `Z` rule moves to the writer.** A frame has no ages, so a reader cannot apply it. The pipeline steps `Z` down before writing the frame.
- **The `B3` question is answered by position.** A new section, *Context by position*, reads road rows and foot rows from the `k` line. The agent-crossing case is left open and flagged.
- **The header example shows `spd`.** Both frames now carry `spd=1`, and `spd` follows the same digit rules as any other digit.
- **The header gains `key`.** It is the frame's age in ticks since the last full-resolution baseline, so an agent can see how stale its picture is and the pipeline can set the refresh threshold. Proposed by the project's author. The name means *keyframe* here, and nothing else in the file uses the word.
- **A Scars section joins the file.** It holds the table-pipe rendering warning and the `sd2` misread, and gives readers a one-line form for stamping their own errors.

## Changes in v1.2

Drafted by DeepSeek in the chorus relay and integrated by Rowan into the v1.1 body (DeepSeek's export carried the front matter; the learning rules and changes ladder were restored from v1.1 so nothing constitutional was lost in transit). Five edits:

- Rule 3: digit 3 is restricted to road-class things; a non-road glyph carrying 3 is a contradiction and reads `?`. **Open, flagged for the log:** the `B3` boundary. DeepSeek's read, offered as an example not a ruling: a cyclist is road-class when the road is treating them as flow — `B3` beside a bike lane reads true; `B3` on a sidewalk is the `t2` contradiction again. Which suggests the fence is not on the glyph but on the context, and the library has no syntax for context: **open, and possibly a context question wearing a glyph's clothes.** Field data will say whether context needs a home (a locality-adjacent mark?) or reader judgment covers it. Rowan's counter-note for the same list: the frame's geography may already carry context — a glyph's row and neighbors (road row vs sidewalk row) are positional context the format has never named.
- A reader holding a stale `Z` treats it as `F` or `z` until refreshed; the step-down window is a field-test parameter, not syntax.
- A mark inside a fusion is a component like any other: the digit binds the whole fusion (`XP0`); the marks' "no digits" rule governs bare marks only.
- Glyph-class fusions take digits under the same law (`sd2`, `sD1`); a component that cannot take a speed makes the digit a contradiction (rule 4).
- The frame header gains `spd`, the agent's own speed digit.

## Changes in v1.1

One line, grown from the blind reading test: floor rule 4 now carries its example — a digit on a thing that cannot move (`t2`) reads as `?` whole. The test's reader found the contradiction but hedged the resolution; the key ruled rule 4 already decides it. The example is added so the next reader doesn't have to re-derive it, per learning rule 5: disagreement is information about the glyph — add an example.

## Changes in v1.0

Finalized by Rowan, on three fixes caught by Claude's read of v0.9:

- The fusion table's markdown is repaired (a blank line had split it; the `sd`, `sD`, `Cd` and `XP` rows now render under their header).
- The `.` separator rule is generalized: any adjacent glyphs that would accidentally form a listed fusion are written with `.` between them (`s.d` is not a lift).
- The second frame's introduction no longer calls the fusions "proposed"; they are integrated canon.

## Changes from v0.8

- Rowan's review accepted all five of Claude's proposals; they are integrated above: `sd` and `sD` (the lift), `Cd` (car with door open), `XP` (live handoff), `=` (painted crossing, drawn class).
- Fusion digit-binding stated with its example: a digit after a fusion binds the whole body (`PA2`); differing speeds are written unfused.
- The walk-signal note kept as a standing note (it is the one-glyph-per-consequence rule at work, not a glyph).
- Unchanged: the floor (five rules), the definition list, the frame format, the learning rules.

## Changes from v0.7

- The hard rules shrink to five. The reserved-letter list, the invalid-cell rule, the greedy-parse rule and the mandatory version check are dropped. Readers who hit something unlisted write `?`.
- Each glyph now carries a fusion and an example string.
- Case reads per letter, which makes mixed fusions like `Cd` and `sD` lawful.
- New proposals: `sd`, `sD`, `Cd`, `XP`, `=`.
- Unchanged from v0.7: `f`/`F` for the fault pair (`!` retired), `.` for open ground, `PA` and `PP`.

*The old marks worked this way: a stroke was a tree, a tally was a count, a paling was a fence.*
