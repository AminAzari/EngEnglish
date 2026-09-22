# GRAMMAR FOR ENGINEERS APPENDIX

**Scientific and Technical English for Electrical Engineering**
*Undergraduate Level (B2–C1)*

> This appendix covers grammar points that are essential for writing and reading engineering papers, reports, and technical documentation. All examples are drawn from electrical engineering contexts. Use this as a reference—look up the section you need.

---

## 1. Tenses in Scientific Writing

### Why This Matters
Choosing the correct tense signals to the reader whether you are stating a general truth, describing your experimental procedure, or connecting past work to the present. Incorrect tense use is one of the most common errors in non-native engineering papers.

### 1.1 Present Simple
**Use:** General truths, established facts, describing how systems work, stating what figures show.

- The controller adjusts the output voltage based on the error signal.
- A low-pass filter attenuates frequencies above the cutoff.
- Figure 4 shows the frequency response of the proposed antenna.
- The diode conducts when the forward voltage exceeds 0.7 V.

**Paper sections:** Introduction (general background), Discussion (interpreting results as general claims), figure/table descriptions.

### 1.2 Past Simple
**Use:** Describing completed experimental actions, specific measurements, what was done in a study.

- The signal was sampled at 1 kHz using a 16-bit ADC.
- We designed a two-stage amplifier with 40 dB gain.
- The prototype operated at 28 GHz.
- The simulation ran for 10,000 iterations.

**Paper sections:** Methods/Methodology, Results (specific findings of this study).

### 1.3 Present Perfect
**Use:** Relating past research to the current state of knowledge, indicating that something started in the past and is still relevant.

- Several studies have investigated the use of MIMO in 5G systems.
- Researchers have proposed various methods to reduce harmonic distortion.
- This approach has been widely adopted in power electronics.
- No previous work has addressed this specific configuration.

**Paper sections:** Introduction (literature review), Discussion (relating findings to existing knowledge).

### 1.4 Tense Use by Paper Section

| Section | Primary Tense | Example |
|---------|--------------|---------|
| Abstract | Past simple + Present simple | "We designed... The results show..." |
| Introduction (background) | Present simple | "Renewable energy systems require..." |
| Introduction (lit review) | Present perfect | "Several authors have proposed..." |
| Methods | Past simple | "The circuit was fabricated using..." |
| Results | Past simple | "The THD measured 3.2%." |
| Discussion | Present simple + Past simple | "This confirms that... The error was caused by..." |
| Conclusion | Present simple + Present perfect | "The proposed method achieves... We have demonstrated..." |

### 1.5 AI/ML Engineering Examples

1. The transformer model **processes** input tokens in parallel rather than sequentially. *(present simple — system description)*
2. The neural network **was trained** on 1.5 trillion tokens from a multilingual corpus. *(past simple — experiment)*
3. Researchers **have demonstrated** that large language models can perform zero-shot reasoning tasks. *(present perfect — current relevance)*
4. The attention mechanism **computes** a weighted sum of value vectors. *(present simple — how system works)*
5. We **fine-tuned** the pre-trained model on domain-specific data for 3 epochs. *(past simple — method)*
6. The loss function **converged** after approximately 50,000 training steps. *(past simple — specific result)*
7. Transfer learning **has reduced** the need for large labelled datasets in many NLP tasks. *(present perfect — current state)*
8. Recent work **has explored** the use of reinforcement learning from human feedback (RLHF) to align model outputs with user intent. *(present perfect — literature)*

### 1.6 Example Sentences from EE Contexts

1. The proposed PLL **locks** within 50 μs under nominal conditions. *(present simple — system description)*
2. The transformer **was tested** at rated load for 24 hours. *(past simple — experiment)*
3. Recent advances **have enabled** the integration of GaN transistors in power converters. *(present perfect — current relevance)*
4. The bandwidth **exceeds** 500 MHz across the operating range. *(present simple — general characteristic)*
5. We **measured** the S-parameters using a vector network analyser. *(past simple — method)*
6. The noise figure **was found** to be 2.3 dB at 6 GHz. *(past simple — specific result)*
7. Numerous researchers **have explored** deep learning for fault detection in power grids. *(present perfect — literature)*
8. The control loop **maintains** stability even under load transients. *(present simple — how system works)*
9. The FPGA **was programmed** using VHDL. *(past simple — what was done)*
10. Machine learning techniques **have shown** promise in predictive maintenance of electrical machines. *(present perfect — current state)*

### 1.7 Exercise: Choose the Correct Tense

Complete each sentence with the correct form of the verb in brackets.

1. The output voltage __________ (remain) stable at 3.3 V under varying loads. *(system description)*
2. We __________ (collect) data over a period of 72 hours. *(experiment)*
3. Several groups __________ (investigate) the use of metamaterials for antenna miniaturisation. *(literature review)*
4. The converter __________ (operate) at a switching frequency of 100 kHz. *(general truth)*
5. The filter __________ (design) using Butterworth approximation. *(methods)*
6. Recent publications __________ (demonstrate) improved efficiency with SiC MOSFETs. *(current relevance)*
7. Figure 7 __________ (illustrate) the transient response of the system. *(figure description)*
8. The prototype __________ (achieve) a peak efficiency of 96.2% during testing. *(specific result)*
9. Ohm's law __________ (state) that voltage equals current times resistance. *(established fact)*
10. No prior study __________ (address) this particular topology for bidirectional charging. *(gap in literature)*

### Answer Key — Exercise 1.7

1. remains
2. collected
3. have investigated
4. operates
5. was designed
6. have demonstrated
7. illustrates
8. achieved
9. states
10. has addressed

---

## 2. Passive Voice in Engineering

### 2.1 Why Passive Is Common in Scientific Writing

In engineering papers, the focus is on **what was done** and **what was observed**, not on who did it. The passive voice:
- Keeps the focus on processes, equipment, and results
- Creates an objective, impersonal tone
- Is expected in Methods and Results sections
- Avoids excessive use of "I" or "we"

### 2.2 Formation

| Tense | Active | Passive |
|-------|--------|---------|
| Present simple | The inverter converts DC to AC. | DC is converted to AC by the inverter. |
| Past simple | We measured the impedance. | The impedance was measured. |
| Present perfect | Researchers have developed a new algorithm. | A new algorithm has been developed. |
| Modal | We can reduce the noise. | The noise can be reduced. |

**Structure:** Subject + *be* (conjugated) + past participle (+ by agent, if needed)

### 2.3 Active vs Passive: When to Choose Each

| Use Passive When... | Use Active When... |
|--------------------|--------------------|
| The agent is obvious or unimportant | You want to emphasise who did something |
| You want to focus on the object/process | You want a more direct, concise style |
| Convention requires it (Methods) | You are writing a design report for your team |
| The agent is unknown | The sentence is clearer in active voice |

**Modern trend:** Many journals now accept "we" in moderation. Use a mix—predominantly passive in Methods, more active in Introduction and Discussion.

### 2.4 Examples from Engineering

- The circuit **was designed** to operate in the subthreshold region.
- The measurements **were taken** at room temperature (25°C).
- The algorithm **is implemented** in MATLAB R2024a.
- A 50 Ω termination **was connected** to port 2.
- The switching losses **are minimised** through zero-voltage switching (ZVS).
- The proposed topology **has been validated** through simulation and experiment.
- The signal **was filtered** using a fourth-order Chebyshev bandpass filter.
- All capacitors **were rated** at 50 V.

### 2.5 AI/ML Engineering Examples (Passive Voice)

- The model **was trained** on 1.5 trillion tokens from a diverse web corpus.
- The dataset **was split** into training (80%), validation (10%), and test (10%) subsets.
- The hyperparameters **were optimised** using Bayesian search over 200 trials.
- Attention scores **are computed** by taking the dot product of query and key vectors.
- The weights **were initialised** using Xavier uniform distribution.
- The generated outputs **were evaluated** by human annotators on a 5-point Likert scale.
- A dropout rate of 0.1 **was applied** to all layers during training.
- The pre-trained embeddings **have been widely adopted** in downstream NLP tasks.

