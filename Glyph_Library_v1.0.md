# Glyph Library v1.0 — Perception by Consequence (DRAFT)

*Scope: the glyphs, what each one does to the agent, an example of each in use, and how to learn more. Nothing else. The definition list below is the contract: if two readers hold it and read a frame differently, add an example until they don't.*

## The floor (the only hard rules)

1. **A glyph names what a thing DOES to the agent**, not what it IS. If two things ask for the same move, they share a glyph.
2. **One character is one cell.** A digit or swing-mark written directly after a glyph belongs to it and takes the next cell.
3. **Digits are speed, only speed:** 0 still, 1 walk, 2 fast, 3 traffic. A thing that can move and carries no digit reads as walking. Stillness is written (`c0`).
4. **`?` means don't guess.** Unclassified, unseen, or unsure: write `?`.
5. **Case asks one question: is a decider engaged?** lowercase = no, the thing as terrain. UPPERCASE = yes, the thing with a decider fused into it. A *decider* is whoever can answer back: a person, a driver, a guard, a system, an event.

Everything else in this file is vocabulary, and vocabulary is allowed to grow.

## The test: what does it fuse?

A true glyph can be said out loud as *this plus that*. `B` is a **person** plus a **bike**: the vector belongs to the bike and the priority belongs to the human, and the shape holds both. `C` is a person in a car, `W` a person behind a cart, `T` a person in a tree, `K` a person at the edge of a curb. In each, the decider is the person inside the glyph, and uppercase is simply the decider fused into the thing.

When a new situation needs a glyph, ask what it fuses. If you can say it, it is probably a glyph. If you can't, it is probably `?`, or it already has a glyph.

**Case reads per letter.** In a two-letter fusion each letter keeps its own case: `sd` is two terrain forms fused; `Cd` is an occupied car fused with a terrain door.

## Definition list

### The world and its actors (fusions of thing + decider)

| glyph | fuses | what it does to the agent | seen as |
|---|---|---|---|
| `w` | — | a rolling mass with no one behind it: cart, stroller, loose tire. Yield, offset | `..w0..` a bin standing; `..w1..` rolling free |
| `W` | person + `w` | rolling mass under human hands; slow, wide, wanders | `..W1..` a cart being pushed |
| `c` | — | a full road vehicle as traffic-mass. Never share its lane | `c0` parked |
| `C` | person + `c` | a car with a driver aboard; will signal, can negotiate | `C2` a driver at fast |
| `b` | — | a light, fast, fragile bike vector | `b0` leaned on a wall |
| `B` | person + `b` | a person on a bike: the vector is the bike's, the priority is the human's | `B1` a rider at walking pace |
| `m` | — | a motorcycle alone: parked, fallen, unattended | `m0` a fallen machine |
| `M` | person + `m` | a motorcycle with its rider; the living case | `M2` |
| `t` | — | rooted vertical; permanent, may be trusted from one pass to the next | `..t..` |
| `T` | person + `t` | a tree with someone in it; what is above can descend | `..T..` |
| `g` | — | a barrier whose state can change; state unreported. Read it on approach | `|||g|||` |
| `g>` | `g` + opening | the leaf swinging toward open: a passage forming | `|||g>|||` |
| `g<` | `g` + closing | the leaf swinging shut: a passage vanishing, a wall becoming | `|||g<|||` |
| `G` | decider + `g` | a gate that decides: a guard, a handshake, an authentication. Address it and wait | `|||G|||` |
| `k` | — | the step between road-world and foot-world | `kkkkk` |
| `K` | person + `k` | an occupied curb: someone at the edge, crossing imminent | `kkKkk` |
| `r` | — | a dropped curb, the legal crossing | `kkrkk` |
| `R` | person + `r` | a ramp in use: the lane is theirs | `kkRkk` |
| `s` | — | stairs: a wall lying about being a floor | `ss` |
| `S` | person + `s` | occupied stairs: actors the agent can't follow; their vectors arrive at its foot | `sSs` |
| `d` | — | a door; a delivery interface, a hand-off point | `|d|` |
| `D` | decider + `d` | a door that decides: a person in the doorway, a locker that authenticates | `|D|` |
| `o` | — | debris beneath naming; transient, re-read every pass | `..o..` |
| `O` | agent + `o` | a downed agent: obstacle in shape, actor in standing. Never read as debris | `..O..` |
| `h` | — | glass, sharp scatter, slick: damage at rest | `hhh` |
| `H` | decider + `h` | a hazard being driven: sprayer, welder, sweeper. The damage is aimed | `H1` a sweeper |
| `p` | — | a person as mass: counted, not yet reckoned with; the distant figure, the crowd cell | `ppp` a crowd |
| `P` | `p` + resolved | a person in range: vector resolved, rights engaged. Yield always | `P1` |
| `a` | — | ambient wildlife: squirrel, bird. Counted, flowed past | `a2` |
| `A` | `a` + decider | an animal in range, dog-class: small, fast, erratic | `A2` |
| `f` | — | one wrong cell: cracked tile, dead patch. Noted, flowed over | `..f..` |
| `F` | `f` + event | an anomaly in progress: dense, dynamic, unresolved | `FFF` |
| `z` | — | a locality: a named region, inert context | `zzzz` |
| `Z` | `z` + decider | a flagged zone: the place has become an actor in every reading of its cells | `ZZZZ` |

