# EntangleMint

> **Build a circuit. Watch the state change.**

EntangleMint is an interactive four-qubit quantum circuit simulator that lets you
experiment with quantum gates and see the resulting state update in real time.
It is designed as a visual, approachable way to explore superposition,
measurement, probability amplitudes, and entanglement directly in the browser.

## Live demo

**[Open EntangleMint](https://soham-santra.github.io/EntangleMint/)**

## Features

- Simulate a four-qubit pure state in the browser
- Apply common single-qubit gates, including H, X, Y, Z, S, T, phase, rotation,
  measurement, and reset operations
- Add and rearrange gates on circuit tracks with click or drag and drop
- Apply two-qubit CNOT gates
- Load a ready-made Bell state circuit
- View measurement probabilities and the current state vector
- Inspect entanglement and a Bloch sphere visualization
- Save and load circuits as JSON
- Export the circuit view as a PNG image

## How it works

The simulator calculates the state vector using JavaScript complex-number
operations and gate matrices. Each operation is applied to the current
four-qubit state, then the state is normalized before the readouts are updated.
No backend or build step is required.

## Run locally

Because EntangleMint is a static page, it can be opened directly in a browser.
For a local web server, run any static server from the project directory, for
example:

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>.

## Project structure

```text
.
├── index.html                 # Application markup, styles, and simulator logic
├── quantum-circuit.png        # Example circuit image
└── quantum-lab-circuit.json   # Example saved circuit
```

## License

No license has been specified yet.