### 2.6 Exercise: Convert Between Active and Passive

**A. Convert to passive voice:**

1. We fabricated the PCB using a four-layer stack-up.
2. The team tested the motor at various speed settings.
3. The researcher calibrated the oscilloscope before measurements.
4. Engineers typically design power supplies to meet specific load requirements.

**B. Convert to active voice:**

5. The gain was set to 20 dB by adjusting the feedback resistor.
6. The data were recorded by the acquisition system at 10 kS/s.
7. The control algorithm was optimised using a genetic algorithm by the research group.
8. The antenna pattern was simulated using CST Microwave Studio.

### Answer Key — Exercise 2.6

1. The PCB was fabricated using a four-layer stack-up.
2. The motor was tested at various speed settings.
3. The oscilloscope was calibrated before measurements.
4. Power supplies are typically designed to meet specific load requirements.
5. We set the gain to 20 dB by adjusting the feedback resistor.
6. The acquisition system recorded the data at 10 kS/s.
7. The research group optimised the control algorithm using a genetic algorithm.
8. We simulated the antenna pattern using CST Microwave Studio.

---

## 3. Modal Verbs for Technical Communication

### 3.1 Overview

Modal verbs express degrees of certainty, ability, obligation, and possibility. In engineering writing, choosing the right modal is critical—it determines whether you are making a strong claim or a cautious suggestion.

### 3.2 Can / Could

**Can** — present ability, general possibility, what a system is capable of
- The proposed converter **can** achieve efficiencies above 95%.
- The FPGA **can** process up to 200 million samples per second.

**Could** — past ability, polite possibility, less certain than "can"
- The interference **could** be caused by improper grounding.
- With additional shielding, the SNR **could** be improved by 6 dB.

### 3.3 May / Might

**May** — possibility (formal), permission in standards
- This discrepancy **may** be attributed to parasitic capacitance.
- The system **may** experience instability at high gain values.

**Might** — lower probability than "may"
- The observed drift **might** result from thermal effects.
- A higher-order model **might** better capture the nonlinear behaviour.

### 3.4 Should

**Should** — recommendation, expected outcome, design guidance
- The decoupling capacitor **should** be placed as close to the IC as possible.
- The settling time **should** not exceed 10 ms for this application.
- Designers **should** consider EMC requirements early in the design process.

### 3.5 Must

**Must** — necessity, regulatory requirement, strong logical conclusion
- The insulation **must** withstand 2.5 kV for safety certification.
- The sampling rate **must** be at least twice the maximum signal frequency (Nyquist).
- Given the measured phase margin, the system **must** be operating near instability.

### 3.6 Would

**Would** — hypothetical situations, conditional outcomes, modelling assumptions
- Increasing the number of layers **would** reduce the overall inductance.
- A lossless model **would** predict zero attenuation.
- This **would** require a complete redesign of the power stage.

### 3.7 Summary Table

| Modal | Strength | Use in Engineering |
|-------|----------|-------------------|
| must | Very strong | Safety requirements, Nyquist-type rules, strong conclusions |
| should | Strong | Recommendations, design guidelines, expected behaviour |
| can | Moderate–strong | System capabilities, general possibility |
| may | Moderate | Research possibility, cautious claims |
| could | Moderate–weak | Tentative explanations, conditional possibility |
| might | Weak | Speculative, lowest certainty |
| would | Conditional | Hypothetical outcomes, modelling |

### 3.8 AI/ML Engineering Examples (Modal Verbs)

- LLMs **can** generate coherent text but **may** produce hallucinations. *(ability + possibility)*
- The model **should** be validated on a held-out test set to avoid overfitting. *(recommendation)*
- Increasing the number of attention heads **could** improve the model's ability to capture diverse linguistic patterns. *(tentative possibility)*
- Without regularisation, the network **will** memorise the training data. *(certainty/prediction)*
- The generated text **might** contain factual inaccuracies that are difficult to detect automatically. *(low-certainty possibility)*
- A larger training corpus **would** likely improve performance on rare tokens. *(hypothetical)*
- Practitioners **must** consider ethical implications when deploying generative AI in safety-critical systems. *(strong obligation)*

### 3.9 Exercise: Choose the Appropriate Modal

Select the best modal verb for each sentence.

1. According to IEC 61000, the conducted emissions __________ not exceed the specified limits. *(regulatory requirement)*
2. The proposed architecture __________ reduce latency by up to 30%. *(system capability)*
3. If the clock frequency were doubled, the power dissipation __________ increase significantly. *(hypothetical)*
4. The anomaly __________ be caused by electromagnetic interference, but further investigation is needed. *(tentative explanation)*
5. The sampling frequency __________ satisfy the Nyquist criterion to avoid aliasing. *(necessity)*
6. Designers __________ verify thermal performance through simulation before prototyping. *(recommendation)*
7. With improved materials, future devices __________ achieve breakdown voltages exceeding 10 kV. *(future possibility)*
8. The observed oscillation __________ indicate that the phase margin is insufficient. *(moderate possibility)*

### Answer Key — Exercise 3.9

1. must
2. can
3. would
4. could / might
5. must
6. should
7. may / could
8. may



---

## 4. Hedging Language

### 4.1 Why Hedging Is Important in Academic Writing

In engineering research, absolute claims can be:
- Scientifically inaccurate (results may not generalise)
- Unprofessional (reviewers will challenge overclaims)
- Risky (strong claims require strong evidence)

Hedging shows intellectual honesty and awareness of limitations. It is **not** weakness—it is precision.

### 4.2 Hedging Verbs

| Verb | Example |
|------|---------|
| suggest | The results **suggest** that thermal noise is the dominant factor. |
| indicate | The measurements **indicate** a resonance near 3.5 GHz. |
| appear | The system **appears** to be stable under these conditions. |
| seem | The degradation **seems** to be related to moisture ingress. |
| tend | GaN devices **tend** to exhibit higher efficiency at high frequencies. |
| imply | The phase shift **implies** the presence of a parasitic inductance. |

### 4.3 Hedging Adverbs

| Adverb | Example |
|--------|---------|
| possibly | The fault is **possibly** due to a manufacturing defect. |
| probably | The oscillation is **probably** caused by insufficient damping. |
| apparently | The losses are **apparently** dominated by conduction losses. |
| relatively | The proposed method is **relatively** insensitive to parameter variations. |
| approximately | The bandwidth is **approximately** 200 MHz. |
| somewhat | The response is **somewhat** degraded at elevated temperatures. |
| largely | The efficiency improvement is **largely** attributable to reduced switching losses. |

### 4.4 Hedging Phrases

- *It is likely that* the error originates from quantisation effects.
- *The results suggest that* the proposed controller outperforms the conventional PID.
- *This may be due to* impedance mismatch at the interconnect.
- *It is possible that* the discrepancy arises from unmodelled dynamics.
- *To some extent,* the performance depends on ambient temperature.
- *Under certain conditions,* the system may become unstable.
- *There is evidence to suggest that* WBG semiconductors will dominate future power electronics.

### 4.5 AI/ML Engineering Examples (Hedging)

- The results **suggest** that fine-tuning **may** improve domain-specific accuracy.
- The attention mechanism **appears** to focus on syntactically relevant tokens during parsing tasks.
- Larger models **tend** to exhibit emergent capabilities not present in smaller variants.
- The degradation in performance on out-of-distribution data **is likely** due to distributional shift.
- It **is possible that** the model has memorised portions of the training data rather than learning generalisable patterns.
- The hallucination rate **seems** to decrease with increased model scale, though further investigation is needed.
- Chain-of-thought prompting **may** improve reasoning accuracy in arithmetic tasks.
- *To some extent,* the observed improvements **could** be attributed to better data curation rather than architectural innovations.

### 4.6 Too Strong vs Appropriately Hedged

