---
title: "qMuVi: <b>q</b>uantum <b>Mu</b>sic <b>Vi</b>deo tool"
layout: post
date: 2022-07-12 17:00
image: /assets/images/qmuvi-logo-white-middle.png
headerImage: false
projects: true
hidden: true
description: "An open-source Python library that turns quantum circuits into music videos. It won 1st place at the Qiskit Hackathon Melbourne 2022 and is now part of the IBM Qiskit Ecosystem."
category: project
externalLink: false
---

<figure class="post-figure">
  <img src="/assets/images/qmuvi-frame.webp" alt="A frame from a qMuVi video showing a 4-qubit circuit above bar charts of basis-state probabilities, a fidelity gauge and a phase colour wheel">
  <figcaption>A frame from a qMuVi video. The circuit runs along the top, the bar charts show the probability of each basis state, colours show phase, and the gauge on the right tracks fidelity.</figcaption>
</figure>

qMuVi is an open-source Python library that turns [Qiskit](https://www.ibm.com/quantum/qiskit) quantum circuits into music videos. It's available on [PyPI](https://pypi.org/project/qmuvi/) and is part of the [IBM Qiskit Ecosystem](https://www.ibm.com/quantum/ecosystem).

Quantum computing is notoriously unintuitive and hard to picture. qMuVi tries to connect a human observer to what's happening inside a quantum computation. By turning circuits into music videos, it lets you "hear" and "see" how a quantum state evolves as an algorithm runs.

<div class="video">
  <iframe src="https://www.youtube-nocookie.com/embed/seersj3W-hg" title="Making music with quantum computation: qMuVi showcase" loading="lazy" allow="accelerometer; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### How it works

- **Sampling the state.** Barrier gates in your circuit mark where qMuVi takes a snapshot of the quantum state. It simulates the circuit with Qiskit Aer, optionally with a noise model, so you can hear how noise changes the result.
- **States become notes.** Each basis state is mapped to a musical note, and its probability sets how loud it plays. Note maps range from chromatic to C major, F minor and arpeggios, or you can write your own.
- **Phase picks the instrument.** A noisy state is split into pure states, each of which gets its own collection of instruments. The phase of each basis state then chooses the instrument within that collection.
- **Output.** qMuVi renders an MP4 music video, along with MIDI and WAV files of the soundtrack.

### Try it

```bash
pip install qmuvi
```

```python
import qmuvi
from qiskit import QuantumCircuit

circ = QuantumCircuit(2)
# barriers tell qMuVi where to sample the state
circ.barrier()
circ.h(0)
circ.barrier()
circ.cx(0, 1)
circ.barrier()

qmuvi.generate_qmuvi(circ, "bell_state")
```

This generates a music video of a Bell state being prepared. There are more examples, and the videos they produce, in the [GitHub repository](https://github.com/garymooney/qmuvi), and full [documentation](https://garymooney.github.io/qmuvi) is online.

### Origins

<figure class="post-figure">
  <img class="post-photo" src="/assets/images/qiskit-hackathon-melbourne-2022-winners.jpg" alt="The qMuVi team with their hackathon award" loading="lazy">
  <figcaption>The qMuVi team at the Qiskit Hackathon Melbourne 2022. From left to right: Yang Yang, me, Harish Vallury and Gan Yu Pin.</figcaption>
</figure>

qMuVi was created for the [IBM Qiskit Hackathon Melbourne 2022](https://github.com/quantum-melbourne/qiskit-hackathon-22), where it won first place from the judges and the community vote. I was the team lead. The project was featured on the [IBM Qiskit Blog](https://medium.com/qiskit/turning-quantum-states-into-music-at-australias-first-ever-qiskit-hackathon-25da7f09d226), and I've continued developing it since.

### Built with

Python, Qiskit and Qiskit Aer, matplotlib, MoviePy, mido for MIDI, and TiMidity++ for audio synthesis.
