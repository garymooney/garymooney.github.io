---
title: Research
layout: page
---
I'm a research fellow in quantum computing at the University of Melbourne. My work focuses on three areas:

- **Benchmarking quantum hardware:** measuring how much entanglement today's devices can generate and preserve.
- **Quantum circuit compilation:** routing and mapping circuits onto real hardware so they run with fewer errors.
- **Quantum optimisation:** applying quantum and quantum-inspired algorithms to real problems, including work with Ford Motor Company on automotive manufacturing.

I've run experiments on both superconducting (IBM Quantum) and ion-trap (Quantinuum) hardware. I also help run the [IBM Quantum Hub](https://www.unimelb.edu.au/quantumhub) at the University of Melbourne. My full publication list is on [Google Scholar](https://scholar.google.com/citations?user={{ site.google-scholar }}).

<figure class="research-figure">
  <img src="/assets/images/aqc_graphic-topdown.webp" alt="Particle visualisation of a complete graph embedded onto a quantum annealing architecture" loading="lazy">
  <figcaption><b>Fig.</b> "Optimal embedding of a complete graph onto a quantum annealing architecture with nearest-neighbour couplings", my entry in the <a href="https://www.cqc2t.org/">CQC2T</a> Quantum Graphics Competition (2018). It shows a modified simulated annealing algorithm I wrote during my master's degree, rendered with Unity's Visual Effect Graph particle systems. Each cluster of connected nodes is drawn in one colour. The goal is to colour the clusters so that every coloured cluster connects to every other one, using as few nodes as possible.</figcaption>
</figure>

## Highlights

- **5 world records** for large-scale entanglement detection, up to 414 qubits, across a 6-paper benchmarking programme, [featured on the IBM Research Blog](https://research.ibm.com/blog/whole-device-entanglement).
- **Industry collaboration with Ford Motor Company** on quantum optimisation for automotive manufacturing (2 papers).
- **Quantum-inspired optimisation heuristic** for the binary paint shop problem that is competitive with state-of-the-art heuristics on up to 8,192 nodes.
- **Qubit routing algorithm** for circuit compilation that beats the state of the art on both runtime and fidelity.
- **Up to 50% lower** fault-tolerant gate synthesis costs by using the full Clifford hierarchy.
- **Invited talks** at the IBM Quantum Summit (New York, 2023) and the IPAM workshop at UCLA (2023).
- **Teaching and supervision:** lecturer for MULT90063 *Introduction to Quantum Computing*, and co-supervisor of 3 MSc students through to completion.

## Selected publications

**Entanglement benchmarking and teleportation**

- Kang, Kam, **Mooney**, Hollenberg. [Entanglement teleportation along a regenerating hamster-wheel graph state](https://www.nature.com/articles/s41598-025-30301-0), *Scientific Reports* (2025)<br>
  <span class="summary">Teleports an entangled state around a reusable ring of qubits on Quantinuum hardware, travelling further than the device has qubits.</span>
- Kang, Kam, **Mooney**, Hollenberg. [Teleporting two-qubit entanglement across 19 qubits on a superconducting quantum computer](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.23.014057), *Physical Review Applied* (2025)
- Kam, Kang, Hill, **Mooney**, Hollenberg. [Characterization of entanglement on superconducting quantum computers of up to 414 qubits](https://link.aps.org/doi/10.1103/PhysRevResearch.6.033155), *Physical Review Research* (2024)<br>
  <span class="summary">Entangles every active qubit on 22 IBM devices, including all 414 active qubits of the 433-qubit Osprey processor.</span>
- **Mooney**, White, Hill, Hollenberg. [Whole-device entanglement in a 65-qubit superconducting quantum computer](https://onlinelibrary.wiley.com/doi/10.1002/qute.202100061), *Advanced Quantum Technologies* (2021)
- **Mooney**, White, Hill, Hollenberg. [Generation and verification of 27-qubit Greenberger-Horne-Zeilinger states in a superconducting quantum computer](https://iopscience.iop.org/article/10.1088/2399-6528/ac1df7), *Journal of Physics Communications* (2021)
- **Mooney**, Hill, Hollenberg. [Entanglement in a 20-qubit superconducting quantum computer](https://www.nature.com/articles/s41598-019-49805-7), *Scientific Reports* (2019)<br>
  <span class="summary">Shows that an entire 20-qubit IBM device can be entangled; my most-cited paper.</span>

**Quantum optimisation (with Ford)**

- **Mooney**, Villanueva, Radhan, Ghosh, Hill, Hollenberg. [Optimization-free recursive QAOA for the binary paint shop problem](https://journals.aps.org/prresearch/abstract/10.1103/xv79-w3rs), *Physical Review Research* (2026)<br>
  <span class="summary">Skips QAOA's costly parameter-optimisation loop without losing solution quality, on a real car-manufacturing scheduling problem.</span>
- Villanueva, **Mooney**, Radhan, Ghosh, Hill, Hollenberg. [Hybrid quantum optimization in the context of minimizing traffic congestion](https://arxiv.org/abs/2504.08275), arXiv (2025, accepted)

**Compilation and fault tolerance**

- **Mooney**. [Adaptable weighted token swapping algorithm for optimal multi-qubit pathfinding](https://arxiv.org/abs/2405.18785), arXiv (2024, under review)
- **Mooney**, Hill, Hollenberg. [Cost-optimal single-qubit gate synthesis in the Clifford hierarchy](https://quantum-journal.org/papers/q-2021-02-15-396/), *Quantum* (2021)
- **Mooney**, Tonetto, Hill, Hollenberg. [Mapping NP-hard problems to restricted adiabatic quantum architectures](https://arxiv.org/abs/1911.00249), arXiv (2019)

**Quantum machine learning and characterisation**

- Ma, **Mooney**, Petersen, Hollenberg, Dong. [Quantum autoencoders using mixed reference states](https://www.nature.com/articles/s41534-024-00872-3), *npj Quantum Information* (2024)
- Xiao, Wang, Zhang, Dong, **Mooney**, Petersen, Yonezawa. [A two-stage solution to quantum process tomography: error analysis and optimal design](https://arxiv.org/abs/2402.08952), *IEEE Transactions on Information Theory* (2025)

## PhD thesis

**Mooney**. [Entanglement in superconducting quantum devices and improving quantum circuit compilation](https://minerva-access.unimelb.edu.au/items/a7ae6399-00a8-4082-a2b9-b4858bf246f7), School of Physics, The University of Melbourne (2022)

## In the media

- Davis and Vogt-Lee. ["Turning quantum states into music at Australia's first ever Qiskit hackathon"](https://medium.com/qiskit/turning-quantum-states-into-music-at-australias-first-ever-qiskit-hackathon-25da7f09d226), IBM Qiskit Blog (2022)
- White, Mooney, Hill, Hollenberg. ["Generating whole-processor entanglement on 27- and 65-qubit quantum systems"](https://research.ibm.com/blog/whole-device-entanglement), IBM Research Blog (2021)
- Holland. ["So, you want to work in quantum computing"](https://pursuit.unimelb.edu.au/articles/so-you-want-to-work-in-quantum-computing), Pursuit, University of Melbourne (2018)