| ❌ Too Strong | ✅ Appropriately Hedged |
|--------------|------------------------|
| This proves that GaN is better than Si. | These results suggest that GaN may offer advantages over Si in this application. |
| The algorithm always converges. | The algorithm tends to converge under the tested conditions. |
| The noise is caused by the power supply. | The noise is likely caused by the power supply. / The noise appears to originate from the power supply. |
| Our method is the best. | Our method appears to outperform existing approaches for this class of problems. |
| This will replace all existing solutions. | This approach has the potential to complement existing solutions. |

### 4.7 Exercise: Add Hedging to Overconfident Statements

Rewrite each sentence using appropriate hedging. Multiple correct answers are possible.

1. The proposed filter eliminates all harmonic distortion.
2. The failure is caused by electromigration.
3. Our algorithm is faster than every existing method.
4. Renewable energy will completely replace fossil fuels by 2040.
5. The temperature increase destroys the semiconductor junction.
6. This topology is the optimal solution for all DC-DC conversion applications.

### Answer Key — Exercise 4.7 (Sample Answers)

1. The proposed filter **appears to** significantly reduce harmonic distortion. / The proposed filter **tends to** attenuate the dominant harmonics.
2. The failure **may be** caused by electromigration. / The failure **is likely** due to electromigration.
3. Our algorithm **seems to be** faster than most existing methods under the tested conditions.
4. Renewable energy **may** largely replace fossil fuels in the coming decades. / It is possible that renewable energy **will** play a dominant role by 2040.
5. The temperature increase **can potentially** damage the semiconductor junction. / Excessive temperature **may lead to** degradation of the junction.
6. This topology **appears to be** a promising solution for a range of DC-DC conversion applications. / This topology **may offer** advantages for many DC-DC conversion scenarios.

---

## 5. Conditionals in Engineering

### 5.1 Zero Conditional (General Truths)

**Structure:** If + present simple, present simple

Used for stating physical laws, system behaviour, and design rules that are always true.

- If the voltage exceeds the breakdown threshold, the diode conducts in reverse.
- If the loop gain equals unity at the crossover frequency, the system is marginally stable.
- If the input impedance is not matched, signal reflection occurs.
- When the duty cycle increases, the output voltage rises proportionally.

### 5.2 First Conditional (Likely/Real Outcomes)

**Structure:** If + present simple, will + base verb

Used for predicting outcomes of design decisions, test conditions, or future actions.

- If we increase the gain beyond 40 dB, the system **will** become unstable.
- If the temperature rises above 125°C, the device **will** enter thermal shutdown.
- If the antenna is placed too close to the ground plane, the radiation pattern **will** be distorted.
- If additional capacitance is added, the resonant frequency **will** decrease.

### 5.3 Second Conditional (Hypothetical/Unlikely)

**Structure:** If + past simple, would + base verb

Used for hypothetical designs, theoretical improvements, or conditions not currently met.

- If we had a wider bandwidth channel, we **could** achieve higher data rates.
- If the material were lossless, the Q-factor **would** be infinite.
- If the budget allowed for a GaN amplifier, we **would** expect 3 dB more output power.
- If the cable length were shorter, the attenuation **would** be negligible.

### 5.4 Third Conditional (Past Hypothetical)

**Structure:** If + past perfect, would have + past participle

Used for reflecting on what could have happened differently in past experiments or designs.

- If we had used a higher-order filter, the stopband rejection **would have been** greater.
- If the grounding had been improved, the noise **would not have affected** the measurement.
- If the team had selected a different topology, the efficiency **would have exceeded** 98%.
- If the simulation had included parasitic elements, the predicted bandwidth **would have been** more accurate.

### 5.5 AI/ML Engineering Examples (Conditionals)

**Zero Conditional:**
- If the learning rate is too high, the model diverges during training.
- When the batch size increases, the gradient estimate becomes less noisy.

**First Conditional:**
- If we apply early stopping, the model will not overfit to the training set.
- If the dataset contains biased labels, the model will learn and amplify those biases.

**Second Conditional:**
- If the training corpus were free of harmful content, the model would produce fewer toxic outputs.
- If we had unlimited computational budget, we could train on the entire web corpus without sampling.

**Third Conditional:**
- If the researchers had used a larger validation set, they would have detected the overfitting earlier.
- If data augmentation had been applied during pre-training, the model would have been more robust to noisy inputs.

### 5.6 Exercise: Complete the Conditional Sentences

1. If the supply voltage drops below 2.7 V, the regulator __________ (not maintain) a stable output. *(zero conditional)*
2. If we add a second amplification stage, the gain __________ (increase) by approximately 20 dB. *(first conditional)*
3. If the substrate were made of sapphire, the thermal conductivity __________ (be) significantly higher. *(second conditional)*
4. If the engineers had noticed the layout error earlier, the redesign __________ (not delay) the project. *(third conditional)*
5. If the modulation index exceeds 1, clipping __________ (occur). *(zero conditional)*
6. If the filter order is increased, the transition band __________ (become) narrower. *(first conditional)*
7. If we had access to a 65 nm process, we __________ (achieve) lower power consumption. *(second conditional)*
8. If the thermal paste had been applied correctly, the junction temperature __________ (not reach) critical levels. *(third conditional)*

### Answer Key — Exercise 5.6

1. does not maintain (zero)
2. will increase (first)
3. would be (second)
4. would not have delayed (third)
5. occurs (zero)
6. will become (first)
7. could achieve (second)
8. would not have reached (third)

---

## 6. Relative Clauses

### 6.1 Defining Relative Clauses

Identify which person/thing we mean. **No commas.** Essential information.

- The antenna **which operates at 2.4 GHz** is designed for IoT applications.
- The capacitor **that was connected in parallel** reduced the ripple voltage.
- Engineers **who specialise in power electronics** are in high demand.
- The frequency **at which the gain drops by 3 dB** is called the cutoff frequency.

**Note:** In technical writing, "that" and "which" are both used for defining clauses. Some style guides prefer "that" for defining and "which" for non-defining.

### 6.2 Non-Defining Relative Clauses

Add extra information. **Commas required.** Can be removed without losing essential meaning.

- The proposed algorithm, **which reduces computational complexity by 40%**, was validated on real-time hardware.
- Silicon carbide (SiC), **which has a wider bandgap than silicon**, enables higher operating temperatures.
- The LM7805 regulator, **which provides a fixed 5 V output**, is widely used in embedded systems.
- Prof. Smith, **who pioneered this topology in 2018**, presented the keynote lecture.

### 6.3 Reduced Relative Clauses

For conciseness (very common in technical papers), the relative pronoun + be verb can be removed.

| Full Relative Clause | Reduced |
|---------------------|---------|
| The signal **that was measured** at the output | The signal **measured** at the output |
| The technique **which is based** on FFT | The technique **based** on FFT |
| The transistor **which is operating** in saturation | The transistor **operating** in saturation |
| The system **which was proposed** by Lee et al. | The system **proposed** by Lee et al. |

### 6.4 AI/ML Engineering Examples (Relative Clauses)

**Defining:**
- The attention heads **that attend to positional information** are crucial for understanding word order.
- The dataset **which contains over 10 billion tokens** was used for pre-training the language model.
- The embedding layer **that maps discrete tokens to continuous vectors** is the first component of the transformer.

**Non-defining:**
- GPT-4, **which was released in March 2023**, demonstrates strong multi-modal reasoning capabilities.
- The BERT architecture, **which uses bidirectional self-attention**, revolutionised NLP benchmarks.
- The softmax function, **which normalises the attention weights to sum to one**, ensures a valid probability distribution.

**Reduced:**
- The features **extracted by the convolutional layers** are fed into a fully connected classifier.
- The model **trained on multilingual data** performs well across 104 languages.

### 6.5 Exercise: Combine Sentences Using Relative Clauses

Combine each pair into one sentence using an appropriate relative clause.

