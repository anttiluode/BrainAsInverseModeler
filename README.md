# Brain as Inverse Modeler

**Could a neuron reconstruct a hidden process from its sensory history, then make part of that reconstruction available through the signal it emits?**

This repository develops that question from Antti Luode's Deerskin / Geometric-Neuron idea, Takens-style state reconstruction, state-dependent action-potential waveforms, and the concrete inverse problem demonstrated by [Varjoluotain](https://github.com/anttiluode/Varjoluotain).

The working hypothesis is:

> Diverse dendritic dynamics may maintain coordinates of an observable hidden process. Somatic and axonal output may expose selected aspects of those coordinates. A receiving neuron interprets the arriving signal through its own history-dependent state. Learning could organize these coupled systems into a distributed predictive model.

There are two different questions here: **what the neuron can retain**, and **what another neuron can recover from its output**. Neither follows automatically from the other.

## Read the analysis

- **[Research note: history, emitted state, and the inverse model](docs/analysis.md)** develops the mathematics, the biological evidence, the connection to the repositories, and the useful consequences.
- **[Experiment protocol](docs/experiments.md)** describes tests that distinguish hidden-state reconstruction, transmission, and downstream use.

## Why the waveform paper matters

Martin-Burgos and colleagues' 2026 preprint, *Action potential waveforms are state-dependent*, reports that intracellular spike shape varies systematically with recent input and local network conditions. It makes the emitted event a plausible additional measurement of the state that produced it. The study does not establish that downstream neurons decode a world model from those waveforms.

The stronger computational question is therefore:

**Can two histories that require different future predictions remain distinguishable after dendritic processing, spike generation, transmission, and reception?**

## Why the wall matters

Varjoluotain demonstrates how an obstruction can structure a measurement so that hidden sources become distinguishable. Its code also tracks differences that the measurement cannot resolve. Those two ideas belong together: build an instrument for recovering hidden state, and keep an account of what it leaves ambiguous.

For the proposed neuron, the corresponding instrument is its temporal response geometry. Its recent history, filter diversity, nonlinearities, and readout determine which hidden distinctions become accessible.

## Status

Research analysis and proposed experiments, 30 September 2026. No new neuronal simulations or biological replications have been run for this repository. Existing repository results are discussed as reported results and inspected mechanisms, with their limits preserved.

The mathematical foundation has established precedents in delay embedding and reservoir computing. The proposed connection to a particular dendritic architecture, waveform communication, and a distributed inverse model remains to be tested.

Primary references and the source-review scope are in the [research note](docs/analysis.md#references-and-source-review).