`Z` steps down by silence (`Z` → `F` → `z`) and snaps back on a fresh `F`. How fast it steps is not a matter of syntax.

### Fusions

| glyph | fuses | what it does to the agent | seen as |
|---|---|---|---|
| `PA` | person + animal | the leash unit: one body with an invisible radius | `PA` / `PA2` |
| `PP` | person + person | a linked pair: couple, escort, adult and child | `PP1` |
| `sd` | stairs + door | **a lift.** Stairs are a wall to wheels; a door is a hand-off; together, a way through the wall. Pass when it opens | `|||sd|||` |
| `sD` | stairs + deciding door | a lift that authenticates: keycard, call button, an attendant | `|||sD|||` |
| `Cd` | driver car + door | **a car with its door open.** Someone is about to enter the lane edge. Give the door its swing | `Cd0` |
| `XP` | destination + person | **the handoff is live:** someone is waiting at the destination. Approach to give, not to leave | `XP0` |

Any two glyphs that would form a listed fusion but are *not* fused — merely neighbors in adjacent cells — are written with a `.` between them. Stairs beside a door that is not a lift is `s.d`, not `sd`; two people standing near each other who are not a linked pair are `P.P`, not `PP`.

A digit after a fusion binds the whole body: `PA2` — the pair moves at fast. If the members move at different speeds, they are not one body in that moment: write them unfused (`P2.A1`).

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

## A frame, written out

The header is optional, but it keeps old and new frames from being mixed up. `head` is the direction `@` faces; N is the top row, E is the right.

```
# v1.0 cell=0.5m head=E
....t......dX.........
|||||||||g>|||||||||||
..@....PA......t......
kkkkkkkkkkkrkkkkkkkkkk
......C2........B1....
```

A second frame using the integrated fusions:

```
# v1.0 cell=0.5m head=E
||||sd||||||||||
....XP0.........
..@.............
kkkkkkkkkkkkkkkk
..C2....=.......
........=.......
```

Reading the second: the agent is on the sidewalk, facing east; a lift sits in the fence line and opens straight onto the destination, where someone is already waiting; in the road, a driver at fast speed approaches a painted crossing.

## Learning the library

1. **Learn the pairs.** Every thing has a terrain form and an actor form. Hold both or hold neither.
2. **Ask what it fuses.** A new glyph earns its place when you can say what it is made of and what it does to the agent that no other glyph does.
3. **One glyph per consequence.** If it demands the same move as an existing glyph, it is that glyph.
4. **Leave `?` honest.** A library that guesses to look complete will eventually guess at the one cell that mattered.
5. **Agreement is the test.** When independent readers parse the same frame the same way, the path is true. When they differ, that is information about the glyph. Add a definition or an example, don't pick a winner.

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