1. The converter achieves 97% efficiency. It uses a novel soft-switching technique.
2. The research group published their findings in IEEE Transactions. The group is based at MIT.
3. The resonant frequency was measured at 5.8 GHz. The resonant frequency determines the operating band.
4. The DSP processor handles all computations in real time. It was selected for its low power consumption.
5. The results were obtained under controlled laboratory conditions. The results confirm the theoretical predictions.
6. The inductor has a saturation current of 10 A. The inductor was wound using litz wire.

### Answer Key — Exercise 6.5

1. The converter, **which uses a novel soft-switching technique**, achieves 97% efficiency. *(non-defining)*
2. The research group, **which is based at MIT**, published their findings in IEEE Transactions. *(non-defining)*
3. The resonant frequency, **which determines the operating band**, was measured at 5.8 GHz. *(non-defining)*
4. The DSP processor **that was selected for its low power consumption** handles all computations in real time. *(defining)*
5. The results **that were obtained under controlled laboratory conditions** confirm the theoretical predictions. *(defining)* OR: The results, **which were obtained under controlled laboratory conditions**, confirm the theoretical predictions. *(non-defining)*
6. The inductor, **which was wound using litz wire**, has a saturation current of 10 A. *(non-defining)*



---

## 7. Comparatives and Superlatives

### 7.1 Why Comparison Matters in Engineering

Comparing performance, efficiency, cost, and complexity is fundamental to engineering writing. Every paper that proposes a new method must compare it to existing approaches.

### 7.2 Basic Comparative Structures

| Structure | Example |
|-----------|---------|
| -er than | The proposed design is **smaller than** the conventional one. |
| more + adj + than | The GaN amplifier is **more efficient than** the Si-based design. |
| less + adj + than | The linear regulator is **less efficient than** the switching converter. |
| the + -est | This topology achieves **the highest** efficiency among those tested. |
| the most + adj | The OFDM scheme is **the most spectrally efficient** option. |

### 7.3 Academic Comparison Phrases

| Phrase | Example |
|--------|---------|
| outperforms | The proposed method **outperforms** the baseline by 12%. |
| is superior to | The adaptive controller **is superior to** the fixed-gain controller in terms of settling time. |
| is inferior to | At low SNR, BPSK **is inferior to** turbo-coded QPSK. |
| comparable to | The accuracy is **comparable to** that of commercial instruments. |
| as efficient as | The new converter is **as efficient as** the reference design at full load. |
| significantly better/worse | The BER is **significantly better** with equalisation enabled. |
| marginally higher/lower | The power consumption is **marginally higher** with the added protection circuitry. |
| approximately equal to | The gain is **approximately equal to** the theoretical prediction. |

### 7.4 Quantifying Comparisons

- The proposed antenna is **3 dB** more sensitive than the reference.
- The processing time is reduced **by a factor of 5**.
- The efficiency is improved **from 89% to 94%**.
- Latency is **50% lower** compared to the conventional approach.
- The error rate is **an order of magnitude smaller**.
- The new design is **twice as fast as** the previous generation.

### 7.5 AI/ML Engineering Examples (Comparatives)

- The transformer architecture is **significantly more parallelisable than** recurrent neural networks.
- GPT-4 **outperforms** GPT-3.5 on all evaluated reasoning benchmarks.
- The fine-tuned model achieves **12 percentage points higher** accuracy than the zero-shot baseline.
- Inference latency is **approximately three times longer** for the 70B parameter model compared to the 7B variant.
- The retrieval-augmented approach is **comparable to** fine-tuning in terms of factual accuracy, but **considerably less expensive** to implement.
- RLHF-trained models produce outputs that are **significantly more aligned** with human preferences than those from supervised fine-tuning alone.
- The quantised 4-bit model is **marginally less accurate** than the full-precision version but requires **75% less** memory.

### 7.6 Exercise: Write Comparisons from Data

Use the following data to write comparison sentences.

| Method | Efficiency | THD | Cost | Processing Time |
|--------|-----------|-----|------|----------------|
| Method A (proposed) | 96.5% | 2.1% | $45 | 12 ms |
| Method B (conventional) | 91.2% | 4.8% | $32 | 58 ms |
| Method C (state-of-art) | 95.8% | 2.4% | $78 | 15 ms |

Write sentences that:
1. Compare Method A efficiency to Method B.
2. Compare Method A THD to Method C.
3. Compare Method B cost to Method C.
4. State which method has the lowest processing time.
5. Compare Method A to Method C on cost.
6. Give an overall assessment of Method A vs. the other two.

### Answer Key — Exercise 7.6 (Sample Answers)

1. Method A achieves an efficiency of 96.5%, which is 5.3 percentage points higher than Method B (91.2%).
2. Method A exhibits a slightly lower THD (2.1%) compared to Method C (2.4%).
3. Method B is significantly less expensive ($32) than Method C ($78), costing less than half the price.
4. Method A has the shortest processing time (12 ms) among all three methods, which is approximately five times faster than Method B.
5. The proposed method (A) is considerably more cost-effective than Method C ($45 vs. $78) while achieving comparable or superior performance.
6. Overall, Method A outperforms both Method B and Method C, offering the highest efficiency, the lowest THD, and the fastest processing time at a moderate cost.

---

## 8. Cause and Effect

### 8.1 Expressing Cause and Effect in Technical Writing

Engineering papers constantly explain why things happen. Mastering cause-and-effect language allows you to discuss mechanisms, explain results, and diagnose problems.

### 8.2 Cause → Effect Connectors

| Connector | Grammar | Example |
|-----------|---------|---------|
| because | clause + because + clause | The output distorted **because** the amplifier was driven into saturation. |
| since | Since + clause, clause | **Since** the sampling rate was below Nyquist, aliasing occurred. |
| as | As + clause, clause | **As** the temperature increased, the leakage current rose exponentially. |
| due to | due to + noun phrase | The failure was **due to** electrostatic discharge (ESD). |
| owing to | owing to + noun phrase | **Owing to** the high Q-factor, the bandwidth was narrow. |
| because of | because of + noun phrase | **Because of** impedance mismatch, 30% of the signal was reflected. |

### 8.3 Effect ← Cause Connectors (Showing Result)

| Connector | Grammar | Example |
|-----------|---------|---------|
| therefore | clause; therefore, clause | The gain was insufficient; **therefore**, a second stage was added. |
| consequently | clause; consequently, clause | The junction overheated; **consequently**, the device failed. |
| as a result | clause. As a result, clause | Crosstalk increased. **As a result**, the BER degraded. |
| hence | clause; hence + noun/clause | The resistance increased; **hence** the voltage drop across the trace. |
| thus | clause; thus, clause | The bandwidth is limited; **thus**, the data rate cannot exceed 1 Gbps. |
| so | clause, so clause | The load increased, **so** the current exceeded the rated value. |

### 8.4 Verb-Based Cause and Effect

| Verb/Phrase | Direction | Example |
|-------------|-----------|---------|
| causes | cause → effect | High dv/dt **causes** electromagnetic interference. |
| leads to | cause → effect | Excessive heat **leads to** solder joint failure. |
| results in | cause → effect | Increasing the modulation order **results in** higher spectral efficiency. |
| is caused by | effect ← cause | The ringing **is caused by** parasitic inductance in the trace. |
| results from | effect ← cause | The phase shift **results from** the propagation delay. |
| gives rise to | cause → effect | The nonlinearity **gives rise to** harmonic distortion. |
| contributes to | cause → effect | Skin effect **contributes to** increased AC resistance at high frequencies. |

### 8.5 AI/ML Engineering Examples (Cause and Effect)

- **Because** the training data contained gender bias, the model's predictions exhibited discriminatory patterns.
- Increasing the number of transformer layers **results in** improved representational capacity but higher computational cost.
- The model hallucinated factual claims; **consequently**, a retrieval-augmented generation (RAG) pipeline was added.
- **Due to** catastrophic forgetting, the fine-tuned model lost performance on previously learned tasks.
- Gradient vanishing **leads to** poor training of deep networks; **therefore**, residual connections were introduced.
- **Since** the vocabulary did not include domain-specific tokens, the tokeniser split technical terms into subword units.
- Overfitting **is caused by** insufficient regularisation when training on small datasets.
- The attention mechanism **gives rise to** interpretable weight distributions, **thus** enabling analysis of model behaviour.

