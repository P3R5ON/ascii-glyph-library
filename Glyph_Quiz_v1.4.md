# Glyph Library v1.4 — Reading Quiz

**For the reader.** Hold only Glyph Library v1.4. Do not rely on earlier versions, other chats, or anything outside that file. Do not add glyphs. If the file gives no ruling, say so, give your best reading, and mark it as a guess. You will not be told whether a reading is right, and you may not ask questions; answer from the file alone.

For every doubt, stamp it in the form the file's Scars section uses: `version · what I read · what the file meant`.

---

## Part A — Strings

Read each string alone. Unless a line says otherwise, assume a frame with a `k` row and `@` on the sidewalk. For each, give **the reading** (or `?`) and **the one rule or table row that decides it**.

1. `Cd1`
2. `Cd2`
3. `K1`
4. `m3`, standing on a foot row
5. `B3`, standing on a foot row
6. `B3`, standing on a road row
7. `s.d`
8. `sD`
9. `sd2`
10. `P1.P2`
11. `F2`
12. `XP0`
13. `w3`
14. `R1`
15. `@2`
16. `%`
17. `G>`

---

## Part B — Frames

For each frame give **A. Parse**: every glyph as `row,column: glyph — reading`, rows counted from 1 at the top and columns from 0 at the left. Skip repeated fence (`|`), curb (`k`) and open-ground (`.`) cells and say so once. Then answer the question under the frame, with your working.

### Frame 1

```
# v1.4 cell=0.5m head=E spd=1 key=0
.....B3......t......
@.P1.......C3.......
kkkkkkkkkkrkkkkkkkkk
..Cd1.......B3......
........b2..........
```

**Question 1.** Which glyphs in this frame read `?`, and why? Which glyph reads as written but stands where it should not, and how far ahead of the agent is its head, in meters?

### Frame 2

```
# v1.4 cell=0.5m head=E spd=1 key=2
@..P1....B3...M3..
...........w2.....
```

**Question 2a.** Which glyph reads `?`, and what single feature of the frame decides it?

**Question 2b.** How far is the `M3` from the agent, head to head, in meters? Does it read as written?

### Frame 3

```
# v1.4 cell=1m head=N spd=3 key=0
....C2....=.....
..........=.....
kkkkkkkkkkrkkkkk
..PP1......p.p..
...@............
```

**Question 3a.** What is directly ahead of the agent in its own column, and how far away is it?

**Question 3b.** How does the header's `spd=3` read for this agent, and why?

### Frame 4

```
# v1.4 cell=0.5m head=W spd=0 key=7
.....ZZZ.......f.
..........@......
```

**Question 4a.** What is directly ahead of the agent along its own row, and how far does the clear ground run? What does the frame say about anything beyond it?

**Question 4b.** At `key=7`, how does a reader treat the `ZZZ`, and what does `key=7` tell the reader about the frame as a whole?

---

## Return format

Part A as a numbered list. Part B as one block per frame: parse, then answers. At the end, list your doubts in stamp form. Do not explain the library back to us.
