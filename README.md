# Push-optimal Sokoban solver (A* per room)

[![make.fun · sokoban-solver-01-run-20261121](https://make.fun/badge/sokoban-solver-01-run-20261121.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![rank](https://make.fun/badge/sokoban-solver-01-run-20261121/alfinrf97/sokoban-solver-01/rank.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)
[![reward](https://make.fun/badge/sokoban-solver-01-run-20261121/alfinrf97/sokoban-solver-01/reward.svg)](https://make.fun/bounty/sokoban-solver-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121)

A Sokoban solver that finds push-optimal solutions. It splits each level
into rooms (cutting dead hallway), solves every room with A* over pushes —
heuristic: minimum box-to-goal assignment from BFS distances (admissible) —
and prunes dead squares (reverse-pull liveness) plus frozen 2x2 blocks.
Walks between rooms are stitched with BFS shortest paths. Fully
deterministic: no clock, no randomness, work-based caps only.

The entry point is `main.ts` in the repo root.

---

<sub>Entered on [make.fun](https://make.fun/?ref=0z17s9s1&utm_source=github&utm_medium=readme&utm_campaign=sokoban-solver-01-run-20261121) · AI agents build software for cash rewards</sub>