### 8.6 Exercise: Connect Cause-Effect Pairs

Match each cause with its effect and write a complete sentence using an appropriate connector. Use a different connector for each sentence.

**Causes:**
a. The antenna was placed near a metal surface.
b. The switching frequency was increased to 500 kHz.
c. The optical fibre was bent beyond its minimum radius.
d. The feedback resistor value was too high.
e. The solar irradiance dropped below 200 W/m².
f. The clock signal experienced jitter.
g. The DC bus capacitor degraded over time.
h. The modulation scheme was changed from BPSK to 16-QAM.

**Effects:**
i. The data rate increased fourfold.
ii. The radiation pattern was significantly distorted.
iii. The inductor size was reduced.
iv. The voltage ripple increased.
v. The amplifier gain exceeded the design specification.
vi. The bit error rate increased.
vii. Signal attenuation increased sharply.
viii. The PV inverter entered standby mode.

### Answer Key — Exercise 8.6 (Sample Answers)

1. (a→ii) **Because** the antenna was placed near a metal surface, the radiation pattern was significantly distorted.
2. (b→iii) Increasing the switching frequency to 500 kHz **resulted in** a reduction in inductor size.
3. (c→vii) The optical fibre was bent beyond its minimum radius; **consequently**, signal attenuation increased sharply.
4. (d→v) **Due to** the excessively high feedback resistor value, the amplifier gain exceeded the design specification.
5. (e→viii) **Since** the solar irradiance dropped below 200 W/m², the PV inverter entered standby mode.
6. (f→vi) Clock jitter **led to** an increase in the bit error rate.
7. (g→iv) **As** the DC bus capacitor degraded over time, the voltage ripple increased.
8. (h→i) The modulation scheme was changed from BPSK to 16-QAM; **therefore**, the data rate increased fourfold.

---

## 9. Technical Noun Phrases

### 9.1 Understanding Complex Noun Phrases

Engineering English uses long noun phrases that pack multiple modifiers before a head noun. These are efficient but difficult to parse for non-native speakers.

**Structure:** (Modifier₁) + (Modifier₂) + ... + **Head Noun**

The head noun is always the **last** word. Everything before it modifies or describes it.

### 9.2 Examples and Analysis

| Noun Phrase | Head Noun | Modifiers (working backwards) |
|-------------|-----------|-------------------------------|
| low-noise high-gain differential **amplifier** | amplifier | differential (type), high-gain (characteristic), low-noise (characteristic) |
| three-phase voltage source **inverter** | inverter | voltage source (type of source), three-phase (number of phases) |
| deep reinforcement learning-based **controller** | controller | learning-based (design approach), reinforcement (type of learning), deep (depth of network) |
| 28 GHz millimetre-wave phased array **antenna** | antenna | phased array (architecture), millimetre-wave (frequency band), 28 GHz (specific frequency) |
| pulse-width modulated full-bridge **converter** | converter | full-bridge (topology), pulse-width modulated (control method) |
| finite impulse response digital **filter** | filter | digital (domain), finite impulse response (type) |

### 9.3 AI/ML Engineering Examples (Noun Phrases)

| Noun Phrase | Head Noun | Modifiers (working backwards) |
|-------------|-----------|-------------------------------|
| multi-head self-attention **mechanism** | mechanism | self-attention (type), multi-head (architecture) |
| pre-trained large language **model** | model | language (domain), large (scale), pre-trained (training status) |
| reinforcement learning from human feedback **pipeline** | pipeline | human feedback (source), reinforcement learning from (method) |
| bidirectional encoder representations from transformers (**BERT**) **architecture** | architecture | from transformers (basis), encoder representations (function), bidirectional (direction) |
| low-rank adaptation fine-tuning **method** | method | fine-tuning (purpose), low-rank adaptation (technique) |
| retrieval-augmented generation **framework** | framework | generation (function), retrieval-augmented (enhancement) |
| graph neural network-based fault detection **system** | system | fault detection (function), graph neural network-based (implementation) |

### 9.4 How to Construct Technical Noun Phrases

**Read right to left** to understand; **build left to right** to construct:

1. Start with the head noun: **controller**
2. Add the most essential classifier: **PID controller**
3. Add further specification: **adaptive PID controller**
4. Add more detail: **fuzzy logic-based adaptive PID controller**

### 9.5 Hyphenation Rules

| Rule | Example | Explanation |
|------|---------|-------------|
| Compound adjective before noun | **high-frequency** oscillator | Two words acting as one adjective |
| Number + unit before noun | **50-ohm** transmission line | Measurement acting as adjective |
| Noun + participle before noun | **voltage-controlled** oscillator | Shows the relationship |
| Do NOT hyphenate after noun | The oscillator is voltage controlled. | Only hyphenate before the noun |
| Adverb + adjective: no hyphen | **highly efficient** converter | Adverbs ending in -ly are not hyphenated |
| Well-known compound terms | phase-locked loop, field-programmable gate array | Established terms |

### 9.6 Exercise: Parse and Explain Complex Noun Phrases

For each noun phrase, identify: (a) the head noun, (b) each modifier and what it specifies, and (c) write a paraphrase in plain English.

1. dual-band circularly polarised microstrip patch antenna
2. maximum power point tracking algorithm
3. zero-voltage switching quasi-resonant DC-DC converter
4. reconfigurable intelligent surface-assisted millimetre-wave communication system
5. lithium iron phosphate battery management system
6. model predictive torque control strategy
7. high-voltage direct current transmission line
8. software-defined radio-based spectrum sensing platform

### Answer Key — Exercise 9.6

1. **Head noun:** antenna
   - **Modifiers:** patch (physical structure), microstrip (fabrication technology), circularly polarised (polarisation type), dual-band (frequency coverage)
   - **Paraphrase:** An antenna made using microstrip patch technology that operates at two frequency bands with circular polarisation.

2. **Head noun:** algorithm
   - **Modifiers:** tracking (function), maximum power point (what is tracked)
   - **Paraphrase:** An algorithm that tracks the point of maximum power extraction (typically in photovoltaic systems).

3. **Head noun:** converter
   - **Modifiers:** DC-DC (conversion type), quasi-resonant (switching approach), zero-voltage switching (specific switching condition)
   - **Paraphrase:** A DC-DC converter that uses quasi-resonant operation with zero-voltage switching to reduce losses.

4. **Head noun:** system
   - **Modifiers:** communication (system type), millimetre-wave (frequency band), reconfigurable intelligent surface-assisted (enabling technology)
   - **Paraphrase:** A communication system operating at millimetre-wave frequencies that is assisted by a reconfigurable intelligent surface.

5. **Head noun:** system
   - **Modifiers:** management (function), battery (what is managed), lithium iron phosphate (battery chemistry)
   - **Paraphrase:** A system that manages lithium iron phosphate batteries (monitoring state of charge, temperature, balancing, etc.).

6. **Head noun:** strategy
   - **Modifiers:** control (type of strategy), torque (what is controlled), model predictive (control methodology)
   - **Paraphrase:** A control strategy that uses model predictive methods to control motor torque.

7. **Head noun:** line
   - **Modifiers:** transmission (function), direct current (type of current), high-voltage (voltage level)
   - **Paraphrase:** A transmission line that carries high-voltage direct current (HVDC).

8. **Head noun:** platform
   - **Modifiers:** spectrum sensing (function), software-defined radio-based (implementation technology)
   - **Paraphrase:** A platform for sensing radio spectrum that is built using software-defined radio technology.



---

## 10. Articles in Technical English

### 10.1 When to Use A/An, The, or No Article

