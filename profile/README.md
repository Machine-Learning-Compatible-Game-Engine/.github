# Machine Learning Compatible Game Engine

Experimental graphics, simulation, editor, and game-engine prototypes built around C++, OpenGL, Python, PyQt, mathematical visualization, and future ML-agent-compatible simulation interfaces.

This organization collects the research trail behind a custom game-engine direction: small visual sketches, C++/OpenGL render loops, FreeGLUT experiments, PyQt editor tooling, mathematical visualizations, raycasting prototypes, and early reusable game-object abstractions.

The current repositories are **research prototypes**, not production-ready engines. The long-term direction is to move from visual/game-engine experiments toward deterministic simulation interfaces that can eventually expose state, actions, observations, rewards, telemetry, replay, and Python integration for machine-learning agents.

---

## Current focus

| Area                      | Repositories                                 | Purpose                                                                             |
| ------------------------- | -------------------------------------------- | ----------------------------------------------------------------------------------- |
| Engine core               | `supEngine`                                  | Focused C++/FreeGLUT engine prototype with primitives, game objects, and components |
| Full research suite       | `full-suite`                                 | Broad PyQt/editor/C++/OpenGL prototype suite                                        |
| Creative C++ sketches     | `p5GL`                                       | p5.js-like sketch framework idea in C++/FreeGLUT                                    |
| Renderer research         | `abstract-template-for-opengl-render-engine` | OpenGL abstractions, buffers, shaders, textures, and ImGui experiments              |
| Raycasting/game prototype | `DoomCloneBuilder`                           | Doom-like raycasting and maze-rendering experiment                                  |
| Study notebook            | `sketchbook`                                 | Curated interactive lessons built from older graphics/math experiments              |

---

## Featured repositories

### `full-suite`

The broadest research prototype in the organization. It combines a PyQt project hub/editor direction, OpenGL scene view experiments, C++ engine pieces, sample projects, and hardware/serial interaction ideas.

Status: research prototype. Needs cleanup, reproducible setup, and clearer architecture documentation.

### `supEngine`

A focused C++/FreeGLUT engine-core candidate. It explores vector math, colors, render primitives, game objects, components, input codes, and simple example projects.

Status: promising engine-core prototype. Needs README, build instructions, API overview, and roadmap.

### `p5GL`

A bridge between creative-coding style and C++/OpenGL. It experiments with a `setup()` / loop-style sketch architecture inspired by p5.js, but implemented in C++/FreeGLUT.

Status: useful conceptual predecessor to later engine work.

### `abstract-template-for-opengl-render-engine`

OpenGL rendering research with abstractions around shaders, buffers, textures, vertex arrays, layouts, and ImGui-style experiments.

Status: renderer research prototype.

### `DoomCloneBuilder`

A 2D raycasting / Doom-like maze prototype using C++ and GLUT-style rendering.

Status: game/simulation learning prototype.

### `sketchbook`

A studyable technical notebook built from historical visualization repositories.

It contains:

* preserved source imports under `sources/`;
* curated learning chapters under `notebook/`;
* inline browser visualizers;
* p5.js demos;
* C++/OpenGL/GLUT static-web strategy notes;
* PyQt/editor-tooling explanations;
* safe documentation around C++ execution on the web.

This is the best entry point for understanding the smaller experiments.

---

## Long-term ML-compatible direction

The organization name points to a future goal: making game-engine or simulation environments easier to connect to machine-learning agents.

That direction requires work that is not fully implemented yet:

* deterministic simulation loop;
* state serialization;
* action/input abstraction;
* observation interface;
* reward interface;
* telemetry export;
* replay system;
* Python bindings or IPC bridge;
* sample random/heuristic/ML agents;
* reproducible scenarios.

Until those layers exist, this organization should be read as a **graphics, simulation, editor, and engine-prototype lab moving toward ML compatibility**, not as a completed ML engine.

---

## Repository status model

| Status            | Meaning                                                                 |
| ----------------- | ----------------------------------------------------------------------- |
| Active prototype  | Still useful as a development target                                    |
| Study source      | Historical repo preserved through `sketchbook`                          |
| Research archive  | Valuable for history, but not active                                    |
| Needs cleanup     | Public but requires README/build/security/provenance cleanup            |
| Private/reference | Too noisy, duplicated, or provenance-sensitive for public portfolio use |

---

## Public-facing roadmap

1. Polish `sketchbook` as the learning and visual index.
2. Clean `supEngine` into the focused engine-core repository.
3. Clean `full-suite` into a documented research suite.
4. Clarify `p5GL` as the creative-coding bridge.
5. Add screenshots, diagrams, and build instructions to public repos.
6. Define the first ML-compatible simulation API.
7. Add a minimal Python agent bridge.
8. Build one reproducible agent-ready demo environment.

---

## Design principle

Small experiments are not failures. They are preserved as stepping stones:

```text
math sketch → rendering experiment → engine primitive → editor tool → simulation interface → agent-compatible environment
```

This organization documents that path.
