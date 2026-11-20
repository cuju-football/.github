# Cuju

Cuju is a family of open source tools for Google Research Football, one of the richest benchmarks of multi-agent reinforcement learning. The engine reproduces Google Research Football bit for bit and runs thousands of matches at once on a GPU or a CPU, so research that once waited on the simulator can move at the speed of the learner. Around it sits a renderer for watching, playing and recording matches in a browser.

## The packages

| Package | What it does | Install |
| --- | --- | --- |
| [cuju-engine](https://github.com/cuju-football/engine) | The engine. A bit-exact, batched reimplementation of Google Research Football for CUDA and the CPU, with the same states, observations, rewards and done flags as the original for the same seed and actions. The import stays `import cuju`. | `pip install cuju-engine` |
| [cuju-render](https://github.com/cuju-football/render) | The renderer. Watch saved or live matches in the browser, play against the built-in AI or a trained team, export video and data, and follow training as it runs. Its current release works with `cuju` 0.2.1. | `pip install cuju-render` |

Each repository holds its own guides, from a first match to the details of the recording format, and each package keeps the versions of the others it works with in its requirements. This page lists each package once it is released.

## Where to start

New to Cuju, start with the [engine README](https://github.com/cuju-football/engine#readme), which shows a first batch of matches and how results compare with published Google Research Football numbers. To watch a match, the [cuju-render README](https://github.com/cuju-football/render#readme) opens one in a few commands.

Questions and ideas are welcome in the discussions of each repository, and bugs in its issues. Testing is internal, and reports of anything that behaves differently from Google Research Football are especially valued.

## A note on names

Cuju takes its name from the ancient Chinese ball game. It is an independent project, neither affiliated with nor endorsed by Google. Google Research Football is a project of Google Research, and Google is a trademark of Google LLC.