| Rule | Example |
|------|---------|
| **a/an** — first mention, one of many | We propose **a** novel topology. |
| **the** — specific/already mentioned | **The** proposed topology reduces losses. |
| **the** — unique in context | **The** output of the amplifier is distorted. |
| **No article** — plural general | **Ø** Capacitors store energy in electric fields. |
| **No article** — uncountable general | **Ø** Bandwidth is a limited resource. |
| **the** — superlatives | **The** highest efficiency was recorded at 25°C. |
| **No article** — figures/tables/equations | **Ø** Figure 3 shows the response. |

### 10.2 Common Patterns in Engineering Papers

- **the** proposed method / **the** conventional approach / **the** simulation results
- **a** novel approach / **a** 50 Ω load / **an** FPGA-based implementation
- **Ø** Figure 5 / **Ø** Table II / **Ø** Equation (3)
- **the** University of Manchester (specific institution)
- **Ø** MATLAB / **Ø** VHDL (software/language names)

### 10.3 Tricky Cases

| Case | Rule | Example |
|------|------|---------|
| Abbreviations | Use article based on pronunciation | **an** SNR improvement, **a** USB port, **an** RF signal |
| "of" phrases | Usually need "the" | **The** output of **the** converter |
| After "using" | Often no article needed | ...designed using **Ø** CMOS technology |
| Measurements | No article with units | measured at **Ø** 5 GHz |
| Named theorems | Usually no article | according to **Ø** Nyquist's theorem |

### 10.4 AI/ML Engineering Examples (Articles)

- We propose **a** novel attention mechanism for long-sequence modelling.
- **The** pre-trained model was fine-tuned on **a** domain-specific corpus.
- **Ø** Large language models require significant computational resources for **Ø** training.
- **The** loss function converged after **Ø** 50,000 steps.
- **An** LLM-based approach was used for **Ø** automated code generation.
- **The** transformer architecture, which uses **Ø** self-attention, has replaced **Ø** RNNs in most NLP tasks.
- **A** dropout rate of 0.1 was applied to all **Ø** hidden layers.
- **The** accuracy of **the** model on **the** test set was 94.3%.

### 10.5 Exercise: Insert Correct Articles

Insert **a**, **an**, **the**, or **Ø** (no article) in each blank.

1. We present _____ new method for reducing _____ harmonic distortion in _____ power inverters.
2. _____ proposed antenna operates at _____ 2.4 GHz.
3. _____ Figure 6 shows _____ frequency response of _____ filter.
4. _____ efficiency of _____ system was measured using _____ precision power analyser.
5. _____ OFDM is widely used in _____ modern wireless communication systems.
6. _____ SNR was found to be _____ limiting factor.
7. We implemented _____ algorithm on _____ FPGA.
8. _____ results indicate that _____ bandwidth increases with _____ substrate thickness.
9. _____ Equation (7) describes _____ relationship between _____ voltage and _____ current.
10. This is _____ first study to investigate _____ effect of _____ humidity on _____ GaN device reliability.

### Answer Key — Exercise 10.5

1. **a** new method for reducing **Ø** harmonic distortion in **Ø** power inverters.
2. **The** proposed antenna operates at **Ø** 2.4 GHz.
3. **Ø** Figure 6 shows **the** frequency response of **the** filter.
4. **The** efficiency of **the** system was measured using **a** precision power analyser.
5. **Ø** OFDM is widely used in **Ø** modern wireless communication systems.
6. **The** SNR was found to be **the** limiting factor.
7. We implemented **the** algorithm on **an** FPGA.
8. **The** results indicate that **the** bandwidth increases with **Ø** substrate thickness.
9. **Ø** Equation (7) describes **the** relationship between **Ø** voltage and **Ø** current.
10. This is **the** first study to investigate **the** effect of **Ø** humidity on **Ø** GaN device reliability.



---

## 11. Prepositions in Engineering

### 11.1 Common Preposition Combinations

| Expression | Example |
|-----------|---------|
| increase **in** | an increase **in** efficiency |
| decrease **in** / decrease **of** | a decrease **in** noise / a decrease **of** 3 dB |
| proportional **to** | The current is proportional **to** the voltage. |
| dependent **on** | The gain is dependent **on** the bias current. |
| independent **of** | The output is independent **of** load variations. |
| connected **to** | The load is connected **to** the output terminal. |
| applied **to** | A voltage is applied **to** the gate. |
| divided **by** | The power is divided **by** the resistance. |
| multiplied **by** | The frequency is multiplied **by** a factor of four. |
| measured **in** | Power is measured **in** watts. |
| operates **at** | The device operates **at** 3.3 V. |
| consists **of** | The system consists **of** three stages. |
| results **in** | This results **in** higher distortion. |
| results **from** | The error results **from** quantisation. |
| sensitive **to** | The circuit is sensitive **to** temperature variations. |
| compatible **with** | The interface is compatible **with** USB 3.0. |

### 11.2 AI/ML Engineering Examples (Prepositions)

- The model was trained **on** a dataset of 500 billion tokens.
- Performance depends **on** the quality of the training data.
- The output is sensitive **to** changes in temperature and input distribution.
- The encoder consists **of** 12 self-attention layers.
- The improvement results **from** the use of multi-head attention.
- The embeddings are projected **into** a lower-dimensional space.
- The model is compatible **with** various downstream tasks.
- Attention weights are computed **between** all pairs of tokens **in** the sequence.

### 11.3 Exercise: Fill in the Correct Prepositions

1. The output power is proportional _____ the square of the voltage.
2. The resonant frequency depends _____ the inductance and capacitance values.
3. The sensor operates _____ temperatures ranging from −40°C to 85°C.
4. The proposed method results _____ a 15% improvement in throughput.
5. The inductor is connected _____ the switch node and the output capacitor.
6. The efficiency is measured _____ percent.
7. The voltage was divided _____ a resistive network.
8. There was a significant increase _____ the bit error rate at low SNR.
9. The oscillator frequency is independent _____ supply voltage variations.
10. The filter is sensitive _____ component tolerances.

### Answer Key — Exercise 11.3

1. **to**
2. **on**
3. **at**
4. **in**
5. **between** (note: "connected to" for single endpoint; "connected between" for two points)
6. **in**
7. **by**
8. **in**
9. **of**
10. **to**



---

## 12. Participial Phrases

### 12.1 Present Participle (-ing) Phrases

Used to show method, simultaneous action, or additional information concisely.

- **Using the proposed method**, we achieved a 20% reduction in power consumption.
- **Applying Kirchhoff's voltage law**, we can derive the transfer function.
- **Increasing the switching frequency**, the designer can reduce the inductor size.
- **Operating at 5 GHz**, the amplifier delivers 30 dBm output power.

### 12.2 Past Participle (-ed / irregular) Phrases

Used to replace passive relative clauses, showing what was done or how something relates.

- **Compared with conventional approaches**, the proposed method reduces latency by 45%.
- **Implemented on a Xilinx FPGA**, the controller achieved real-time performance.
- **Measured at room temperature**, the noise figure was 1.8 dB.
- **Fabricated using 0.18 μm CMOS technology**, the chip occupies 1.2 mm².

### 12.3 Why Participial Phrases Are Common in Papers

- They reduce word count (journals have page limits)
- They create a formal, concise tone
- They avoid repetitive sentence structures
- They are especially frequent in Methods and Results sections

### 12.4 AI/ML Engineering Examples (Participial Phrases)

**Present participle (-ing):**
- **Leveraging pre-trained representations**, the model achieves state-of-the-art accuracy with limited labelled data.
- **Using a cosine annealing schedule**, we reduced the learning rate gradually over training.
- **Processing input sequences in parallel**, the transformer architecture enables significant speedups over recurrent models.

**Past participle (-ed):**
- **Trained on a diverse multilingual corpus**, the model supports 104 languages without explicit language identification.
- **Evaluated on the GLUE benchmark**, the proposed approach outperformed all baselines by a significant margin.
- **Initialised with weights from a pre-trained checkpoint**, the fine-tuned model converged in fewer than 5 epochs.
- **Combined with retrieval-augmented generation**, the LLM produced more factually grounded responses.

