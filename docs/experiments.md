# Experiments that separate reconstruction, transmission, and use

*Proposed protocol, 30 September 2026. No results have been generated for these experiments.*

The objective is to locate which hidden-world distinctions survive a complete observer pathway. Each stage should produce its own result before the next stage is interpreted. Freeze the implementation, schedules, metrics and numeric acceptance thresholds before collecting its first receipt.

## A. Does the observer retain hidden dynamical state?

Start with a pendulum and a Lorenz system as calibration worlds. The observer receives one declared scalar observable. Use a causal bank of delays, diverse decay filters, or resonators; expose its full current state to an evaluation decoder.

For the Lorenz system, a standard initial setting is sigma = 10, rho = 28, beta = 8/3, observing x only. This is a familiar numerical reconstruction benchmark, not a claim that the chosen observable satisfies a generic embedding theorem everywhere. Include a second declared scalar mixture and record where the two sensors differ in recoverability.

The online model receives no hidden coordinates. A separate decoder may use hidden labels on calibration trajectories to evaluate what its states contain. Fit normalization, decoder capacity, filter-selection choices and hyperparameters only on the calibration split. Freeze them before evaluating new trajectories and initial conditions. Separate temporal blocks by more than the largest retained history window, and ensure all tap timestamps are at or before the current observation.

### Comparisons

| Model | Purpose |
|---|---|
| Current observation only | Shows what history adds |
| Raw delay vector | Established positive control for the reconstruction setup |
| Equal-size ordinary reservoir | Tests whether the proposed organization adds an advantage |
| Dendritic filter/resonator state | Tests the proposed history coordinates |
| Deerskin-style squared projection and average | Measures loss at the current recognition readout |
| Several soma readouts or a soma output history | Tests practical access to retained coordinates |

Count real state variables, retained samples, learned parameters and readout cost separately. A complex mode contains two real state variables. Match evaluation-decoder capacity across comparisons; do not hide a larger decoder in one arm.

### Measurements and controls

Measure held-out hidden-coordinate error, using training-scale normalization; multi-step sensory forecasts; and examples with closely matched current observations but materially different hidden states and futures. Fit or learn transitions from permitted observations, then close the input channel for short intervals and report forecast error as a function of the gap. Chaotic systems have limited forecast horizons, so show the full error curve.

Reset the observer immediately before readout; shuffle histories; replace diverse filters with identical ones; vary noise and sampling rate. Add a truly uncoupled hidden variable that never affects the observable. Any claimed recovery of that variable must be treated as leakage or a dataset shortcut until disproved.

A successful calibration requires hidden-state recovery and disambiguation beyond the current-observation baseline. If the raw delay positive control also fails, diagnose the sensor, sampling, data coverage and evaluation before blaming the dendritic mechanism. Architectural value requires a further measured benefit over the capable matched baselines.

## B. Does a useful distinction survive the emitted signal?

Only proceed after A has shown that the sender contains the target distinction. Compare its internal state, accessible soma output, emitted signal, post-transmission signal and receiver state separately.

An engineered state-dependent waveform can first test computational sufficiency. Label it explicitly as a constructed channel: mapping the withheld answer directly into waveform width would demonstrate a communication code, not discovery of one. A subsequent mechanistic model should generate shape variation from declared internal dynamics without receiving the evaluation target as a privileged input.

Use the same event schedule in the waveform and fixed-template comparison. Add separate controls for amplitude, area, energy and timing; report which cues survive each normalization. Equal-area and equal-energy waveform families are useful engineered controls, but should not be presented as observed biological constraints.

The receiver must only receive the channel output. It must not receive sender state, waveform labels, hidden world coordinates, or a time index that identifies the answer.

If using the attached paper's data to identify candidate waveform features, separate pre-spike/baseline measurements from features actually available in the arriving signal. Include controls conditioned on baseline voltage, current drive and a capable recent-spike-history model. A predictive electrode-window feature is not automatically a usable communication feature.

Test transmission transformations rather than assuming an intracellular soma waveform reaches the receiver unchanged. Begin with an explicit filter and noisy synaptic conversion; then compare a declared conductance-based pathway if warranted. Inspect whether the target information survives at each location.

Controls: waveform clamping; waveform shuffling within matched event-time groups; fixed receiver susceptibility; receiver reset; and a capable timing/rate-history baseline. If shape contributes an extra analog channel, count its degrees of freedom, resolution, noise and decoding cost. Also compare with a timing channel allowed a corresponding additional communication budget.

The useful result is a receiver prediction improved by a distinction transmitted through shape, with causal ablations removing that gain. Failure after transmission, despite a readable sender state, identifies the bottleneck directly.

## C. Does history support new questions and distributed inference?

Choose the query only after the observation history. Possible questions include direction, a hidden coordinate, future threshold crossing, or phase at a declared horizon. Present identical stored state to different queries. Train on one set of queries and evaluate explicitly declared held-out queries or horizons.

This makes the measurement harder to satisfy by compiling one fixed answer during the history. Keep a conventional recurrent model with comparable state and training resources as a capable competitor. A query-responsive state is compatible with many recurrent mechanisms; selective response alone does not establish a special resonance mechanism.

For distributed inference, give two observers complementary measurements. Compare each alone, two observers without communication, a shared-drive control, fixed-shape events, and state-dependent events at matched budgets. Intervene on the communication pathway while preserving the sensory streams. Measure whether the receiver recovers missing state or makes better predictions.

A synchrony plot is insufficient. The criterion is a causal improvement attributable to useful exchanged information, beyond common drive and the receiver's independent history.

## D. Connect the observer to the wall instrument

After A-C, use Varjoluotain's forward model to generate a slowly changing hidden source behind the occluder. Begin with a low-dimensional scene family: a known pattern with changing position, angle or a few independently varying intensities. Give the observer a declared small subset of wall measurements, potentially one pixel over time.

A temporal observer may recover low-dimensional dynamics when those dynamics leave distinguishable measurements. It cannot be expected to reconstruct an arbitrary static high-resolution image from one constant scalar. Specify the scene family and its dimension in the demo.

Compare present-frame inversion with history-based inference, plate present versus absent, correctly calibrated versus perturbed geometry, and changes in room light. Generate test data with a different renderer or controlled real setup when possible. Using the same forward model for generation and inversion is a calibration, with optimistic model matching.

Display five things: the permitted observation, estimated hidden state, its forecast, uncertainty or surviving alternatives, and withheld truth. Show a confused pair of worlds and the next measurement that separates them. This would make the accidental instrument and the temporal observer visible in the same demonstration.

## Receipt and stopping rules

For each stage record the code revision, seeds, world parameters, sampling interval, sensor definition, split boundaries, state/communication budgets, trained parameters, metrics and every ablation. Keep failed seeds and confused examples.

Classify outcomes separately:

- **Retention:** the internal state contains the distinction.
- **Access:** the permitted soma output exposes it.
- **Transmission:** the channel preserves it.
- **Use:** the receiver gains a correct prediction or action from it.
- **Identification:** the result transfers across declared model or sensor mismatch.

Stop expanding the biological interpretation when the relevant stage fails. Correct the identified bottleneck or keep the negative result. A positive result at one stage should remain valuable on its own.