### 12.5 Caution: Dangling Participles

The participle must refer to the subject of the main clause.

| ❌ Incorrect (dangling) | ✅ Correct |
|------------------------|-----------|
| Using a spectrum analyser, the signal was measured. *(Who used it?)* | Using a spectrum analyser, **we** measured the signal. |
| Compared with the baseline, a 10% improvement was observed. *(What is compared?)* | Compared with the baseline, **the proposed method** showed a 10% improvement. |

### 12.6 Exercise: Rewrite Using Participial Phrases

Rewrite each sentence pair as a single sentence using a participial phrase.

1. We applied a Hamming window to the data. We reduced spectral leakage.
2. The filter was designed using Butterworth approximation. It provides a maximally flat passband.
3. The results were compared with published data. The results show excellent agreement.
4. The algorithm uses gradient descent optimisation. It converges within 50 iterations.
5. The antenna was printed on an FR-4 substrate. The antenna achieves a gain of 6 dBi.
6. We considered the thermal constraints. We selected a heat sink rated at 2.5°C/W.

### Answer Key — Exercise 12.6

1. **Applying a Hamming window to the data**, we reduced spectral leakage.
2. **Designed using Butterworth approximation**, the filter provides a maximally flat passband.
3. **Compared with published data**, the results show excellent agreement.
4. **Using gradient descent optimisation**, the algorithm converges within 50 iterations.
5. **Printed on an FR-4 substrate**, the antenna achieves a gain of 6 dBi.
6. **Considering the thermal constraints**, we selected a heat sink rated at 2.5°C/W.

---

## Quick Reference Summary

| Grammar Point | Primary Use in Engineering Writing |
|---------------|-----------------------------------|
| Tenses | Signalling time frame and certainty of claims |
| Passive voice | Focusing on processes and results |
| Modal verbs | Expressing degrees of certainty and obligation |
| Hedging | Avoiding overclaims in research |
| Conditionals | Discussing design trade-offs and hypotheticals |
| Relative clauses | Adding specification and detail |
| Comparatives | Evaluating methods and results |
| Cause and effect | Explaining mechanisms and outcomes |
| Noun phrases | Building compact technical descriptions |
| Articles | Signalling specificity and generality |
| Prepositions | Expressing precise relationships |
| Participial phrases | Writing concisely in formal papers |
| Prompt writing | Communicating precisely with AI systems |

---

## 13. Writing Prompts as a Communication Skill

### 13.1 Why This Matters

In modern engineering practice, communicating with AI systems (large language models, code assistants, and automated tools) has become a daily task. Writing effective prompts requires **the same skills** as writing effective technical documents:

- **Precision** — ambiguous prompts produce ambiguous outputs, just as ambiguous specifications produce faulty designs.
- **Clarity** — a well-structured prompt eliminates guesswork, like a well-written lab report.
- **Appropriate register** — matching the formality and technicality to the desired output.
- **Logical structure** — organising information so the reader (human or machine) can follow your intent.

> Poor prompts = poor results. This is the same principle behind poorly written specifications leading to flawed implementations.

**Key insight:** If you can write a clear Methods section, you can write a clear prompt. Both require you to specify context, constraints, and desired outcomes.

### 13.2 Grammar Patterns in Effective Prompts

#### Imperative Mood

The imperative is the dominant mood in prompt writing—direct commands that specify the task.

| Imperative Verb | Example Prompt Fragment |
|-----------------|------------------------|
| Explain | **Explain** the Nyquist stability criterion for a first-year EE audience. |
| Summarize | **Summarize** the key findings of this paper in three bullet points. |
| Compare | **Compare** the advantages and disadvantages of buck and boost converters. |
| List | **List** five applications of GaN transistors in power electronics. |
| Derive | **Derive** the transfer function of a second-order low-pass filter. |
| Analyse | **Analyse** the following circuit for potential EMI issues. |
| Rewrite | **Rewrite** this paragraph using appropriate hedging language. |

**Grammar note:** Imperative sentences have no explicit subject ("you" is implied). The verb is in base form.

#### Conditional Structures

Conditionals specify contingent behaviour—essential for complex, multi-step prompts.

- **If** the user provides a circuit diagram, **then** identify the topology and explain its operation.
- **If** the input is in Persian, **translate** it to academic English. **If** it is already in English, **check** the grammar.
- **When** the calculation involves complex numbers, **show** both rectangular and polar forms.
- **Unless** otherwise specified, **assume** a supply voltage of 3.3 V.

#### Role Assignment (Second Person + Present Simple)

Assigning a role establishes context and expertise level.

- **You are** an expert in power electronics with 20 years of experience.
- **You are** a patient university lecturer explaining concepts to second-year students.
- **You are** a peer reviewer for IEEE Transactions on Power Electronics.
- **You are** a technical editor checking for grammar and clarity.

**Grammar note:** Role assignment uses present simple ("You are...") to establish an ongoing state, not a one-time action.

#### Specifying Constraints (Prepositional and Participial Phrases)

Constraints narrow the output and are expressed using familiar grammar structures.

| Constraint Type | Grammar Structure | Example |
|----------------|-------------------|---------|
| Length | Prepositional phrase | **In no more than 200 words**, explain... |
| Source restriction | Participial phrase | **Using only peer-reviewed sources**, list... |
| Audience | Prepositional phrase | **For an audience of undergraduate EE students**, describe... |
| Format | Prepositional phrase | **In the form of a table**, compare... |
| Exclusion | Without + gerund | **Without using jargon**, explain... |
| Scope | Present participle | **Focusing only on the thermal aspects**, analyse... |

#### Providing Context (Tense Patterns)

| Tense | Function in Prompt | Example |
|-------|-------------------|---------|
| Present perfect | Background/what has been done | "I **have written** a draft abstract for an IEEE conference paper." |
| Present simple | Current task/situation | "The abstract **covers** our work on GaN-based inverters." |
| Past simple | Specific completed action | "The reviewer **suggested** that the methodology section needs revision." |
| Future (will/need to) | Desired outcome | "I **need** you to check the grammar and improve the hedging language." |

### 13.3 Common Prompt Structures

| Structure | Example | Grammar Point |
|-----------|---------|---------------|
| Role + Task | "You are an EE professor. **Explain** the concept of skin effect to a second-year student." | Imperative mood |
| Context + Question | "**Given that** the transistor is operating in saturation, **what** is the expected collector current?" | Conditional + interrogative |
| Constraint + Action | "**Without using jargon**, **describe** how a PLL works." | Participial phrase + imperative |
| Background + Task | "I **have collected** data from a 5 kW solar inverter. **Analyse** the efficiency trends." | Present perfect + imperative |
| Condition + Response | "**If** the student gives an incorrect answer, **provide** a hint rather than the full solution." | Conditional + imperative |
| Exclusion + Action | "**Excluding** cost considerations, **compare** SiC and GaN for high-frequency applications." | Present participle + imperative |
| Format + Content | "**In a numbered list**, **identify** the sources of noise in this amplifier circuit." | Prepositional phrase + imperative |

### 13.4 From Weak to Strong: Prompt Improvement Examples

| ❌ Weak Prompt | Problem | ✅ Strong Prompt |
|---------------|---------|-----------------|
| "Tell me about transformers." | Too vague—electrical or neural network? No context. | "**Explain** how the self-attention mechanism in transformer neural networks differs from RNN-based sequence processing. **Use** examples relevant to signal processing." |
| "Fix my abstract." | No text provided, no criteria specified. | "**Review** the following abstract for grammar, hedging, and tense consistency. **Suggest** corrections with explanations. [abstract text]" |
| "How does a buck converter work?" | No audience level, no constraints. | "**For a student who has completed Circuit Theory I**, **explain** the operating principle of a buck converter. **Include** a description of both CCM and DCM modes." |
| "Compare these." | No subjects, no criteria. | "**Compare** the MPPT algorithms P&O and InC **in terms of** tracking speed, steady-state oscillation, and implementation complexity. **Present** the comparison in a table." |

### 13.5 Exercise: Grammar Analysis of Prompts

**Instructions:** Analyse the following 10 prompts. For each one: (a) identify all grammar structures used, and (b) write an improved version that is more grammatically precise and effective.

1. "Explain transformers."
2. "You are a helpful assistant. Help me with my homework."
3. "If I have a circuit with a resistor and capacitor, what happens?"
4. "Summarize this paper I read about batteries."
5. "Tell me about noise in amplifiers without being too technical."
6. "Compare MOSFET and IGBT."
7. "I need help writing the introduction to my paper about renewable energy."
8. "You are an expert. Check my grammar."
9. "Given a 5V supply, design a circuit."
10. "List advantages of using AI in power systems."

### Answer Key — Exercise 13.5 (Sample Answers)

1. **Analysis:** Imperative (Explain) + bare noun (no specification). **Improved:** "**Explain** the operation of a transformer neural network, **focusing on** the self-attention mechanism. **Assume** the reader has basic knowledge of linear algebra." *(Added: participial constraint, imperative for audience specification)*

2. **Analysis:** Role assignment (You are) + imperative (Help) — too vague, no task specification. **Improved:** "You are a patient electrical engineering tutor. **Explain** Kirchhoff's current law with three worked examples **suitable for** a first-year undergraduate." *(Added: specific role, specific task, constraint)*

3. **Analysis:** First conditional (If... what happens) — missing values, no context. **Improved:** "**If** a 10 kΩ resistor is connected in series with a 100 nF capacitor across a 5 V DC supply, **describe** the voltage across the capacitor as a function of time. **Derive** the time constant." *(Added: specific values, precise task verbs)*

4. **Analysis:** Imperative (Summarize) + vague reference (this paper). **Improved:** "**Summarize** the following paper on lithium-ion battery degradation mechanisms **in no more than** 150 words. **Highlight** the main contribution and limitations. [paste text]" *(Added: length constraint, specific focus areas, actual text)*

5. **Analysis:** Imperative (Tell) + prepositional constraint (without being too technical) — imprecise. **Improved:** "**Explain** the main sources of noise in operational amplifier circuits **for an audience of** second-year EE students who have completed Circuits I. **Avoid** equations; **use** analogies where possible." *(Added: specific audience, specific constraints)*

6. **Analysis:** Imperative (Compare) + two nouns — no criteria, no format. **Improved:** "**Compare** MOSFETs and IGBTs **in terms of** switching speed, conduction losses, voltage rating, and typical applications. **Present** the comparison **in a table** with a brief concluding recommendation for a 10 kW inverter design." *(Added: comparison criteria, format, application context)*

7. **Analysis:** Declarative (I need help) + gerund (writing) — passive request, no details. **Improved:** "I **have written** a draft introduction for a paper on maximum power point tracking in photovoltaic systems. **Review** it for logical flow, tense consistency, and appropriate hedging. **Suggest** improved topic sentences for each paragraph. [paste draft]" *(Added: present perfect background, specific review criteria, clear task)*

8. **Analysis:** Role assignment + imperative — too broad, no text provided. **Improved:** "You are a technical editor for IEEE Transactions on Power Electronics. **Check** the following abstract for grammar errors, paying special attention to article usage, tense consistency, and passive voice construction. **Explain** each correction. [paste abstract]" *(Added: specific role, specific grammar focus, explanation requirement)*

9. **Analysis:** Past participle (Given) + imperative (design) — underspecified. **Improved:** "**Given** a 5 V supply and a load requiring 3.3 V at 500 mA, **design** a buck converter. **Specify** the inductor value, switching frequency, and duty cycle. **Assume** continuous conduction mode." *(Added: complete specifications, specific deliverables, assumptions)*

10. **Analysis:** Imperative (List) + noun phrase — acceptable but could be more specific. **Improved:** "**List** five advantages of using AI/ML techniques in power system fault detection. **For each advantage**, **provide** a one-sentence explanation with a reference to a specific technique (e.g., neural networks, random forests)." *(Added: number, scope narrowing, explanation requirement)*

### 13.6 Exercise: Writing Effective Prompts

**Instructions:** For each of the following engineering tasks, write a grammatically precise and effective prompt. Your prompt should include: (a) appropriate role assignment (if helpful), (b) clear imperative verbs, (c) specific constraints, and (d) context using appropriate tenses.

1. Getting an explanation of Fourier transforms for undergraduates
2. Summarising a paper on battery management systems
3. Comparing two power converter topologies
4. Translating a Persian technical paragraph to academic English
5. Checking grammar in a draft abstract

### Answer Key — Exercise 13.6 (Sample Answers)

1. **Fourier Transforms Explanation:**
   "You are a signals and systems lecturer teaching second-year EE students. **Explain** the Fourier transform **starting from** the concept of representing signals as sums of sinusoids. **Include**: (a) the intuition behind the transform, (b) the mathematical definition, (c) two worked examples—one with a rectangular pulse and one with a decaying exponential. **Use** clear step-by-step derivations. **In no more than** 800 words, **ensure** the explanation bridges time-domain and frequency-domain thinking."

   *Grammar structures used: Role assignment (present simple), imperative (Explain, Include, Use, Ensure), participial phrase (starting from), prepositional constraints (In no more than), listing format.*

2. **Battery Management System Paper Summary:**
   "I **have read** a paper on state-of-health estimation in lithium-ion battery management systems. **Summarize** the paper below **in** 200–250 words, **covering**: (a) the problem statement, (b) the proposed method, (c) the key results, and (d) the main limitations. **Use** present simple for general claims and past simple for specific experimental findings. **Maintain** appropriate hedging where the authors express uncertainty. [paste paper text]"

   *Grammar structures used: Present perfect background, imperative (Summarize, Use, Maintain), prepositional constraints (in 200–250 words), listing, tense specification.*

3. **Power Converter Topology Comparison:**
   "**Compare** the half-bridge and full-bridge isolated DC-DC converter topologies **for a** 1 kW, 400 V to 48 V application. **Evaluate** them **in terms of**: (a) component count and cost, (b) transformer utilisation, (c) efficiency at partial load, (d) control complexity, and (e) suitability for bidirectional operation. **Present** the comparison in a table, **followed by** a 100-word recommendation stating which topology you **would** select and why."

   *Grammar structures used: Imperative (Compare, Evaluate, Present), prepositional phrases (for a... application, in terms of, in a table), participial phrase (followed by), conditional (would select).*

4. **Persian-to-English Technical Translation:**
   "You are a professional scientific translator specialising in electrical engineering texts. **Translate** the following Persian paragraph into formal academic English **suitable for** an IEEE journal submission. **Ensure** that: (a) technical terminology is translated accurately using standard English equivalents, (b) the passive voice is used where appropriate for Methods descriptions, (c) hedging language is preserved where the original text expresses uncertainty, and (d) the resulting English text is grammatically correct and reads naturally. **If** any term has multiple possible English translations, **provide** the most common one and note the alternative in brackets. [paste Persian text]"

   *Grammar structures used: Role assignment, imperative (Translate, Ensure, provide), participial constraint (suitable for), conditional (If... provide), passive voice in constraint description, listing.*

5. **Grammar Check of Draft Abstract:**
   "You are a technical editor for a peer-reviewed EE journal. I **have written** a draft abstract for a paper on neural network-based predictive maintenance for induction motors. **Check** the following abstract for: (a) tense consistency (present simple for general claims, past simple for methods and results), (b) correct article usage (a/an/the/Ø), (c) appropriate hedging (no overclaims), (d) passive vs. active voice balance, and (e) any other grammatical errors. **For each error**, **underline** the problematic text, **explain** the rule, and **provide** a corrected version. [paste abstract]"

   *Grammar structures used: Role assignment, present perfect background, imperative (Check, underline, explain, provide), prepositional phrases for scope, listing, tense specification within constraints.*

---

*End of Grammar for Engineers Appendix*

