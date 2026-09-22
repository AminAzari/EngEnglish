# Scientific and Technical English for Electrical Engineering

## Part 2: Writing and Academic Communication (Weeks 5–9)

**Course Level:** Undergraduate Electrical Engineering  
**Target Proficiency:** B2 → C1 (CEFR)  
**Focus:** Technical writing, academic communication, and professional correspondence  

---

# WEEK 5: Technical Writing Fundamentals

## Learning Objectives

By the end of this week, students will be able to:

1. Distinguish between active and passive voice and apply each appropriately in engineering writing
2. Write clear, precise technical sentences free of ambiguity and unnecessary words
3. Structure coherent technical paragraphs with topic sentences, supporting evidence, and concluding sentences
4. Use cohesion devices to create logical flow between sentences and paragraphs
5. Apply scientific writing style conventions appropriate for EE publications

---

## 5.1 Clear Technical Sentences: Active vs. Passive Voice

### When to Use Active Voice

Active voice emphasizes the **agent** (who or what performs the action). Use it when:

- The doer of the action is important
- Describing what researchers did (methodology sections)
- Writing instructions or procedures
- Making recommendations

| Active Voice Example | Context |
|---------------------|---------|
| We designed a low-pass Butterworth filter with a cutoff frequency of 1 kHz. | Methodology |
| The controller adjusts the output voltage in real time. | System description |
| Engineers must verify the circuit before power-up. | Instructions |
| This paper proposes a novel MPPT algorithm for photovoltaic systems. | Paper introduction |

### When to Use Passive Voice

Passive voice emphasizes the **action or result** rather than the doer. Use it when:

- The agent is unknown, obvious, or unimportant
- Describing general processes or established facts
- Maintaining objectivity in results sections
- The focus should be on the object receiving the action

| Passive Voice Example | Context |
|----------------------|---------|
| The signal was sampled at 44.1 kHz. | Results — focus on the signal |
| Three-phase transformers are widely used in power distribution networks. | General fact |
| The prototype was tested under varying load conditions. | Methodology — agent obvious |
| The data were collected over a 24-hour period. | Results |

### Common Mistakes

> ❌ **Overusing passive:** "It was found that the voltage was increased when the resistance was decreased."  
> ✅ **Better:** "The voltage increased when resistance decreased." (Active, concise)

> ❌ **Inappropriate active:** "I think the circuit is good."  
> ✅ **Better:** "The simulation results confirm that the circuit meets the design specifications." (Objective, evidence-based)

---

## 5.2 Precision and Avoiding Ambiguity

### Principles of Precise Technical Writing

1. **Use specific quantities** instead of vague terms
2. **Define technical terms** on first use
3. **Avoid pronouns with unclear antecedents**
4. **Specify units** for all measurements
5. **Use unambiguous modifiers**

### Examples: Vague vs. Precise

| ❌ Vague / Ambiguous | ✅ Precise / Clear |
|---------------------|-------------------|
| The system is fast. | The system achieves a response time of 2.3 ms. |
| The voltage was high. | The output voltage reached 48 V. |
| The filter works well. | The filter attenuates frequencies above 5 kHz by at least 40 dB. |
| It improved significantly. | The bit error rate decreased from 10⁻³ to 10⁻⁶. |
| The temperature affects the component. | An ambient temperature exceeding 85°C degrades the MOSFET's switching performance by 15%. |
| This method is better. | This method reduces computational complexity by 30% compared to the FFT-based approach. |

### Ambiguous Pronoun References

> ❌ "The amplifier was connected to the filter. **It** had a gain of 20 dB."  
> (What does "it" refer to — the amplifier or the filter?)

> ✅ "The amplifier was connected to the filter. **The amplifier** had a gain of 20 dB."

---

## 5.3 Avoiding Unnecessary Words (Conciseness)

### Wordy vs. Concise Expressions

| ❌ Wordy | ✅ Concise |
|---------|-----------|
| due to the fact that | because |
| in order to | to |
| at the present time | currently / now |
| a large number of | many |
| in the event that | if |
| has the ability to | can |
| it is important to note that | notably / note that |
| for the purpose of | to / for |
| in spite of the fact that | although / despite |
| on a daily basis | daily |
| prior to the start of | before |
| in the majority of cases | usually / often |

### Example Revision

> ❌ "In order to achieve the purpose of reducing the amount of power that is consumed by the system on a daily basis, the implementation of a sleep mode was carried out."

> ✅ "To reduce daily power consumption, a sleep mode was implemented."

**Result:** 34 words → 10 words. Same meaning, much clearer.

---

## 5.4 Paragraph Structure

A well-structured technical paragraph follows this pattern:

```
┌─────────────────────────────────────────┐
│  1. TOPIC SENTENCE                      │
│     (Main idea of the paragraph)        │
├─────────────────────────────────────────┤
│  2. SUPPORTING SENTENCES                │
│     (Explanation, elaboration, detail)  │
├─────────────────────────────────────────┤
│  3. EVIDENCE                            │
│     (Data, citations, examples)         │
├─────────────────────────────────────────┤
│  4. CONCLUDING SENTENCE                 │
│     (Wrap-up, implication, transition)  │
└─────────────────────────────────────────┘
```

### Model Paragraph (Annotated)

> **[Topic Sentence]** Orthogonal Frequency Division Multiplexing (OFDM) offers significant advantages for broadband wireless communication systems. **[Supporting Sentence 1]** By dividing the available bandwidth into multiple orthogonal subcarriers, OFDM converts a frequency-selective fading channel into multiple flat-fading subchannels. **[Supporting Sentence 2]** This approach simplifies equalization, as each subchannel requires only a single-tap equalizer rather than a complex multi-tap structure. **[Evidence]** Empirical measurements in [3] demonstrate that OFDM-based systems achieve a 4 dB improvement in signal-to-noise ratio compared to single-carrier systems operating in multipath environments with delay spreads exceeding 5 μs. **[Concluding Sentence]** Consequently, OFDM has become the modulation scheme of choice for modern standards including IEEE 802.11 (Wi-Fi), LTE, and 5G NR.

---

## 5.5 Cohesion Devices

### Table of Cohesion Devices by Function

| Function | Devices | Example in EE Context |
|----------|---------|----------------------|
| **Addition** | moreover, furthermore, in addition, also | The converter achieves 95% efficiency. **Moreover**, it operates across a wide input voltage range. |
| **Contrast** | however, nevertheless, in contrast, on the other hand, whereas | A PID controller is simple to implement. **However**, it struggles with nonlinear systems. |
| **Cause/Effect** | therefore, consequently, as a result, thus, hence | The sampling rate was below the Nyquist frequency. **Consequently**, aliasing occurred. |
| **Similarity** | similarly, likewise, in the same way | Solar panels degrade under high temperatures. **Similarly**, battery capacity decreases in extreme heat. |
| **Example** | for example, for instance, specifically, namely | Several modulation schemes are used in 5G. **For example**, 256-QAM is employed for high-throughput scenarios. |
| **Sequence** | first, subsequently, finally, then, next | **First**, the raw signal is digitized. **Subsequently**, a digital filter removes noise. **Finally**, the clean signal is processed by the DSP. |
| **Summary** | in summary, overall, to conclude | **Overall**, the proposed algorithm reduces latency by 40% while maintaining acceptable error rates. |

### Usage Tips

> 💡 **Tip:** Do not begin every sentence with a cohesion device. Use them only where the logical relationship between sentences needs clarification.

> ⚠️ **Common Mistake:** Using "however" when "therefore" is needed (or vice versa). Always check whether you are expressing contrast or consequence.

---

## 5.6 Scientific Writing Style

### Rules for Scientific Style

| ❌ Avoid | ✅ Use Instead | Reason |
|---------|--------------|--------|
| The results were amazing. | The results demonstrate a 25% improvement. | No emotional language |
| Everyone knows that... | It is widely established that... [1] | No unsupported claims |
| This cool new method... | This novel method... | No informal language |
| The system kind of works. | The system operates within acceptable parameters. | No vague statements |
| The extremely powerful, highly efficient, remarkably fast processor... | The processor achieves 3.2 GHz clock speed with 92% efficiency. | No excessive adjectives |
| I believe this is correct. | The experimental results confirm this hypothesis. | Objective, evidence-based |

### Examples from EE Papers

**Signal Processing:**
> ❌ "The FFT is a really great algorithm that makes things way faster."  
> ✅ "The FFT reduces the computational complexity of the DFT from O(N²) to O(N log N), enabling real-time spectral analysis."

**Power Systems:**
> ❌ "The power grid has lots of problems with stability when there are too many renewables."  
> ✅ "High penetration of renewable energy sources introduces voltage and frequency instability in power grids due to their intermittent nature [4]."

**Telecommunications:**
> ❌ "5G is incredibly fast and will change everything."  
> ✅ "5G networks achieve peak data rates of 20 Gbps and latencies below 1 ms, enabling applications such as autonomous vehicles and remote surgery [7]."

---

## 5.7 Vocabulary Box

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Cohesion** | The grammatical and lexical linking within a text that holds it together | Good cohesion ensures the reader can follow the argument without confusion. |
| **Topic sentence** | The sentence that states the main idea of a paragraph | The topic sentence should appear at the beginning of a technical paragraph. |
| **Passive voice** | A sentence construction where the subject receives the action | "The circuit was tested" uses passive voice. |
| **Conciseness** | Expressing ideas in as few words as possible without losing meaning | Technical writing values conciseness over elaborate description. |
| **Ambiguity** | Having more than one possible interpretation | Ambiguity in specifications can lead to design errors. |
| **Transition** | A word or phrase that connects ideas between sentences or paragraphs | "However" is a transition that signals contrast. |
| **Objectivity** | Writing without personal bias or emotional language | Scientific writing requires objectivity and evidence-based claims. |

---

## 5.8 Exercises

### Exercise 1: Rewrite Informal Sentences into Formal Technical Style

Rewrite the following sentences to make them appropriate for an engineering research paper:

1. "The circuit board got really hot when we cranked up the power."
2. "We tried a bunch of different filters and the Butterworth one was the best."
3. "The antenna picks up signals pretty well in most directions."
4. "Solar panels are awesome because they give you free electricity."
5. "The robot arm moves around and grabs stuff."
6. "We hooked up the oscilloscope and saw some weird signals."
7. "The battery dies super fast when it's cold outside."
8. "This chip is way better than the old one."

**Model Answers:**

1. "The PCB temperature increased to 95°C when the input power was raised to 50 W."
2. "Among the evaluated filter topologies, the Butterworth filter exhibited the flattest passband response with a maximum ripple of 0.1 dB."
3. "The antenna achieves a gain of 5 dBi with a half-power beamwidth of 65° in the horizontal plane."
4. "Photovoltaic systems convert solar irradiance into electrical energy without fuel costs, reducing long-term operational expenditure."
5. "The robotic arm provides six degrees of freedom, enabling object manipulation within a 1.2 m reach radius."
6. "The oscilloscope measurements revealed unexpected harmonic components at 150 Hz and 250 Hz."
7. "Battery discharge rate increases by approximately 30% at ambient temperatures below −10°C."
8. "The new IC achieves a 45% reduction in power consumption compared to its predecessor while maintaining equivalent processing throughput."

---

### Exercise 2: Identify Topic Sentences and Cohesion Devices

Read the following paragraph and:
- (a) Underline the topic sentence
- (b) Circle all cohesion devices
- (c) Identify the function of each cohesion device (addition, contrast, cause/effect, etc.)

> Digital signal processing (DSP) has transformed modern telecommunications systems. **First**, DSP enables adaptive filtering, which allows receivers to adjust to changing channel conditions in real time. **Furthermore**, digital implementations provide superior noise immunity compared to analog counterparts, as quantized signals are less susceptible to thermal noise degradation. **For example**, a 16-bit ADC provides a theoretical signal-to-noise ratio of 98 dB, far exceeding what analog circuits typically achieve. **However**, DSP systems introduce computational latency, which may be unacceptable in ultra-low-latency applications such as high-frequency trading or real-time control loops. **Nevertheless**, advances in FPGA and ASIC technology have reduced processing delays to sub-microsecond levels. **Consequently**, DSP-based solutions now dominate in applications ranging from 5G base stations to medical imaging systems.

**Answers:**
- Topic sentence: "Digital signal processing (DSP) has transformed modern telecommunications systems."
- Cohesion devices: First (sequence), Furthermore (addition), For example (example), However (contrast), Nevertheless (contrast/concession), Consequently (cause/effect)

---

## 5.9 Activities

### Activity: Write a Technical Paragraph

**Topic:** "Advantages of OFDM in Wireless Communications"

**Instructions:**
1. Write a paragraph of 100–150 words
2. Begin with a clear topic sentence
3. Include at least 2 supporting sentences with specific technical details
4. Use at least 2 cohesion devices
5. End with a concluding sentence
6. Use formal scientific style throughout

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Clear topic sentence | /2 |
| Supporting details with specific data | /3 |
| Appropriate cohesion devices | /2 |
| Scientific style (no informal language) | /2 |
| Concluding sentence | /1 |
| **Total** | **/10** |

---

## 5.10 Homework

**Assignment:** Write 3 technical paragraphs (100–150 words each) on the following topics:

1. "The role of feedback in control systems"
2. "Challenges of integrating renewable energy into the power grid"
3. "Advantages of digital modulation over analog modulation"

**Requirements for each paragraph:**
- Clear topic sentence
- At least 3 supporting sentences
- At least 2 cohesion devices (underline them)
- At least 1 specific technical detail (number, measurement, or fact)
- Formal scientific style
- Concluding sentence

**Due:** Next class session

---

## 5.11 Tips and Common Mistakes

### ✅ Tips for Better Technical Writing

1. **Read your sentences aloud** — if you run out of breath, the sentence is too long
2. **One idea per sentence** — complex ideas need multiple sentences
3. **One main point per paragraph** — if the topic shifts, start a new paragraph
4. **Be specific** — replace "several," "some," "many" with actual numbers when possible
5. **Revise aggressively** — first drafts are always too wordy

### ❌ Common Mistakes to Avoid

| Mistake | Example | Fix |
|---------|---------|-----|
| Run-on sentences | "The filter was designed and then it was tested and the results showed improvement and..." | Break into separate sentences |
| Dangling modifiers | "Using MATLAB, the simulation was completed." (Who used MATLAB?) | "Using MATLAB, we completed the simulation." |
| Nominalizations | "The measurement of the voltage was performed." | "The voltage was measured." |
| Redundancy | "The end result" / "completely eliminated" | "The result" / "eliminated" |
| Hedging too much | "It seems that the results might possibly suggest..." | "The results indicate..." |

---


## 5.12 AI Writing Assistants — Tools and Boundaries

### Overview of AI Writing Tools

Artificial intelligence writing tools have become widely available. As an engineering student, you should understand what these tools can and cannot do.

| Tool | Type | What It Does |
|------|------|-------------|
| **ChatGPT** (OpenAI) | Large Language Model (LLM) | Generates text, answers questions, rewrites content |
| **Claude** (Anthropic) | Large Language Model (LLM) | Similar to ChatGPT; generates and revises text |
| **Grammarly AI** | Grammar + AI rewriting | Checks grammar, suggests style improvements, rewrites sentences |
| **LanguageTool** | Grammar checker | Identifies grammar, punctuation, and style errors |
| **QuillBot** | Paraphrasing tool | Rewrites sentences in different styles |
| **Writefull** | Academic writing AI | Suggests improvements specific to academic/scientific writing |

### What AI Writing Tools Are Good At

AI tools can genuinely help with:

- ✅ **Grammar correction** — fixing subject-verb agreement, articles, prepositions
- ✅ **Spelling and punctuation** — catching typos and formatting errors
- ✅ **Style suggestions** — recommending more formal or concise alternatives
- ✅ **Clarity improvement** — simplifying overly complex sentences
- ✅ **Translation assistance** — helping express technical ideas from Persian/Arabic to English
- ✅ **Formatting** — helping with consistent reference formatting

### What AI Writing Tools Are NOT

> ⚠️ **Critical Understanding:**
>
> AI tools are NOT replacements for:
> - **Thinking** — AI does not understand your circuit design or control system
> - **Understanding** — AI cannot verify whether a technical claim is correct in your specific context
> - **Original analysis** — AI cannot interpret YOUR experimental data or draw valid conclusions from YOUR measurements
> - **Engineering judgment** — AI cannot decide which design tradeoff is appropriate for your application
> - **Learning** — If AI writes your paragraph, YOU have not learned to write

**Example:**
> You design a buck converter and measure its efficiency at various loads. AI can help you write "The converter achieved 94.2% efficiency at full load" in better English, but AI **cannot** determine whether 94.2% is a good result for your topology, or why efficiency dropped at light loads. That requires YOUR understanding.

### The Spectrum of AI Assistance

AI assistance exists on a spectrum from acceptable to unacceptable:

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ✅ ACCEPTABLE          │  ⚠️ GRAY AREA           │  ❌ UNACCEPTABLE     │
│  (Always OK)            │  (Depends on context)    │  (Never OK)          │
├─────────────────────────┼──────────────────────────┼──────────────────────┤
│ • Spell check           │ • Rewriting your own     │ • Generating entire  │
│ • Grammar correction    │   paragraph for better   │   paragraphs you     │
│ • Looking up word       │   style                  │   claim as your own  │
│   usage                 │ • Using AI to suggest    │ • Having AI write    │
│ • Checking punctuation  │   alternative sentence   │   your analysis or   │
│ • Using a dictionary/   │   structures             │   conclusions        │
│   thesaurus             │ • Getting AI feedback    │ • Submitting AI-     │
│ • Checking formatting   │   on your draft          │   generated text     │
│                         │ • Translating your own   │   without disclosure │
│                         │   ideas from L1 to       │ • Using AI to        │
│                         │   English                │   fabricate data or  │
│                         │                          │   results            │
└─────────────────────────┴──────────────────────────┴──────────────────────┘
```

> 💡 **Key Rule:** If you use AI in the "gray area," you must **understand** what the AI produced, **verify** its accuracy, and **disclose** the use according to your instructor's policy.

### Using AI for Persian → English Translation of Technical Ideas

Many EE students think in Persian (or Arabic/French) and then translate to English. AI can help with this process — but with important conditions:

**Acceptable workflow:**
1. Write your technical idea in Persian (or your native language)
2. Use AI to translate to English
3. **Review the translation carefully** — AI may mistranslate technical terms
4. **Verify technical accuracy** — ensure the English version says what you mean
5. **Edit and personalize** — make it sound like your writing
6. **Disclose** that you used AI-assisted translation (if required by your institution)

**Example:**

> **Your idea (in Persian):** مبدل باک طراحی‌شده در بار کامل بازده ۹۴ درصد دارد اما در بارهای سبک بازده کاهش می‌یابد زیرا تلفات سوئیچینگ غالب می‌شوند
>
> **AI translation:** "The designed buck converter has 94% efficiency at full load, but efficiency decreases at light loads because switching losses become dominant."
>
> **Your improved version:** "The designed buck converter achieves 94% efficiency at full load. However, at light loads (below 20% of rated power), efficiency drops to 78% as switching losses become the dominant loss mechanism."

> ⚠️ **Warning:** AI translation may use incorrect technical terminology. Always verify that technical terms match standard IEEE/IEC usage.

### Vocabulary Box: AI-Related Terms

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Large Language Model (LLM)** | An AI system trained on large amounts of text that can generate and modify text | ChatGPT is a large language model developed by OpenAI. |
| **AI-generated text** | Text that was produced by an artificial intelligence system, not written by a human | Submitting AI-generated text as your own work is a form of academic misconduct. |
| **Prompt** | The instruction or question you give to an AI tool | A well-written prompt produces more useful AI output. |
| **Disclosure** | A statement declaring how and where AI was used in your work | Many journals now require an AI use disclosure statement. |
| **AI hallucination** | When an AI generates information that sounds correct but is factually wrong | AI hallucinations are dangerous in engineering because incorrect specifications can cause design failures. |
| **Human-in-the-loop** | A process where a human reviews and verifies AI output before use | Engineering applications require a human-in-the-loop to ensure safety and accuracy. |

---

### Exercise: Compare AI Revision with Student Revision

**Instructions:** Below is a weak paragraph written by a student. First, revise it yourself using the techniques from Sections 5.1–5.6. Then, compare your revision with an AI revision (provided). Discuss which is better and why.

**Weak Paragraph (original student draft):**
> "The PLL is really important in communication systems. It basically locks onto the frequency and it works pretty well most of the time. We used a PLL in our project and it was good. The loop bandwidth affects how fast it can track and there are different types like analog and digital ones. PLLs are used in lots of things like radios and clock recovery and stuff."

**AI Revision (generated by ChatGPT):**
> "The phase-locked loop (PLL) is a fundamental component in communication systems, used for frequency synthesis, clock recovery, and carrier synchronization. The PLL operates by locking its output frequency and phase to a reference signal through a feedback mechanism. The loop bandwidth determines the tracking speed and noise rejection capability of the system. Both analog and digital PLL architectures exist, each suited to different applications depending on performance requirements."

**Questions for discussion:**
1. What did the AI improve? (List at least 4 improvements)
2. What is MISSING from the AI revision? (Hint: specific data, citation, personal contribution)
3. Now write YOUR OWN revision of the weak paragraph, including:
   - Specific technical data (frequencies, performance metrics)
   - A citation to a source
   - Connection to your own project work
   - At least 100 words

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Identified AI improvements correctly | /2 |
| Identified missing elements in AI version | /2 |
| Student's own revision: technical precision | /2 |
| Student's own revision: includes specific data | /2 |
| Student's own revision: scientific style | /2 |
| **Total** | **/10** |

---


# WEEK 6: Paraphrasing, Summarizing, and Academic Integrity

## Learning Objectives

By the end of this week, students will be able to:

1. Paraphrase technical sentences using multiple techniques while preserving meaning
2. Summarize a research paper section concisely and accurately
3. Distinguish between appropriate paraphrasing and plagiarism
4. Apply IEEE citation format correctly in text and reference lists
5. Demonstrate understanding of academic integrity principles

---

## 6.1 Paraphrasing: Techniques and Practice

### What Is Paraphrasing?

Paraphrasing is restating someone else's ideas **in your own words and sentence structure** while maintaining the original meaning. It is NOT simply replacing a few words with synonyms.

### Paraphrasing Techniques

| Technique | Description | Example |
|-----------|-------------|---------|
| **Change sentence structure** | Convert active to passive (or vice versa), change clause order | Original: "Researchers developed a new algorithm." → "A new algorithm was developed." |
| **Use synonyms** | Replace key words with equivalent terms | "reduce power consumption" → "decrease energy usage" |
| **Change word forms** | Convert nouns to verbs, adjectives to adverbs, etc. | "The amplification of the signal" → "The signal is amplified" |
| **Combine/split sentences** | Merge two short sentences or break a long one | Split a compound sentence into two simple ones |
| **Change the order of information** | Present the same ideas in a different sequence | Move the result before the method |

### Paraphrasing Examples from Electrical Engineering

**Original 1 (Signal Processing):**
> "The discrete wavelet transform provides multi-resolution analysis capability, which makes it particularly suitable for analyzing non-stationary signals such as power system transients." [5]

**Good Paraphrase:**
> According to [5], non-stationary signals, including transients in power systems, can be effectively analyzed using the discrete wavelet transform due to its ability to perform analysis at multiple resolutions.

**Bad Paraphrase (too close to original):**
> ❌ The discrete wavelet transform gives multi-resolution analysis ability, which makes it especially appropriate for analyzing non-stationary signals like power system transients [5].

*(Only individual words were changed — the structure is identical. This is plagiarism.)*

---

**Original 2 (Power Systems):**
> "The integration of distributed generation sources into existing power networks necessitates significant modifications to protection coordination schemes." [12]

**Good Paraphrase:**
> Protection coordination systems in conventional power networks require substantial redesign when distributed generation is incorporated [12].

**Bad Paraphrase:**
> ❌ The incorporation of distributed generation sources into current power networks requires significant changes to protection coordination schemes [12].

*(Structure unchanged, only synonyms swapped — still plagiarism.)*

---

**Original 3 (Telecommunications):**
> "Multiple-input multiple-output (MIMO) systems exploit spatial diversity to improve both the reliability and capacity of wireless communication links." [8]

**Good Paraphrase:**
> By leveraging multiple antennas at the transmitter and receiver, MIMO technology enhances wireless link capacity and reduces error rates through spatial diversity gains [8].

---

**Original 4 (Control Systems):**
> "Model predictive control uses an explicit model of the plant to predict future system behavior and optimize control actions over a finite horizon." [15]

**Good Paraphrase:**
> In model predictive control, a mathematical representation of the system is employed to forecast its future states, enabling the optimization of control inputs within a defined time window [15].

---

## 6.2 Summarizing

### What Is Summarizing?

Summarizing means **condensing** a longer text (paper, section, chapter) to its **essential points** only. A summary is significantly shorter than the original (typically 10–25% of original length).

### Steps for Effective Summarizing

1. **Read** the entire text carefully
2. **Identify** the main argument/finding
3. **Note** key supporting points (method, main results)
4. **Write** in your own words without looking at the original
5. **Check** that you have captured the essential meaning
6. **Cite** the original source

### Summary Template

```
[Author/Study] investigated [topic/problem]. Using [method], they found that
[main finding]. The results suggest that [implication/significance]. [Citation]
```

### Example: Summarizing a Paper Section

**Original Paragraph (150 words):**
> "This paper presents a novel maximum power point tracking (MPPT) algorithm for photovoltaic systems based on an adaptive neural network. The proposed method addresses the limitations of conventional perturb and observe (P&O) algorithms, which suffer from oscillations around the maximum power point and poor performance under rapidly changing irradiance conditions. The adaptive neural network is trained using historical irradiance and temperature data, allowing it to predict the optimal operating voltage without the trial-and-error approach inherent in P&O methods. Experimental results obtained from a 5 kW grid-connected PV system demonstrate that the proposed algorithm achieves 99.2% tracking efficiency under steady-state conditions and responds to irradiance changes within 50 ms, representing a 60% improvement in dynamic response compared to conventional P&O."

**Summary (55 words):**
> The authors propose an adaptive neural network-based MPPT algorithm for PV systems that overcomes the oscillation and slow dynamic response problems of conventional P&O methods. Testing on a 5 kW system showed 99.2% tracking efficiency and 60% faster response to irradiance changes compared to P&O [reference].

---

## 6.3 Quoting

### When to Use Direct Quotes

Use direct quotes **sparingly** in technical writing. Quote directly only when:

- The exact wording is important (definitions, standards)
- The original phrasing is particularly effective
- You are analyzing the language itself

### How to Quote

| Format | Example |
|--------|---------|
| Short quote (< 40 words) | According to [3], "the Shannon capacity defines the theoretical maximum data rate for a channel with a given bandwidth and SNR." |
| Longer quote | Indent as a block quote and cite at the end |
| Quote with modification | "The proposed algorithm [for MPPT] achieves higher efficiency" [5]. |
| Quote with omission | "OFDM systems... are robust against multipath fading" [7]. |

> 💡 **Tip:** In engineering writing, paraphrasing is almost always preferred over direct quoting. Most IEEE papers contain very few (if any) direct quotes.

---

## 6.4 IEEE Citation Format

### In-Text Citations

IEEE uses **numbered references** in square brackets:

| Rule | Example |
|------|---------|
| Single reference | The method in [5] achieves 95% accuracy. |
| Multiple references | Several studies [3], [7], [12] confirm this result. |
| Range of references | Prior work [1]–[4] investigated this problem. |
| Reference as noun | In [8], the authors proposed a novel approach. |
| Reference at end of sentence | This has been demonstrated experimentally [6]. |

### Reference List Format (IEEE)

```
JOURNAL ARTICLE:
[1] A. B. Author and C. D. Author, "Title of the article," Journal Name,
    vol. X, no. Y, pp. 000–000, Month Year.

CONFERENCE PAPER:
[2] A. B. Author, "Title of the paper," in Proc. Conference Name,
    City, Country, Year, pp. 000–000.

BOOK:
[3] A. B. Author, Title of the Book, Xth ed. City, Country:
    Publisher, Year.

ONLINE/WEBSITE:
[4] A. B. Author, "Title of page," Website Name. [Online]. Available:
    URL. [Accessed: Month Day, Year].

STANDARD:
[5] Title of Standard, Standard Number, Organization, Year.

THESIS:
[6] A. B. Author, "Title of thesis," M.S. thesis, Dept., Univ.,
    City, Country, Year.
```

### Complete Reference Examples

```
[1] S. Haykin and M. Moher, "An introduction to analog and digital
    communications," IEEE Trans. Commun., vol. 55, no. 3, pp. 431–445,
    Mar. 2007.

[2] K. Zhang and L. Wang, "Deep learning for power system fault
    detection," in Proc. IEEE Power & Energy Soc. General Meeting,
    Portland, OR, USA, 2023, pp. 1–6.

[3] B. Razavi, Design of Analog CMOS Integrated Circuits, 2nd ed.
    New York, NY, USA: McGraw-Hill, 2017.

[4] IEEE Standard for Interconnection and Interoperability of
    Distributed Energy Resources, IEEE Std 1547-2018, 2018.
```

---

## 6.5 Academic Integrity and Plagiarism

### What Counts as Plagiarism?

| Type | Description | Example |
|------|-------------|---------|
| **Direct copying** | Using exact words without quotation marks | Copying a paragraph from a paper without quotes |
| **Inadequate paraphrase** | Changing only a few words from the original | Swapping synonyms but keeping structure |
| **Missing citation** | Using someone's ideas without giving credit | Presenting another's findings as your own |
| **Self-plagiarism** | Reusing your own previously submitted work | Submitting the same lab report for two courses |
| **Fabrication** | Inventing data or results | Reporting measurements that were never taken |
| **Collusion** | Presenting collaborative work as individual | Copying from a classmate's assignment |

### How to Avoid Plagiarism

1. **Always cite** when using others' ideas, data, or methods
2. **Paraphrase properly** — change both words AND structure
3. **Use quotation marks** for any exact phrases from sources
4. **Keep notes** of all sources during research
5. **Manage your time** — rushing leads to poor paraphrasing
6. **When in doubt, cite** — over-citation is better than plagiarism

### Bad Paraphrase vs. Good Paraphrase

**Original:**
> "The finite element method discretizes the problem domain into smaller elements, enabling the numerical solution of complex electromagnetic field distributions that cannot be solved analytically." [9]

**❌ Bad Paraphrase (plagiarism):**
> The finite element method divides the problem domain into smaller parts, allowing the numerical solution of difficult electromagnetic field distributions that cannot be solved analytically [9].

**Why it's bad:** Only "discretizes" → "divides" and "complex" → "difficult" changed. The sentence structure is identical.

**✅ Good Paraphrase:**
> Complex electromagnetic problems that lack analytical solutions can be addressed numerically by partitioning the computational domain into discrete elements — the fundamental principle underlying the finite element method [9].

**Why it's good:** Different structure (result before method), different word forms, reorganized information, same meaning.

---

## 6.6 Vocabulary Box

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Paraphrase** | Restating a text in different words and structure while preserving meaning | A good paraphrase demonstrates understanding of the source material. |
| **Plagiarism** | Presenting another's work or ideas as one's own without proper attribution | Submitting copied text without citation constitutes plagiarism. |
| **Citation** | A reference to a source that supports a claim or provides credit | IEEE papers use numbered citations in square brackets. |
| **In-text citation** | A brief reference within the body of the text | The study [3] confirmed the theoretical predictions. |
| **Reference list** | A complete list of all cited sources at the end of a paper | The reference list should include all works cited in the text. |
| **Self-plagiarism** | Reusing one's own previously published work without acknowledgment | Submitting the same report to multiple courses is self-plagiarism. |
| **Attribution** | Giving credit to the original source of information | Proper attribution is essential in academic writing. |
| **Intellectual property** | Creations of the mind, including written works and inventions | Research papers are protected as intellectual property. |

---

## 6.7 Exercises and Activities

### Activity 1: Paraphrase 5 Technical Sentences

Paraphrase each sentence below. You must change BOTH the structure AND the vocabulary.

1. "Convolutional neural networks have demonstrated remarkable performance in image classification tasks, achieving accuracy levels that surpass human performance on certain benchmarks." [2]

2. "The rapid deployment of electric vehicles will place unprecedented demand on the electrical distribution network, particularly during evening peak hours." [6]

3. "Gallium nitride (GaN) transistors offer superior switching performance compared to silicon-based devices, enabling higher operating frequencies and reduced power losses in converter applications." [11]

4. "The Internet of Things (IoT) relies on low-power wide-area network (LPWAN) technologies such as LoRa and NB-IoT to provide connectivity for billions of distributed sensor nodes." [4]

5. "Adaptive beamforming algorithms dynamically adjust antenna array weights to maximize signal reception from the desired direction while suppressing interference from other sources." [9]

---

### Activity 2: Summarize a Paper Section

**Instructions:** Read the following extract (200 words) and summarize it in approximately 100 words.

> "This study investigates the application of reinforcement learning (RL) to optimal energy management in microgrids with integrated renewable energy sources and battery storage systems. The microgrid under consideration comprises a 100 kW solar photovoltaic array, a 50 kW wind turbine, a 200 kWh lithium-ion battery storage system, and controllable loads. The proposed deep Q-network (DQN) agent learns to make real-time decisions regarding battery charging and discharging, load scheduling, and grid interaction without requiring an explicit model of the system dynamics. Training was conducted using one year of historical weather and load data from a university campus in southern Algeria. The results demonstrate that the RL-based energy management system reduces electricity costs by 23% and curtailment of renewable energy by 45% compared to a rule-based baseline strategy. Furthermore, the agent successfully maintains battery state of charge within safe operating limits (20%–90%) throughout the simulation period. These findings suggest that model-free RL approaches offer a viable alternative to traditional optimization methods for microgrid energy management, particularly in environments with high uncertainty in renewable generation and load patterns."

---

## 6.8 AI-Assisted Paraphrasing — Ethical Boundaries

### How AI Paraphrasing Tools Work

AI paraphrasing tools (QuillBot, ChatGPT with "rephrase this," Claude, etc.) use large language models to rewrite text. They analyze the input sentence structure and vocabulary, then generate alternative versions that preserve the general meaning while changing the surface form.

**How they process text:**
1. The AI reads your input text
2. It identifies the key information and relationships
3. It generates new sentences that convey similar meaning
4. It uses different vocabulary, sentence structures, and word order

**Common AI paraphrasing tools in academic contexts:**

| Tool | How Students Use It | Typical Output |
|------|-------------------|----------------|
| **QuillBot** | Paste text → select mode (Standard, Fluency, Creative) → get rewritten version | Multiple paraphrase options with varying levels of change |
| **ChatGPT / Claude** | "Rephrase this paragraph:" → paste text | Full rewrite with changed structure and vocabulary |
| **Grammarly AI** | Highlight text → click "Rephrase" | Sentence-level rewrites for clarity |
| **Wordtune** | Select sentence → see alternatives | Multiple alternative phrasings |

### When AI Paraphrasing Is Acceptable vs. When It's Plagiarism

The ethical question is NOT "Did you use a tool?" — it is **"Do you understand what you're writing?"**

```
┌────────────────────────────────────────────────────────────────────┐
│                    THE KEY QUESTION:                                │
│                                                                    │
│    "Do you UNDERSTAND what you are writing?"                       │
│                                                                    │
│    If yes → you can use tools to improve expression               │
│    If no  → using AI to hide your lack of understanding           │
│             is academic dishonesty                                 │
└────────────────────────────────────────────────────────────────────┘
```

### Acceptable vs. Unacceptable AI Paraphrasing

| Scenario | Acceptable? | Why? |
|----------|-------------|------|
| You write a paragraph about your PLL design results. The English is awkward. You use AI to improve the grammar and flow. | ✅ Yes | You wrote the content; AI only improved the language |
| You find a paragraph in a paper about OFDM. You paste it into QuillBot to rephrase it. You put the result in your report without citation. | ❌ No | This is plagiarism — you are hiding the source |
| You find a paragraph in a paper about OFDM. You paste it into QuillBot to rephrase it. You add a citation [5]. | ⚠️ Problematic | You have a citation, but you haven't demonstrated understanding — the AI did the paraphrasing, not you |
| You read a paper about OFDM, understand the key ideas, close the paper, write the ideas in your own words, then use AI to check your grammar. | ✅ Yes | You paraphrased yourself; AI only fixed language errors |
| You don't understand a complex section about adaptive beamforming. You ask AI to "explain it simply" then copy that explanation into your report. | ❌ No | The explanation is not yours — it's AI-generated content presented as your understanding |

### How AI Paraphrasing Differs from Genuine Understanding

**AI paraphrasing produces surface-level changes:**
- Changes word order
- Swaps synonyms
- Restructures sentences
- Preserves meaning of the input text

**Genuine understanding produces deep-level changes:**
- Connects the idea to other knowledge you have
- Allows you to explain WHY something works, not just WHAT it does
- Enables you to give your own examples
- Lets you identify implications the original author didn't mention
- Allows you to explain the concept to someone else without notes

**Example — Original text:**
> "The Kalman filter provides optimal state estimation for linear systems with Gaussian noise by recursively combining predictions from a dynamic model with noisy measurements." [10]

**AI paraphrase (surface change only):**
> "For linear systems affected by Gaussian noise, the Kalman filter achieves optimal estimation of system states through a recursive process that merges dynamic model predictions with noisy measurement data [10]."

**Human paraphrase (showing genuine understanding):**
> "In control systems with linear dynamics and normally distributed noise, the Kalman filter estimates unmeasured states — such as the position of a drone from noisy GPS readings — by balancing trust between the mathematical model's predictions and the actual sensor measurements. Each time new data arrives, the filter updates its estimate, weighting the model more heavily when sensors are unreliable and trusting measurements more when the model is uncertain [10]."

> 💡 **Notice:** The human paraphrase adds an example (drone GPS), explains the mechanism (balancing trust), and demonstrates understanding of when each component matters. The AI paraphrase only rearranges words.

---

### Exercise: Compare Human Paraphrase vs. AI Paraphrase

**Instructions:** Read the original EE text below. You are given an AI-generated paraphrase and must write your own human paraphrase. Then answer the comparison questions.

**Original text (from an IEEE paper on power electronics):**
> "Silicon carbide (SiC) MOSFETs enable significantly higher switching frequencies compared to silicon IGBTs, which allows for the reduction of passive component sizes in power converter designs. However, the faster switching transients of SiC devices generate increased electromagnetic interference (EMI) that must be mitigated through careful PCB layout and appropriate filtering techniques." [14]

**AI Paraphrase (QuillBot output):**
> "Compared to silicon IGBTs, silicon carbide (SiC) MOSFETs allow for considerably higher switching frequencies, enabling smaller passive components in power converters. Nevertheless, the rapid switching transients of SiC devices produce more electromagnetic interference (EMI), requiring mitigation through proper PCB design and suitable filtering methods [14]."

**Your task:**
1. Write your OWN paraphrase (without using AI). Your paraphrase should:
   - Change both vocabulary AND structure significantly
   - Show that you understand the cause-effect relationship
   - Add a brief explanation of WHY higher frequency allows smaller passives
   - Include the citation [14]
   - Be 40–60 words

2. Answer these questions:
   - (a) How is the AI paraphrase different from the original? (List specific changes)
   - (b) What is SIMILAR between the AI paraphrase and the original? (What didn't change?)
   - (c) Why might a plagiarism checker still flag the AI paraphrase?
   - (d) What does your human paraphrase include that the AI version does not?

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Human paraphrase: significant structural change | /2 |
| Human paraphrase: demonstrates understanding (explains WHY) | /3 |
| Human paraphrase: correct citation included | /1 |
| Analysis questions answered correctly | /4 |
| **Total** | **/10** |

---

## 6.9 Homework

**Assignment:** Find a published IEEE paper in your area of interest within Electrical Engineering.

1. **Paraphrase** the abstract of the paper (write it entirely in your own words — DO NOT copy any phrases of 3+ consecutive words)
2. **Write the full IEEE reference** for the paper
3. **Highlight** at least 3 techniques you used to paraphrase (e.g., changed structure, used synonyms, changed word forms)

**Submission format:**
- Original abstract (copied exactly)
- Your paraphrased version
- IEEE reference
- List of paraphrasing techniques used with specific examples

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Meaning accurately preserved | /3 |
| Sufficient structural change from original | /3 |
| Vocabulary appropriately varied | /2 |
| Correct IEEE reference format | /1 |
| Techniques identified and explained | /1 |
| **Total** | **/10** |

---

## 6.10 Tips and Common Mistakes

### ✅ Tips for Effective Paraphrasing

1. **Read the original multiple times** until you fully understand it
2. **Put the original away** and write from memory
3. **Compare** your version to the original — if more than 3 consecutive words match, revise
4. **Maintain the technical accuracy** — do not distort the meaning
5. **Always include a citation** — paraphrasing is not a way to avoid referencing

### ❌ Common Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Word-for-word synonym swap | Still plagiarism | Change sentence structure too |
| Changing meaning while paraphrasing | Misrepresentation | Verify technical accuracy |
| Forgetting the citation | Plagiarism even if paraphrased well | Always cite the source |
| Paraphrasing common knowledge | Unnecessary — no citation needed | "Ohm's law states V=IR" needs no citation |
| Over-quoting instead of paraphrasing | Shows lack of understanding | Limit quotes; paraphrase most content |

---


# WEEK 7: Writing Abstracts, Introductions, and Conclusions

## Learning Objectives

By the end of this week, students will be able to:

1. Write a structured abstract (150–250 words) following the background-problem-method-results-conclusion pattern
2. Construct an effective introduction using the general-to-specific funnel structure
3. Write a conclusion that summarizes findings, states contributions, acknowledges limitations, and suggests future work
4. Use standard academic phrases appropriate for each section
5. Select appropriate keywords and write author affiliation information

---

## 7.1 Abstract Structure

### The Five Components of an Abstract

An abstract is a **single paragraph** (150–250 words) that contains:

| Component | Purpose | Approximate Length |
|-----------|---------|-------------------|
| **Background** | Establish context and importance | 1–2 sentences |
| **Problem/Gap** | State what is missing or unsolved | 1 sentence |
| **Method** | Describe what was done | 1–2 sentences |
| **Results** | Present key findings with data | 1–2 sentences |
| **Conclusion** | State the significance/implication | 1 sentence |

### Abstract Language Patterns and Useful Phrases

**Background:**
- "In recent years, [topic] has attracted significant research interest due to..."
- "[Topic] plays a critical role in..."
- "The increasing demand for [X] has motivated research in..."
- "[X] is widely used in [application] owing to its [properties]."

**Problem/Gap:**
- "However, existing methods suffer from..."
- "Despite these advances, [problem] remains a challenge."
- "Current approaches fail to address..."
- "Limited attention has been paid to..."

**Method:**
- "This paper presents / proposes / introduces..."
- "In this work, we develop a [method] for [purpose]."
- "The proposed approach employs / utilizes / leverages..."
- "A [method]-based technique is applied to..."

**Results:**
- "Experimental results demonstrate that..."
- "The proposed method achieves [metric] of [value]."
- "Simulation results show a [X]% improvement over..."
- "Compared to [baseline], the proposed approach reduces [metric] by [value]."

**Conclusion:**
- "These results confirm that..."
- "The proposed method offers a viable solution for..."
- "This work contributes to [field] by providing..."
- "The findings suggest that [X] can be effectively applied to [Y]."

---

### Model Abstract: "Deep Learning for Power System Fault Detection"

> **[Background]** Rapid and accurate fault detection is essential for maintaining the reliability and safety of modern power systems. **[Problem]** Conventional protection relays rely on threshold-based algorithms that struggle to differentiate between faults and non-fault transient events, particularly in networks with high penetration of distributed generation. **[Method]** This paper proposes a deep convolutional neural network (CNN) architecture for real-time fault detection and classification in transmission lines. The model is trained on a dataset of 50,000 simulated fault scenarios generated using PSCAD/EMTDC, encompassing ten fault types across varying fault locations, resistances, and inception angles. **[Results]** The proposed CNN achieves an overall classification accuracy of 99.4% with a detection time of 5 ms (quarter cycle at 50 Hz), outperforming support vector machine and random forest classifiers by 3.2% and 2.8%, respectively. The model maintains accuracy above 98% even under noisy conditions (SNR = 20 dB). **[Conclusion]** These results demonstrate that deep learning-based fault detection offers a robust and computationally efficient alternative to conventional methods, with potential for deployment in digital substation environments.

**Word count:** 183 words

### Annotated Breakdown:

| Component | Text | Words |
|-----------|------|-------|
| Background | "Rapid and accurate fault detection...modern power systems." | 17 |
| Problem | "Conventional protection relays...distributed generation." | 30 |
| Method | "This paper proposes...inception angles." | 52 |
| Results | "The proposed CNN achieves...SNR = 20 dB)." | 60 |
| Conclusion | "These results demonstrate...digital substation environments." | 24 |

---

## 7.2 Introduction Structure

### The Funnel Model

An introduction moves from **general** to **specific**:

```
╔══════════════════════════════════════════════════════╗
║        GENERAL CONTEXT (broad field)                ║
╠════════════════════════════════════════════════╗     ║
║      SPECIFIC TOPIC (narrowed focus)          ║     ║
╠══════════════════════════════════╗             ║     ║
║    GAP/PROBLEM (what's missing)  ║             ║     ║
╠════════════════════════╗         ║             ║     ║
║  OBJECTIVE (this paper)║         ║             ║     ║
╠══════════════╗         ║         ║             ║     ║
║ PAPER OUTLINE║         ║         ║             ║     ║
╚══════════════╝         ║         ║             ║     ║
```

### Introduction Components

| Move | Purpose | Typical Length |
|------|---------|---------------|
| **Move 1: Establish territory** | Show the field is important and active | 2–4 sentences |
| **Move 2: Establish niche** | Identify the gap or problem | 2–3 sentences |
| **Move 3: Occupy the niche** | State your objective and contribution | 2–3 sentences |
| **Move 4: Paper organization** | Outline the paper structure | 1–2 sentences (optional) |

### Introduction Useful Phrases

**Move 1 — Establishing Territory (General Context):**
- "In recent decades, [topic] has emerged as a key technology for..."
- "[Field] has undergone significant transformation due to..."
- "The growing demand for [X] has driven extensive research in..."
- "Significant advances have been made in [topic] [1]–[5]."
- "[Technology] is widely employed in [applications] owing to..."

**Move 2 — Establishing the Niche (Gap/Problem):**
- "However, few studies have addressed..."
- "Despite significant progress, [challenge] remains unresolved."
- "Existing methods are limited by..."
- "A key limitation of current approaches is..."
- "To date, no study has investigated..."
- "The aforementioned methods fail to account for..."

**Move 3 — Occupying the Niche (Objective):**
- "This paper proposes / presents / introduces..."
- "The main contribution of this work is..."
- "In this paper, we develop a novel [method] that..."
- "The objective of this study is to..."
- "To address this gap, we propose..."
- "The key contributions of this paper are threefold: (1)... (2)... (3)..."

**Move 4 — Paper Organization:**
- "The remainder of this paper is organized as follows."
- "Section II presents the system model. Section III describes the proposed method. Section IV presents experimental results, and Section V concludes the paper."

---

### Model Introduction Paragraph

> **[Move 1]** The rapid proliferation of Internet of Things (IoT) devices has created an unprecedented demand for energy-efficient wireless communication protocols [1]–[3]. Current projections estimate that over 75 billion IoT devices will be connected by 2030, the majority of which will be battery-powered sensors operating in resource-constrained environments [4]. Low-Power Wide-Area Network (LPWAN) technologies such as LoRa, Sigfox, and NB-IoT have been developed to serve this growing market by providing long-range connectivity at minimal energy cost [5]. **[Move 2]** However, existing LPWAN protocols employ fixed transmission parameters regardless of channel conditions, leading to unnecessary energy expenditure when the channel quality is favorable and packet loss when conditions deteriorate [6], [7]. Although adaptive data rate (ADR) mechanisms exist in protocols such as LoRaWAN, they rely on simple heuristic rules that respond slowly to changing environments and do not optimize for energy efficiency explicitly [8]. **[Move 3]** This paper proposes a reinforcement learning-based adaptive transmission strategy for LoRa end devices that jointly optimizes spreading factor, transmission power, and coding rate to minimize energy consumption while maintaining a target packet delivery ratio above 99%. The main contributions of this work are: (1) a deep Q-network formulation for joint parameter optimization, (2) a lightweight inference model suitable for deployment on microcontrollers, and (3) extensive experimental validation on a 50-node testbed. **[Move 4]** The remainder of this paper is organized as follows. Section II reviews related work. Section III describes the system model. The proposed method is detailed in Section IV. Section V presents results, and Section VI concludes the paper.

---

## 7.3 Conclusion Structure

### Components of a Conclusion

| Component | Purpose | Example Starter |
|-----------|---------|----------------|
| **Summary** | Briefly restate what was done and found | "This paper presented..." |
| **Main contribution** | Highlight the significance | "The key contribution is..." |
| **Limitations** | Acknowledge constraints honestly | "A limitation of this study is..." |
| **Future work** | Suggest next steps | "Future work will investigate..." |

### Conclusion Useful Phrases

**Summary:**
- "This paper has presented a [method] for [purpose]."
- "In this work, a novel [approach] was developed and validated."
- "The proposed system was shown to achieve [result]."

**Main Contribution:**
- "The primary contribution of this work is..."
- "These findings demonstrate that..."
- "The results confirm the effectiveness of..."
- "This work advances the state of the art by..."

**Limitations:**
- "A limitation of the current study is..."
- "The proposed method assumes [condition], which may not hold in..."
- "The experimental validation was limited to [scope]."
- "Further investigation is needed to confirm..."

**Future Work:**
- "Future work will extend this approach to..."
- "In future research, we plan to investigate..."
- "Potential directions for further study include..."
- "The proposed framework can be extended by incorporating..."

---

### Model Conclusion Paragraph

> This paper has presented a deep CNN-based approach for real-time fault detection and classification in transmission lines. The proposed architecture achieves 99.4% classification accuracy with a detection time of 5 ms, representing a significant improvement over conventional machine learning classifiers. The key contribution of this work is demonstrating that CNN-based protection can maintain high accuracy under noisy conditions and varying fault parameters without requiring manual feature extraction. A limitation of the current study is that the model was trained and validated exclusively on simulated data; performance on real-world fault recordings may differ. Furthermore, the computational requirements of the CNN may challenge deployment on existing relay hardware. Future work will focus on transfer learning to adapt the model to real field data and on model compression techniques to enable deployment on embedded protection devices.

---

## 7.4 Author Affiliation and Keywords

### Author Information Conventions

```
Author Name¹*, Co-Author Name²

¹ Department of Electrical Engineering, University Name, City, Country
² Laboratory of [X], Institution Name, City, Country
* Corresponding author: email@university.edu
```

### Keywords Selection

**Guidelines:**
- Choose 4–6 keywords
- Include the main topic, method, application domain
- Use established terms from the field (check IEEE Thesaurus)
- Avoid overly general terms ("engineering," "system")
- Avoid overly specific terms that no one would search for

**Example:**
> **Keywords:** fault detection, convolutional neural network, power system protection, transmission lines, deep learning, pattern recognition

---

## 7.5 Vocabulary Box

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Abstract** | A concise summary of a research paper (150–250 words) | The abstract should allow readers to determine the paper's relevance without reading the full text. |
| **Introduction** | The opening section that establishes context, identifies the gap, and states objectives | A strong introduction guides the reader from general context to the specific research question. |
| **Conclusion** | The final section summarizing findings and suggesting future directions | The conclusion should not introduce new information or data. |
| **Research gap** | An area that has not been adequately addressed by existing studies | Identifying a clear research gap justifies the need for the study. |
| **Contribution** | The new knowledge or method that the paper adds to the field | The main contribution should be clearly stated in both the abstract and conclusion. |
| **Affiliation** | The institution or organization to which an author belongs | Author affiliations appear below the author names on the first page. |
| **Keywords** | Terms that represent the main topics of a paper for indexing | Well-chosen keywords improve the discoverability of a paper in databases. |

---

## 7.6 Exercises and Activities

### Exercise 1: Analyze an Abstract

Read the following abstract and identify the five components (Background, Problem, Method, Results, Conclusion):

> "Smart grids incorporate advanced metering infrastructure and two-way communication to enable real-time monitoring and control of power distribution. However, the increased connectivity introduces cybersecurity vulnerabilities that can be exploited to disrupt grid operations. This paper proposes a federated learning-based intrusion detection system (IDS) for smart grid networks that preserves data privacy while enabling collaborative threat detection across multiple utility domains. The system was evaluated using the NSL-KDD and CIC-IDS-2017 datasets with simulated smart grid traffic patterns. Results show that the federated approach achieves 97.8% detection accuracy while reducing false alarm rates by 35% compared to centralized approaches. The proposed framework offers a scalable and privacy-preserving solution for enhancing cybersecurity in smart grid infrastructure."

---

### Activity: Write an Abstract

**Instructions:** Write an abstract (150–250 words) for a hypothetical paper on ONE of the following topics:

1. "A Fuzzy Logic Controller for Battery Management in Electric Vehicles"
2. "Performance Analysis of 5G mmWave Communication in Urban Environments"
3. "Design of a Grid-Connected Inverter for Residential Solar PV Systems"
4. "Machine Learning-Based Predictive Maintenance for Wind Turbines"

**Your abstract must include:**
- Background (1–2 sentences)
- Problem/Gap (1 sentence)
- Method (1–2 sentences)
- Results (1–2 sentences with specific numbers)
- Conclusion (1 sentence)

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| All 5 components present | /3 |
| Appropriate length (150–250 words) | /1 |
| Specific results with numbers | /2 |
| Academic language and style | /2 |
| Logical flow between components | /2 |
| **Total** | **/10** |

---

## 7.7 Homework

**Assignment:** Choose an EE topic of interest and write an introduction (approximately 300 words) that includes:

1. **Move 1:** General context establishing the importance of the field (2–3 sentences with at least 2 citations)
2. **Move 2:** Identification of a specific gap or problem (2–3 sentences)
3. **Move 3:** Statement of your paper's objective and contributions (2–3 sentences)
4. **Move 4:** Brief paper organization (1–2 sentences)

**Requirements:**
- Use at least 3 phrases from the "Useful Phrases" sections
- Include at least 4 references (you may use placeholder numbers [1]–[4])
- Follow formal scientific style
- Underline your cohesion devices

**Due:** Next class session

---

## 7.8 Tips and Common Mistakes

### ✅ Tips for Writing Abstracts

1. **Write the abstract last** — after completing the full paper
2. **Do not include references** in the abstract (some journals allow it, but generally avoid)
3. **Do not use abbreviations** without defining them (except very common ones like IEEE)
4. **Include at least one quantitative result** — numbers make abstracts convincing
5. **Keep it to one paragraph** — no line breaks within an abstract

### ✅ Tips for Introductions

1. **Start broad, end specific** — follow the funnel model
2. **Cite extensively** — introductions typically have the highest citation density
3. **Make the gap explicit** — use words like "however," "despite," "limited"
4. **State contributions clearly** — use numbered lists for multiple contributions
5. **Do not include results** — the introduction states what you will do, not what you found

### ❌ Common Mistakes

| Section | Mistake | Fix |
|---------|---------|-----|
| Abstract | Too long or too short | Target 150–250 words exactly |
| Abstract | Missing results/numbers | Always include quantitative findings |
| Abstract | "In this paper, we will..." (future tense) | Use present or past tense: "This paper presents..." |
| Introduction | Starting too specific | Begin with the broad field, then narrow |
| Introduction | No clear gap statement | Explicitly state what is missing/unsolved |
| Conclusion | Introducing new data | Conclusions only summarize and reflect |
| Conclusion | Merely repeating the abstract | Add limitations and future work |
| Conclusion | Being overly modest | State your contribution confidently |

---


## 7.9 Academic Integrity in the Age of AI

### Updated Definition of Plagiarism

Traditional plagiarism means presenting someone else's work as your own. In the AI era, this definition has expanded:

```
┌────────────────────────────────────────────────────────────────────┐
│              UPDATED PLAGIARISM DEFINITION                          │
│                                                                    │
│  Plagiarism now includes:                                          │
│  1. Copying text from a source without attribution                 │
│  2. Inadequate paraphrasing of others' work                        │
│  3. Presenting AI-generated text as your own writing               │
│     WITHOUT appropriate disclosure                                 │
│  4. Using AI to paraphrase others' work to avoid detection         │
│  5. Having AI generate analysis, conclusions, or methodology       │
│     that you present as your own intellectual contribution         │
└────────────────────────────────────────────────────────────────────┘
```

> ⚠️ **Key Point:** The issue is NOT that you used AI. The issue is that you **did not disclose** AI use, or that the work does **not represent your understanding**.

### University AI Policies: Three Types

Universities worldwide have adopted different approaches to AI. Know your institution's policy:

| Policy Type | Description | What's Allowed | Examples |
|-------------|-------------|----------------|----------|
| **Type 1: Ban** | AI tools prohibited for coursework | No AI use at all; all work must be entirely human-written | Some exams, certain assignments with explicit instructions |
| **Type 2: Permit with Disclosure** | AI allowed for specific purposes if declared | Grammar checking, translation, brainstorming — with mandatory disclosure statement | Most common policy at universities currently |
| **Type 3: Free Use** | AI use encouraged as a skill | AI may be used freely; assessment focuses on final output quality | Some graduate research, professional contexts |

> 💡 **Important:** Most universities currently use **Type 2** — they allow AI as a tool but require you to declare its use. Always check the specific policy for each course.

### What Constitutes AI Plagiarism vs. Legitimate AI Assistance

| Action | AI Plagiarism? | Why? |
|--------|---------------|------|
| Using Grammarly to fix grammar errors | ❌ No | Tool corrects your language; ideas are yours |
| Asking ChatGPT to "write a 200-word introduction about PV inverters" and submitting the output | ✅ Yes | The content is AI-generated, not your intellectual work |
| Writing your results section, then asking AI to check for grammar and clarity | ❌ No | You wrote the content; AI only polished the language |
| Asking AI to "paraphrase this paragraph from [source]" and putting it in your paper with a citation | ⚠️ Problematic | Citation is good, but the paraphrasing was not your intellectual effort |
| Using AI to brainstorm ideas for your project topic, then writing everything yourself | ❌ No | AI was used for ideation; all writing is yours |
| Asking AI to generate your methodology section | ✅ Yes | Methodology should reflect what YOU actually did |
| Using AI to translate your own ideas from Persian to English, then editing | ❌ No (with disclosure) | Ideas are yours; AI assisted with language only |
| Asking AI to write your conclusion based on results you describe to it | ✅ Yes | Conclusions should demonstrate YOUR analytical thinking |

### Disclosure Statements: How to Declare AI Use

When your institution permits AI with disclosure, you must include a statement. Here is a standard format:

**Sample AI Disclosure Statement:**

```
┌────────────────────────────────────────────────────────────────────┐
│                    AI USE DISCLOSURE                                │
│                                                                    │
│ In preparing this report, the following AI tools were used:        │
│                                                                    │
│ 1. Grammarly AI — Used for grammar and spelling correction         │
│    throughout the document.                                        │
│                                                                    │
│ 2. ChatGPT (GPT-4) — Used to check English grammar in             │
│    Sections 3 and 4, which were originally drafted in Persian      │
│    and translated by the author.                                   │
│                                                                    │
│ 3. QuillBot — Used to rephrase 3 sentences in Section 2 for       │
│    improved clarity.                                               │
│                                                                    │
│ All technical content, analysis, data interpretation, and          │
│ conclusions are entirely the author's own work. The author         │
│ takes full responsibility for the accuracy and integrity of        │
│ this document.                                                     │
│                                                                    │
│ Student Name: ___________________                                  │
│ Date: ___________________                                          │
│ Signature: ___________________                                     │
└────────────────────────────────────────────────────────────────────┘
```

**What to include in a disclosure:**
- Which AI tools you used
- What you used each tool for (be specific)
- Which sections were affected
- A statement that the intellectual content is your own

### AI-Generated Text Detection Tools

Instructors may use detection tools to identify AI-generated text:

| Tool | How It Works | Accuracy |
|------|-------------|----------|
| **Turnitin AI Detection** | Integrated with existing plagiarism checker; analyzes writing patterns | ~80–98% for fully AI text; lower for mixed text |
| **GPTZero** | Analyzes "perplexity" and "burstiness" of text | Good for fully AI text; struggles with edited AI text |
| **Originality.ai** | Scans for AI patterns in sentence structure and vocabulary | Similar accuracy range to GPTZero |

### ⚠️ Critical Limitations of AI Detection Tools

> **WARNING: AI detection tools have serious limitations, especially for non-native English speakers.**

| Limitation | Explanation | Impact on EE Students |
|-----------|-------------|----------------------|
| **False positives** | Tools may flag human-written text as "AI-generated" | Non-native writers who use simple, clear sentences may be falsely accused |
| **Non-native writer bias** | Non-native English writers tend to use patterns similar to AI (short sentences, common vocabulary, standard structures) | Iranian, Algerian, and other non-native EE students are disproportionately affected |
| **Edited AI text** | If a student edits AI output significantly, detection drops dramatically | Tools cannot reliably detect "AI-assisted" writing |
| **Technical writing style** | Scientific writing is naturally formulaic, which can resemble AI patterns | Results sections and methods descriptions may trigger false positives |
| **No tool is 100% accurate** | All tools have error rates | An AI detection score is NOT proof of misconduct |

> 💡 **What this means for you:** If you are falsely accused, you should be able to:
> - Show your drafts and revision history
> - Explain your writing process
> - Demonstrate understanding of the content by answering questions about it
> - Keep notes, outlines, and rough drafts as evidence of your process

### The Fundamental Principle

```
┌────────────────────────────────────────────────────────────────────┐
│                                                                    │
│     ACADEMIC WORK DEMONSTRATES YOUR UNDERSTANDING                  │
│                                                                    │
│     The purpose of writing assignments is NOT to produce           │
│     perfect text — it is to demonstrate that YOU have:             │
│                                                                    │
│     • Understood the concepts                                      │
│     • Analyzed the problem                                         │
│     • Applied your knowledge                                       │
│     • Formed your own conclusions                                  │
│     • Developed your communication skills                          │
│                                                                    │
│     If AI does these things for you, you have NOT learned.         │
│     Your degree will represent knowledge you do not have.          │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Scenario-Based Exercises: "Is This Acceptable?"

**Instructions:** For each scenario below, decide: ✅ Acceptable, ⚠️ Gray area (needs disclosure), or ❌ Unacceptable. Explain your reasoning.

**Scenario 1:**
> Fatima is writing her lab report on a buck converter experiment. She writes her results section in Persian first, then uses ChatGPT to translate it to English. She then reads the English version, corrects two technical errors in the translation, and submits the report with a disclosure note saying "AI-assisted translation was used."

**Scenario 2:**
> Ali has a research paper due about MPPT algorithms. He asks ChatGPT: "Write a 300-word literature review about MPPT algorithms for PV systems." He copies the output directly into his paper, adding [1]–[5] as citations (without checking if those references exist).

**Scenario 3:**
> Sara writes her complete discussion section herself. The English has some grammar mistakes. She pastes it into Grammarly, accepts the grammar corrections, and submits it. She does not include an AI disclosure statement.

**Scenario 4:**
> Karim doesn't understand how the Z-transform works. He asks Claude to "explain the Z-transform and its applications in digital control systems in 200 words, written as if for an assignment." He copies this explanation into his assignment.

**Scenario 5:**
> Maryam writes her abstract for a conference paper. She then asks ChatGPT: "Can you suggest improvements to this abstract?" ChatGPT suggests combining two sentences and changing "utilizes" to "employs." Maryam accepts both suggestions and submits with a disclosure note.

**Scenario 6:**
> Hossein finds a paper about GaN transistors. He copies a paragraph, pastes it into QuillBot set to "Creative" mode, and puts the output in his report with a citation to the original paper but no AI disclosure.

**Model Answers:**

| Scenario | Answer | Reasoning |
|----------|--------|-----------|
| 1 (Fatima) | ✅ Acceptable | She wrote the content herself, used AI for translation only, verified accuracy, and disclosed AI use |
| 2 (Ali) | ❌ Unacceptable | Entirely AI-generated content; fake citations; no understanding demonstrated |
| 3 (Sara) | ✅ Acceptable | Grammar-only corrections are generally accepted without disclosure (like using spell-check); however, some strict policies may require disclosure even for this |
| 4 (Karim) | ❌ Unacceptable | He does not understand the content; the explanation is AI's intellectual work, not his |
| 5 (Maryam) | ✅ Acceptable | She wrote the content; AI only suggested minor improvements; she disclosed |
| 6 (Hossein) | ⚠️ Problematic/Unacceptable | Using AI to paraphrase someone else's work does not constitute genuine paraphrasing; the citation helps, but AI did the intellectual work of rephrasing; AI use was not disclosed |

---

### Updated Academic Integrity Pledge

Below is a sample academic integrity pledge that accounts for AI:

```
┌────────────────────────────────────────────────────────────────────┐
│                ACADEMIC INTEGRITY PLEDGE                            │
│                                                                    │
│ I, _________________________, declare that:                        │
│                                                                    │
│ 1. This work is substantially my own. All ideas, analysis, and    │
│    conclusions represent my genuine understanding.                  │
│                                                                    │
│ 2. All sources used have been properly cited using IEEE format.    │
│                                                                    │
│ 3. I have disclosed all use of AI tools in the attached           │
│    AI Use Disclosure statement, including:                         │
│    • Which tools were used                                         │
│    • For what purpose (grammar, translation, brainstorming, etc.) │
│    • Which sections were affected                                  │
│                                                                    │
│ 4. No portion of this work was generated by AI and presented      │
│    as my own intellectual contribution without disclosure.          │
│                                                                    │
│ 5. I can explain and defend any part of this work if asked.       │
│                                                                    │
│ 6. I understand that violation of this pledge may result in        │
│    academic penalties including a grade of zero.                    │
│                                                                    │
│ Student Name: ___________________                                  │
│ Student ID: ___________________                                    │
│ Course: ___________________                                        │
│ Date: ___________________                                          │
│ Signature: ___________________                                     │
└────────────────────────────────────────────────────────────────────┘
```

### Vocabulary Box: Academic Integrity and AI

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **AI disclosure** | A formal statement declaring how AI tools were used in academic work | Include an AI disclosure at the end of your report if you used ChatGPT. |
| **Academic misconduct** | Any action that gives an unfair advantage or misrepresents one's abilities | Submitting AI-generated text without disclosure is academic misconduct. |
| **False positive** | When a detection tool incorrectly identifies human text as AI-generated | Non-native English writers face higher rates of false positives from AI detectors. |
| **Text perplexity** | A measure of how predictable text is; AI text tends to have low perplexity | AI detection tools measure text perplexity to estimate the likelihood of AI authorship. |
| **Burstiness** | Variation in sentence length and complexity; human text is typically more "bursty" | Human writers naturally vary their sentence length more than AI does. |
| **Intellectual contribution** | The original thinking, analysis, and understanding a student brings to their work | Your intellectual contribution is what makes academic work valuable for your learning. |

---


# WEEK 8: Professional Communication — CV and Cover Letter

## Learning Objectives

By the end of this week, students will be able to:

1. Structure a professional CV tailored to electrical engineering positions
2. Differentiate between a CV and a resume and choose appropriately
3. Identify strengths and weaknesses in CV examples
4. Write an effective cover letter for academic and industry positions
5. Use action verbs and quantifiable achievements in professional documents

---

## 8.1 CV Structure for EE Students

### Recommended CV Sections (in order)

| Section | Content |
|---------|---------|
| **Contact Information** | Full name, address, phone, email, LinkedIn, GitHub/personal website |
| **Education** | Degrees (most recent first), institution, dates, GPA (if strong), relevant coursework |
| **Technical Skills** | Software, programming languages, hardware, lab equipment |
| **Research Experience** | Projects, labs, thesis work |
| **Projects** | Academic and personal engineering projects |
| **Publications** | Papers, conference presentations (if any) |
| **Internships/Work Experience** | Engineering-related positions |
| **Awards & Honors** | Scholarships, competition wins, Dean's list |
| **Languages** | Languages spoken and proficiency levels |
| **Professional Memberships** | IEEE student member, etc. |

### Technical Skills Categories for EE Students

| Category | Examples |
|----------|----------|
| **Simulation Software** | MATLAB/Simulink, PSCAD/EMTDC, ETAP, PowerWorld, HOMER |
| **EDA/CAD Tools** | LTspice, Altium Designer, KiCad, Cadence Virtuoso, Eagle |
| **Programming Languages** | Python, C/C++, VHDL, Verilog, Assembly, MATLAB |
| **HDL/FPGA** | VHDL, Verilog, Xilinx Vivado, Intel Quartus |
| **Embedded Systems** | Arduino, STM32, Raspberry Pi, ESP32, ARM Cortex |
| **Data/ML Tools** | TensorFlow, PyTorch, scikit-learn, Pandas, NumPy |
| **Office/Documentation** | LaTeX, Microsoft Office, Markdown, Git |
| **Lab Equipment** | Oscilloscope, spectrum analyzer, network analyzer, logic analyzer |
| **Standards Knowledge** | IEEE, IEC, NEC, ANSI |

---

## 8.2 CV vs. Resume

| Feature | CV (Curriculum Vitae) | Resume |
|---------|----------------------|--------|
| **Length** | 2+ pages (no limit) | 1–2 pages maximum |
| **Used for** | Academic positions, research, graduate school, international applications | Industry jobs, internships (mainly US/Canada) |
| **Content** | Comprehensive: all publications, presentations, teaching, research | Targeted: only relevant experience for the specific position |
| **Format** | Chronological, detailed | Concise, tailored to each application |
| **Region** | Common worldwide (especially Europe, Middle East, Asia) | Primarily US/Canada |
| **Updates** | Grows over career | Tailored per application |

> 💡 **Tip for EE students:** In most countries outside North America, "CV" is the standard term. For academic positions (Master's/PhD applications, research assistantships), always use a CV format.

---

## 8.3 Weak CV Example (with Problems Identified)

```
                        CURRICULUM VITAE
Name: Mohamed
Email: cool_engineer99@gmail.com                    ❌ Unprofessional email
Phone: 05XXXXXXXX

Education:
I studied electrical engineering at the university   ❌ Narrative style, not bullet points
from 2020 to 2024. I took many courses.             ❌ Vague, no specifics

Skills:
- Computers                                          ❌ Too vague
- Microsoft Word                                     ❌ Not engineering-relevant
- Some programming                                   ❌ Not specific
- MATLAB (beginner)                                  ❌ Don't list "beginner" level skills

Experience:
I worked at a shop in summer 2022.                   ❌ Not relevant
I did a project in school.                           ❌ Vague, no details

Hobbies:
- Football, video games, watching TV                 ❌ Not relevant for engineering CV

References: Available upon request                   ❌ Outdated phrase, wastes space
```

### Problems Identified:
1. ❌ Unprofessional email address
2. ❌ No last name, no LinkedIn/GitHub
3. ❌ Written in paragraph form instead of bullets
4. ❌ No specific courses, GPA, or achievements listed
5. ❌ Skills are vague and include non-technical items
6. ❌ No engineering-related experience or projects
7. ❌ Irrelevant work experience without transferable skills highlighted
8. ❌ Hobbies section adds no value
9. ❌ No publications, awards, or languages section
10. ❌ No action verbs or quantifiable achievements

---

## 8.4 Strong CV Example (with Explanations)

```
═══════════════════════════════════════════════════════════════════
                    MOHAMED BENALI
═══════════════════════════════════════════════════════════════════
📧 m.benali@university.edu | 📱 +213 XX XXX XXXX
🔗 linkedin.com/in/mbenali | 💻 github.com/mbenali-ee

───────────────────────────────────────────────────────────────────
EDUCATION
───────────────────────────────────────────────────────────────────
B.Sc. Electrical Engineering (Power Systems)          2020 – 2024
University of Science and Technology, Oran, Algeria
• GPA: 15.5/20 (Top 10% of class)
• Relevant Coursework: Power Electronics, Control Systems, Digital
  Signal Processing, Renewable Energy Systems, Embedded Systems
• Final Year Project: "Design and Simulation of a Grid-Connected
  PV Inverter with MPPT Control" (Grade: 18/20)

───────────────────────────────────────────────────────────────────
TECHNICAL SKILLS
───────────────────────────────────────────────────────────────────
Simulation:     MATLAB/Simulink, PSCAD/EMTDC, ETAP, LTspice
Programming:    Python, C, VHDL, MATLAB scripting
Hardware:       Arduino, STM32, Raspberry Pi, FPGA (Xilinx)
EDA Tools:      Altium Designer, KiCad, Proteus
Lab Equipment:  Oscilloscope, spectrum analyzer, power analyzer
Other:          LaTeX, Git, Linux, Microsoft Office

───────────────────────────────────────────────────────────────────
RESEARCH EXPERIENCE
───────────────────────────────────────────────────────────────────
Undergraduate Research Assistant                    Sep 2023 – Jun 2024
Power Electronics Laboratory, USTO
• Designed and simulated a three-phase grid-connected inverter using
  MATLAB/Simulink with a novel MPPT algorithm
• Achieved 98.5% maximum power point tracking efficiency under
  varying irradiance conditions (200–1000 W/m²)
• Implemented the control algorithm on an STM32 microcontroller
  for hardware-in-the-loop testing
• Co-authored a conference paper accepted at ICEE 2024

───────────────────────────────────────────────────────────────────
PROJECTS
───────────────────────────────────────────────────────────────────
Smart Home Energy Management System               Mar – May 2023
• Developed a real-time energy monitoring system using ESP32 and
  current/voltage sensors
• Programmed a Python-based dashboard displaying power consumption
  with 95% measurement accuracy
• Implemented automated load scheduling reducing energy usage by 18%

Line-Following Robot with PID Control              Oct – Dec 2022
• Designed and built an autonomous robot using Arduino Mega
• Implemented PID control achieving ±2mm tracking accuracy at 0.5 m/s
• Won 2nd place in the university robotics competition (50 teams)

───────────────────────────────────────────────────────────────────
PUBLICATIONS
───────────────────────────────────────────────────────────────────
[1] M. Benali and A. Khemis, "Adaptive MPPT Algorithm for PV Systems
    Under Partial Shading," in Proc. ICEE, Algiers, 2024, pp. 1–5.

───────────────────────────────────────────────────────────────────
INTERNSHIPS
───────────────────────────────────────────────────────────────────
Engineering Intern                                 Jul – Aug 2023
Sonelgaz (Electricity Distribution), Oran
• Assisted in the maintenance and testing of 30 kV/400 V
  distribution transformers
• Analyzed power quality data and identified 3 harmonic distortion
  issues in industrial feeders
• Prepared technical reports on equipment condition assessment

───────────────────────────────────────────────────────────────────
AWARDS & HONORS
───────────────────────────────────────────────────────────────────
• 2nd Place, University Robotics Competition (2022)
• Dean's Honor List (2021, 2022, 2023)
• National Scholarship for Academic Excellence (2020–2024)

───────────────────────────────────────────────────────────────────
LANGUAGES
───────────────────────────────────────────────────────────────────
Arabic:    Native
French:    Fluent (C1)
English:   Upper-Intermediate (B2)

───────────────────────────────────────────────────────────────────
PROFESSIONAL MEMBERSHIPS
───────────────────────────────────────────────────────────────────
• IEEE Student Member (since 2022)
• IEEE Power & Energy Society (PES) Student Member
```

### Why This CV Works:
- ✅ Professional contact information with LinkedIn and GitHub
- ✅ Specific GPA and class ranking
- ✅ Relevant coursework listed
- ✅ Technical skills organized by category
- ✅ Research experience with quantifiable results
- ✅ Action verbs: designed, simulated, achieved, implemented, co-authored
- ✅ Specific numbers: 98.5% efficiency, ±2mm accuracy, 18% reduction
- ✅ Publication in IEEE format
- ✅ Relevant internship with engineering tasks
- ✅ Awards demonstrate excellence
- ✅ Languages with proficiency levels

---

## 8.5 Action Verbs for Engineering CVs

| Category | Verbs |
|----------|-------|
| **Design** | designed, developed, created, engineered, architected, modeled |
| **Analysis** | analyzed, evaluated, assessed, characterized, investigated, benchmarked |
| **Implementation** | implemented, built, constructed, fabricated, assembled, integrated |
| **Simulation** | simulated, modeled, validated, verified, tested, prototyped |
| **Optimization** | optimized, improved, enhanced, reduced, increased, streamlined |
| **Programming** | programmed, coded, debugged, compiled, automated, scripted |
| **Communication** | presented, published, co-authored, documented, reported, proposed |
| **Leadership** | led, coordinated, supervised, mentored, managed, organized |
| **Research** | researched, investigated, explored, surveyed, reviewed, discovered |

> 💡 **Tip:** Start each bullet point with an action verb. Combine it with a quantifiable result:
> "**Optimized** the PID controller parameters, **reducing** settling time by 40%."

---

## 8.6 Cover Letter Structure

### Components of a Cover Letter

```
┌────────────────────────────────────────────────────────┐
│ YOUR CONTACT INFORMATION                               │
│ Date                                                   │
│ Recipient's Information                                │
├────────────────────────────────────────────────────────┤
│ PARAGRAPH 1: Opening                                   │
│ • State the position you're applying for               │
│ • How you found out about it                           │
│ • Brief statement of why you're a strong candidate     │
├────────────────────────────────────────────────────────┤
│ PARAGRAPH 2: Qualifications & Technical Experience     │
│ • Relevant education and skills                        │
│ • Specific projects/research that match the position   │
│ • Technical achievements with numbers                  │
├────────────────────────────────────────────────────────┤
│ PARAGRAPH 3: Why This Organization                     │
│ • What attracts you to this specific organization      │
│ • How your goals align with their work                 │
│ • What you can contribute                              │
├────────────────────────────────────────────────────────┤
│ PARAGRAPH 4: Closing                                   │
│ • Express enthusiasm                                   │
│ • Request interview/meeting                            │
│ • Thank the reader                                     │
│ • Signature                                            │
└────────────────────────────────────────────────────────┘
```

---

## 8.7 Cover Letter Examples

### Example 1: Internship Application

```
Mohamed Benali
m.benali@university.edu | +213 XX XXX XXXX
linkedin.com/in/mbenali

October 15, 2025

Human Resources Department
Schneider Electric Algeria
Algiers, Algeria

Dear Hiring Manager,

I am writing to apply for the Power Systems Engineering Intern
position advertised on your website (Ref: SE-INT-2025-042). As a
final-year Electrical Engineering student at USTO with a focus on
power electronics and renewable energy, I am eager to contribute
to Schneider Electric's work in smart grid solutions.

During my undergraduate studies, I have developed strong skills in
power system simulation and control. In my final year project, I
designed and simulated a grid-connected PV inverter with an adaptive
MPPT algorithm, achieving 98.5% tracking efficiency in
MATLAB/Simulink. Additionally, during my internship at Sonelgaz, I
gained practical experience in transformer maintenance and power
quality analysis, where I identified harmonic distortion issues in
three industrial feeders. I am proficient in MATLAB/Simulink,
PSCAD/EMTDC, ETAP, Python, and embedded C programming.

I am particularly drawn to Schneider Electric's EcoStruxure platform
and its approach to integrating IoT with power distribution. Your
company's commitment to sustainable energy solutions aligns with my
research interests in renewable energy integration and smart grid
technologies. I believe my combination of simulation experience and
hands-on hardware skills would allow me to contribute meaningfully
to your engineering team.

I would welcome the opportunity to discuss how my skills and
experience align with your team's needs. I am available for an
interview at your convenience. Thank you for considering my
application.

Sincerely,
Mohamed Benali
```

---

### Example 2: Research Assistant Position

```
Mohamed Benali
m.benali@university.edu | +213 XX XXX XXXX

November 5, 2025

Prof. Sarah Chen
Department of Electrical and Computer Engineering
Technical University of Munich
Munich, Germany

Dear Professor Chen,

I am writing to express my interest in the Research Assistant
position in your Power Electronics and Renewable Energy Laboratory,
as advertised on your department website. I recently completed my
B.Sc. in Electrical Engineering at USTO (GPA: 15.5/20, top 10%)
and am seeking a research-intensive Master's program to deepen my
expertise in power electronics for renewable energy applications.

My undergraduate research focused on MPPT algorithms for PV systems
under partial shading conditions. I developed a novel adaptive
algorithm that achieved 98.5% tracking efficiency across varying
irradiance levels (200–1000 W/m²), and this work resulted in a
conference paper at ICEE 2024. I am experienced with
MATLAB/Simulink, PSCAD, and STM32 microcontrollers for
hardware-in-the-loop testing. Additionally, I have completed
coursework in power electronics, control systems, and digital
signal processing, providing a solid theoretical foundation for
your group's research on wide-bandgap semiconductor converters.

Your recent publication on GaN-based multilevel inverters for EV
charging [Chen et al., IEEE TPEL, 2024] particularly captured my
interest, as it aligns with my goal of contributing to
high-efficiency power conversion technologies. I am enthusiastic
about the opportunity to contribute to your ongoing projects while
developing advanced research skills.

I have attached my CV and academic transcripts for your review. I
would be grateful for the opportunity to discuss potential research
projects in your group. Thank you for your time and consideration.

Sincerely,
Mohamed Benali
```

---

### Example 3: Master's Program Application (Motivation Letter)

```
Mohamed Benali
m.benali@university.edu

January 10, 2026

Admissions Committee
M.Sc. Electrical Power Engineering
Aalborg University
Aalborg, Denmark

Dear Admissions Committee,

I am writing to apply for the M.Sc. in Electrical Power
Engineering at Aalborg University for the September 2026 intake. As
a graduate in Electrical Engineering from USTO with a strong
background in power electronics and renewable energy systems, I am
confident that Aalborg's world-renowned power electronics program
will provide the ideal environment to advance my research career.

My undergraduate studies equipped me with comprehensive knowledge
in power systems, power electronics, and control theory. My final
year project — designing a grid-connected PV inverter with adaptive
MPPT control — sparked my passion for power conversion research.
Beyond simulation, I implemented the control algorithm on an STM32
microcontroller, achieving hardware-in-the-loop validation. This
experience taught me the full development cycle from theory to
prototype, and I am eager to develop this expertise further at the
graduate level.

Aalborg University's Department of Energy is globally recognized
for its contributions to power electronics and wind energy
research. The opportunity to work alongside researchers who have
shaped modern converter topologies and grid integration techniques
is highly motivating. Furthermore, Denmark's position as a leader
in renewable energy provides an ideal context for studying power
systems of the future.

I am committed to pursuing a research career in power electronics
for renewable energy, and I believe that Aalborg's program will
provide the skills, mentorship, and environment necessary to
achieve this goal. I look forward to your consideration of my
application.

Sincerely,
Mohamed Benali
```

---

### Example 4: Engineering Job Application

```
Mohamed Benali
m.benali@university.edu | +213 XX XXX XXXX

March 3, 2026

Engineering Recruitment
Huawei Technologies Algeria
Algiers, Algeria

Dear Recruitment Team,

I am applying for the Telecommunications Engineer position
(Ref: HW-TE-2026-015) advertised on LinkedIn. With a B.Sc. in
Electrical Engineering and hands-on experience in signal processing
and embedded systems, I am prepared to contribute to Huawei's 5G
deployment projects in Algeria.

Through my academic training, I have developed expertise in digital
communications, signal processing, and wireless systems. I am
proficient in MATLAB for communication system simulation and have
implemented digital filter designs on FPGA platforms using VHDL. In
a team project, I designed a complete OFDM transceiver simulation
achieving a bit error rate below 10⁻⁴ at 15 dB SNR. My programming
skills in Python and C, combined with experience in embedded
systems (STM32, ESP32), enable me to work effectively on both
software and hardware aspects of telecommunications infrastructure.

Huawei's leadership in 5G technology and its significant investment
in North African telecommunications infrastructure make it an
exciting environment for an early-career engineer. I am particularly
interested in contributing to radio access network optimization and
look forward to applying my signal processing skills to real-world
deployment challenges.

I would appreciate the opportunity to discuss this position further
and am available for an interview at your convenience. Thank you for
your consideration.

Sincerely,
Mohamed Benali
```

---

## 8.8 Vocabulary Box

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Curriculum Vitae (CV)** | A comprehensive document detailing academic and professional history | Submit your CV along with your application for the research position. |
| **Cover letter** | A formal letter accompanying a CV that explains motivation and qualifications | The cover letter should be tailored to each specific position. |
| **Action verb** | A strong verb that describes an accomplishment | Use action verbs like "designed," "implemented," and "optimized" to describe achievements. |
| **Quantifiable achievement** | An accomplishment described with specific numbers or metrics | "Reduced processing time by 35%" is a quantifiable achievement. |
| **Transferable skills** | Skills applicable across different positions or industries | Problem-solving and programming are transferable skills for engineers. |
| **Tailored application** | An application customized for a specific position or organization | A tailored cover letter references the specific company and role. |
| **Professional profile** | A brief summary of qualifications and career goals at the top of a CV | A professional profile should be 2–3 sentences summarizing your expertise. |

---

## 8.9 Exercises and Activities

### Activity: Draft Your Own CV

Using the template and strong example above, create your own CV. Include:

1. ✅ Professional contact information
2. ✅ Education with GPA and relevant coursework
3. ✅ Technical skills organized by category
4. ✅ At least 2 projects with action verbs and results
5. ✅ Any internship or work experience (highlight engineering-relevant aspects)
6. ✅ Languages with proficiency levels

**Peer Review:** Exchange CVs with a partner. Using the checklist below, identify 3 strengths and 3 areas for improvement.

| Checklist Item | Yes/No | Comments |
|---------------|--------|----------|
| Professional email address | | |
| Clear, consistent formatting | | |
| Action verbs used for descriptions | | |
| Quantifiable achievements included | | |
| Technical skills specific and categorized | | |
| No spelling or grammar errors | | |
| Relevant to engineering career | | |
| Appropriate length (1–2 pages) | | |

---

## 8.10 Homework

**Assignment:** Write a cover letter (250–350 words) for ONE of the following scenarios:

1. A summer internship at a renewable energy company
2. A research assistant position in a university power electronics lab
3. A Master's program in telecommunications engineering
4. A junior engineer position at a telecommunications company

**Requirements:**
- Follow the 4-paragraph structure
- Reference specific skills and projects from your CV
- Include at least 3 action verbs
- Mention something specific about the organization
- Professional formatting and tone
- No grammatical errors

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Correct structure (4 paragraphs) | /2 |
| Position clearly stated | /1 |
| Relevant qualifications highlighted | /2 |
| Specific achievements with numbers | /2 |
| Organization-specific content | /1 |
| Professional language and tone | /1 |
| No errors | /1 |
| **Total** | **/10** |

---

## 8.11 Tips and Common Mistakes

### ✅ Tips for CVs

1. **Tailor to the position** — reorder sections based on what's most relevant
2. **Use numbers everywhere** — "Improved efficiency by 20%" beats "Improved efficiency"
3. **Keep it updated** — add new projects and skills regularly
4. **Use consistent formatting** — same fonts, spacing, and bullet styles throughout
5. **Proofread** — one typo can disqualify you

### ✅ Tips for Cover Letters

1. **Never send a generic letter** — customize for each application
2. **Research the organization** — mention specific projects, products, or papers
3. **Show, don't tell** — instead of "I am hardworking," give an example
4. **Keep it concise** — one page maximum
5. **Match keywords** — use terminology from the job posting

### ❌ Common Mistakes

| Document | Mistake | Fix |
|----------|---------|-----|
| CV | Using "responsible for..." | Use action verbs: "designed," "implemented" |
| CV | Including photo (in some countries) | Check the country's conventions |
| CV | Listing every course taken | Only list relevant coursework |
| CV | "References available upon request" | Remove — it's assumed |
| Cover Letter | Starting with "My name is..." | Start with the position and your interest |
| Cover Letter | Repeating the CV word-for-word | Highlight key points and add context |
| Cover Letter | "I think I might be a good fit" | Be confident: "My experience in X qualifies me for Y" |
| Cover Letter | Forgetting to proofread | Read aloud and ask someone to review |

---

## 8.12 Using AI Responsibly in the Writing Process

### Where AI Can Help in Article/Report Writing

AI tools can legitimately assist at several stages of writing a technical paper or report:

| Writing Stage | How AI Can Help | Example |
|---------------|----------------|---------|
| **Brainstorming** | Generate topic ideas, suggest angles you haven't considered | "What are current challenges in grid-connected PV inverters?" |
| **Outline feedback** | Review your outline structure and suggest gaps | "Here's my outline for a paper on SiC converters. What sections might I be missing?" |
| **Grammar checking** | Fix errors in your drafted text | Paste your paragraph → get grammar corrections |
| **Sentence clarity** | Suggest clearer ways to express your ideas | "How can I make this sentence clearer: [your sentence]?" |
| **Vocabulary** | Find the right technical term in English | "What's the engineering term for when a system oscillates before settling?" |
| **Formatting** | Help with LaTeX formatting, IEEE reference formatting | "Format this reference in IEEE style: [details]" |

### Where AI Should NOT Be Used

> ❌ **Never use AI for these critical sections — they must represent YOUR work:**

| Section | Why AI Is Inappropriate |
|---------|------------------------|
| **Methodology** | This section describes what YOU did. AI cannot know your actual experimental setup, equipment, procedures, or decisions. |
| **Results** | These are YOUR measurements and data. AI cannot generate real experimental results. Fabricating results is research fraud. |
| **Analysis/Discussion** | This demonstrates YOUR understanding of what the results mean. If AI writes your analysis, you have not demonstrated learning. |
| **Original conclusions** | These are YOUR intellectual contributions based on YOUR evidence. |
| **Literature review content** | AI may hallucinate references that don't exist. You must read and understand the papers yourself. |

**Example of why this matters in EE:**
> You measure the THD (Total Harmonic Distortion) of your inverter output at 4.7%. AI cannot tell you whether this meets IEEE 519 standards for your specific application, whether your measurement setup introduced errors, or why the 5th harmonic is unexpectedly high. That requires YOUR engineering knowledge.

### The Responsible AI Writing Workflow

Follow this four-step workflow:

```
┌──────────────────────────────────────────────────────────────────┐
│                                                                    │
│   Step 1: WRITE FIRST                                             │
│   ─────────────────                                               │
│   Write your own draft. Get your ideas on paper.                  │
│   It doesn't need to be perfect — just get YOUR                   │
│   thoughts and analysis written down.                             │
│                                                                    │
│   Step 2: USE AI TO IMPROVE                                       │
│   ─────────────────────────                                       │
│   After writing, use AI to:                                       │
│   • Check grammar and spelling                                    │
│   • Suggest clearer sentence structures                           │
│   • Identify unclear passages                                     │
│   • Improve transitions between paragraphs                        │
│                                                                    │
│   Step 3: VERIFY ACCURACY                                         │
│   ────────────────────────                                        │
│   Read the AI-improved version carefully:                         │
│   • Did AI change any technical meaning?                          │
│   • Are all numbers and specifications still correct?             │
│   • Does it still say what YOU meant to say?                      │
│   • Are any AI-introduced claims unsupported?                     │
│                                                                    │
│   Step 4: DISCLOSE AI USE                                         │
│   ─────────────────────                                           │
│   Add a disclosure statement noting:                              │
│   • Which tool(s) you used                                        │
│   • What you used them for                                        │
│   • Which sections were affected                                  │
│                                                                    │
└──────────────────────────────────────────────────────────────────┘
```

### Practical Demo: Using AI to Get Feedback on an Abstract Draft

**Your first draft (before AI):**
> "This paper present a design of boost converter for PV system. The converter use a new MPPT algorithm based on fuzzy logic. We simulate the system in MATLAB. The results show that the efficiency is improved compared to P&O method. The converter works good under different irradiance conditions."

**Your prompt to AI:**
> "I am an EE undergraduate writing a paper abstract. Please check the grammar and suggest improvements to make this more formal and precise. Do NOT change the technical content or add information I haven't provided:
>
> [paste your draft above]"

**AI response:**
> "Here's a corrected version with grammar fixes and improved formality:
>
> 'This paper presents the design of a boost converter for a photovoltaic (PV) system. The converter employs a novel MPPT algorithm based on fuzzy logic. The system was simulated in MATLAB/Simulink. The results demonstrate improved efficiency compared to the conventional perturb and observe (P&O) method. The converter maintains performance under varying irradiance conditions.'
>
> Changes made:
> - 'present' → 'presents' (subject-verb agreement)
> - 'use' → 'employs' (more formal)
> - 'works good' → 'maintains performance' (more academic)
> - Added 'photovoltaic (PV)' for first-use definition
> - Changed 'improved' phrasing for clarity"

**What YOU should do next:**
1. ✅ Accept the grammar corrections (subject-verb agreement, etc.)
2. ✅ Accept the formality improvements ("employs" instead of "use")
3. ⚠️ ADD specific numbers: What efficiency? What improvement percentage?
4. ⚠️ ADD scope: How many irradiance conditions? What range?
5. ⚠️ The AI version is still weak because it lacks YOUR specific data

**Your final version (after AI grammar help + your additions):**
> "This paper presents the design of a boost converter with a fuzzy logic-based MPPT algorithm for photovoltaic (PV) systems. The proposed controller was simulated in MATLAB/Simulink under irradiance variations from 200 to 1000 W/m². Results demonstrate that the fuzzy MPPT achieves 98.3% tracking efficiency with a response time of 45 ms, representing a 12% improvement in dynamic response compared to the conventional perturb and observe (P&O) method. The converter maintains efficiency above 95% across the entire operating range."

> 💡 **Notice:** The AI fixed your grammar, but YOU added the specific numbers (98.3%, 45 ms, 12%, 200–1000 W/m²) that make the abstract convincing. Those numbers come from YOUR simulation — AI cannot provide them.

### Exercise: AI-Assisted Writing Workflow Practice

**Instructions:** Follow the four-step workflow for the following task.

**Task:** Write a 100-word abstract for a paper titled "Design of a PID Controller for DC Motor Speed Control."

1. **Step 1 — Write your own first draft** (even if the English is imperfect). Include:
   - What you did (method)
   - What results you got (with specific numbers — invent realistic values)
   - Why it matters (significance)

2. **Step 2 — Identify what AI could improve.** Underline sentences where you think AI help with grammar or clarity would be appropriate.

3. **Step 3 — For each underlined sentence, write the specific prompt you would give AI.** (Do NOT actually use AI — just write what you would ask.)

4. **Step 4 — Write a disclosure statement** for this abstract assuming you used Grammarly for grammar correction and ChatGPT to improve one sentence.

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| First draft contains own ideas and specific data | /3 |
| Correctly identifies areas where AI help is appropriate | /2 |
| Prompts are specific and appropriate (not asking AI to write content) | /2 |
| Disclosure statement is complete and honest | /2 |
| Understands boundary between AI-appropriate and AI-inappropriate tasks | /1 |
| **Total** | **/10** |

---

---


# WEEK 9: Email Writing — Academic and Professional

## Learning Objectives

By the end of this week, students will be able to:

1. Write clear, professional academic emails to professors and researchers
2. Compose effective professional emails for industry communication
3. Structure emails with appropriate subject lines, greetings, body, and closings
4. Identify and correct common email writing mistakes
5. Adapt email tone and style to different recipients and purposes
6. Apply cultural awareness in professional communication

---

## 9.1 Academic Email Types

### Types of Academic Emails

| Purpose | Recipient | Key Considerations |
|---------|-----------|-------------------|
| Requesting information | Professor/Administrator | Be specific about what you need |
| Asking for a meeting | Professor/Supervisor | Propose specific times |
| Submitting an assignment | Professor/TA | Mention course code and deadline |
| Asking about research opportunities | Professor (other university) | Show you've read their work |
| Requesting a recommendation letter | Professor | Give sufficient advance notice |
| Following up on a previous email | Anyone | Reference the original email |
| Requesting an extension | Professor | Provide valid reason, propose new date |

### Academic Email Structure

```
SUBJECT LINE: [Course Code] - [Specific Purpose]
─────────────────────────────────────────────────
Dear Professor [Last Name],

[Opening: State who you are and your purpose]
[Body: Provide necessary details/context]
[Request: State clearly what you need]
[Closing: Thank them and offer availability]

Best regards,
[Your Full Name]
[Student ID]
[Program/Department]
[University]
```

---

## 9.2 Professional Email Types

### Types of Professional Emails

| Purpose | Recipient | Key Considerations |
|---------|-----------|-------------------|
| Requesting technical information | Engineer/Company | Be specific and professional |
| Inquiring about internship | HR/Manager | Attach CV, be concise |
| Following up after a meeting | Business contact | Reference the meeting specifics |
| Requesting collaboration | Researcher/Company | Explain mutual benefit |
| Submitting a report/deliverable | Supervisor/Client | Summarize contents clearly |
| Scheduling a meeting | Colleague/Partner | Propose options |

---

## 9.3 Email Structure in Detail

### Subject Line

| ❌ Bad Subject Lines | ✅ Good Subject Lines |
|---------------------|---------------------|
| Hi | EE401 – Request for Project Extension (Due Oct 20) |
| Question | Inquiry: Research Assistant Position in Power Electronics Lab |
| URGENT!!! | Meeting Request – Thesis Progress Discussion (Week 6) |
| (no subject) | Application: Summer Internship – Power Systems Division |
| Help me please | Request for Technical Documentation – Model XR-500 Inverter |

### Greeting

| Context | Appropriate Greeting |
|---------|---------------------|
| Professor you know | Dear Professor [Last Name], |
| Professor you don't know | Dear Professor [Last Name], |
| Generic department contact | Dear Sir/Madam, |
| Company/HR | Dear Hiring Manager, / Dear [Name], |
| Colleague/peer | Dear [First Name], / Hello [First Name], |
| Group email | Dear Team, / Dear Colleagues, |

> ⚠️ **Never use:** "Hey," "Hi there," "Yo," "Dear Sir" (without /Madam if gender unknown)

### Body Structure

1. **Self-identification** (if writing to someone who may not know you)
2. **Purpose statement** (why you are writing — first 1–2 sentences)
3. **Details/Context** (necessary background information)
4. **Clear request** (what you need from them)
5. **Facilitating information** (your availability, attachments, etc.)

### Closing

| Formality Level | Options |
|----------------|---------|
| Formal | Sincerely, / Respectfully, / Yours faithfully, |
| Semi-formal | Best regards, / Kind regards, / With best regards, |
| Professional peer | Best, / Regards, / Thank you, |

---

## 9.4 Bad Email vs. Improved Email Examples

### Pair 1: Emailing a Professor About Research

**❌ Bad Email:**
```
Subject: hey

hey prof,

i want to do research with you. when can i start??
let me know asap.

thanks
mohamed
```

**Problems:** No subject line info, too informal greeting, no self-identification, no evidence of knowing the professor's work, demanding tone, no signature block.

**✅ Improved Email:**
```
Subject: Inquiry – Undergraduate Research Opportunity in Power Electronics

Dear Professor Khemis,

My name is Mohamed Benali, and I am a third-year Electrical
Engineering student at USTO (Student ID: 192035XXX). I am writing
to inquire about potential undergraduate research opportunities in
your Power Electronics Laboratory.

I have completed coursework in Power Electronics (Grade: 17/20) and
Control Systems, and I am particularly interested in your recent
work on multilevel inverter topologies for renewable energy
applications [published in IEEE TPEL, 2024]. My final-year project
focuses on MPPT algorithms for PV systems, and I believe there is
a strong connection between my project and your group's research on
grid-connected converters.

I would be grateful for the opportunity to meet with you to discuss
how I might contribute to your current projects. I am available on
Tuesdays and Thursdays after 2:00 PM. I have attached my CV and
transcript for your reference.

Thank you for your time and consideration.

Best regards,
Mohamed Benali
B.Sc. Electrical Engineering (3rd Year)
University of Science and Technology, Oran
m.benali@university.edu | +213 XX XXX XXXX
```

---

### Pair 2: Requesting a Deadline Extension

**❌ Bad Email:**
```
Subject: assignment

hi,

sorry i cant submit the assignment on time. can i have more time?
im really busy with other stuff.

thanks
```

**Problems:** Vague subject, no course info, no valid reason given, no proposed new date, no professional tone.

**✅ Improved Email:**
```
Subject: EE401 – Request for Extension on Lab Report 3 (Due Oct 15)

Dear Professor Mansouri,

I am writing to respectfully request a short extension for Lab
Report 3 in EE401 (Power Electronics), which is currently due on
October 15, 2025.

Unfortunately, I experienced a hardware failure in my simulation
computer this week, which has delayed my MATLAB/Simulink analysis.
I have arranged access to the university computing lab and estimate
I can complete the report by October 18 (three additional days).

I understand the importance of meeting deadlines and apologize for
any inconvenience. If this extension is not possible, I would
appreciate any guidance you could offer.

Thank you for your understanding.

Best regards,
Mohamed Benali
Student ID: 192035XXX
EE401 – Power Electronics (Section A)
```

---

### Pair 3: Professional Email Requesting Technical Documentation

**❌ Bad Email:**
```
Subject: need info

hi,

i need the datasheet for your inverter. send it to me please.

mohamed
```

**Problems:** Vague subject, no identification of sender or company context, rude tone, no specific product identified, no professional formatting.

**✅ Improved Email:**
```
Subject: Request for Technical Documentation – SolarEdge SE5000H Inverter

Dear SolarEdge Technical Support Team,

I am Mohamed Benali, a final-year Electrical Engineering student at
the University of Science and Technology, Oran, Algeria. I am
currently working on my graduation project, which involves the
design and simulation of a residential grid-connected PV system.

I am writing to request the detailed technical datasheet and
application notes for the SolarEdge SE5000H single-phase inverter,
specifically:
• Electrical specifications (efficiency curves, voltage/current
  ratings)
• Communication protocols (RS485, Wi-Fi interface specifications)
• Grid code compliance certifications (EN 50549, VDE-AR-N 4105)

This documentation will support the simulation and validation
phases of my academic project. Any additional design guides or
reference schematics would also be greatly appreciated.

Thank you for your assistance. Please let me know if any additional
information is required from my side.

Best regards,
Mohamed Benali
B.Sc. Electrical Engineering Student
University of Science and Technology, Oran
m.benali@university.edu | +213 XX XXX XXXX
```

---

### Pair 4: Following Up After a Career Fair

**❌ Bad Email:**
```
Subject: we met

hi,

we talked at the career fair. do you have any jobs?

mohamed
```

**✅ Improved Email:**
```
Subject: Follow-Up – Career Fair Conversation (November 12, Power Systems Division)

Dear Mr. Hamidi,

Thank you for taking the time to speak with me at the USTO Career
Fair on November 12. I enjoyed learning about Sonelgaz's ongoing
projects in smart grid modernization and distribution automation.

As we discussed, I am a final-year Electrical Engineering student
with experience in power system simulation (ETAP, PSCAD) and
embedded systems. I was particularly interested in the SCADA
upgrade project you mentioned and would welcome the opportunity to
contribute as a summer intern.

I have attached my CV for your reference. Would it be possible to
schedule a brief call to discuss internship opportunities in your
division? I am available at your convenience.

Thank you again for the informative conversation. I look forward
to hearing from you.

Best regards,
Mohamed Benali
B.Sc. Electrical Engineering (Final Year)
USTO, Oran
m.benali@university.edu | +213 XX XXX XXXX
```

---

## 9.5 Common Mistakes in Email Writing

| Mistake | Example | Correction |
|---------|---------|-----------|
| No subject line | (empty) | Always include a specific, descriptive subject |
| Too casual tone | "Hey prof, what's up?" | "Dear Professor [Name]," |
| Wall of text | One massive paragraph | Break into logical paragraphs (3–5 sentences each) |
| Unclear purpose | Rambling without stating what's needed | State your request in the first 2 sentences |
| Not proofreading | "i would liek to now about..." | Always proofread before sending |
| Demanding tone | "I need this by tomorrow." | "I would be grateful if this could be provided by..." |
| Missing context | "About the project..." | Specify which project, course, date |
| Attaching without mentioning | (file attached but not referenced) | "Please find attached my CV and transcript." |
| Reply-all unnecessarily | Replying to entire department | Reply only to relevant recipients |
| Excessive follow-ups | 3 emails in 24 hours | Wait at least 5–7 working days before following up |

---

## 9.6 Useful Phrases for Email Writing

### Opening Phrases

| Purpose | Phrases |
|---------|---------|
| Self-introduction | "My name is [X], and I am a [year] student in [program] at [university]." |
| Stating purpose | "I am writing to inquire about..." / "I am writing regarding..." / "I am writing to request..." |
| Referencing previous contact | "Following our conversation on [date]..." / "Thank you for your email of [date]." |
| Responding to something | "Thank you for your prompt response." / "I appreciate you taking the time to..." |

### Body Phrases

| Purpose | Phrases |
|---------|---------|
| Providing context | "For context, I am currently working on..." / "As background, my research focuses on..." |
| Making a request | "I would be grateful if you could..." / "Would it be possible to..." / "I would appreciate it if..." |
| Offering information | "Please find attached..." / "For your reference, I have included..." |
| Expressing interest | "I am particularly interested in..." / "Your work on [X] aligns closely with..." |
| Proposing times | "I am available on [days] between [times]." / "Would [date/time] be convenient for you?" |

### Closing Phrases

| Purpose | Phrases |
|---------|---------|
| Expressing gratitude | "Thank you for your time and consideration." / "I appreciate your assistance." |
| Indicating next steps | "I look forward to your response." / "Please let me know if you need additional information." |
| Offering flexibility | "I am happy to provide further details if needed." / "Please do not hesitate to contact me." |
| Polite urgency | "If possible, a response by [date] would be appreciated." |

---

## 9.7 Cultural Considerations in Professional Communication

### Cross-Cultural Email Norms

| Aspect | Formal Cultures (e.g., Germany, Japan) | Less Formal Cultures (e.g., USA, Australia) |
|--------|---------------------------------------|---------------------------------------------|
| **Greeting** | Full title + last name always | May use first name after initial contact |
| **Directness** | May use indirect language | Direct requests are acceptable |
| **Small talk** | Minimal in emails | Brief pleasantry may be appropriate |
| **Response time** | Allow more time | Expect faster responses |
| **Sign-off** | Very formal closings | "Best" or "Thanks" acceptable |

### Universal Best Practices

1. **When in doubt, be more formal** — you can always become less formal later
2. **Use the recipient's title** until they invite you to use their first name
3. **Avoid idioms and slang** — they may not translate across cultures
4. **Be explicit** — don't assume shared context
5. **Proofread for tone** — read your email as if you were the recipient
6. **Consider time zones** — don't expect immediate responses from other countries
7. **Respect hierarchies** — address the most senior person appropriately

### Email Etiquette for Different Scenarios

| Scenario | Guideline |
|----------|-----------|
| Emailing a professor for the first time | Use "Dear Professor [Last Name]" — never first name |
| Professor replies with first name | You may use "Dear [First Name]" in subsequent emails |
| Emailing someone more senior | Formal tone, concise, respectful of their time |
| Group project emails | CC relevant members, use clear subject lines |
| Late response (you delayed replying) | "I apologize for the delayed response." |
| No response after 7 days | Send a polite follow-up referencing your original email |

---

## 9.8 Vocabulary Box

| Term | Definition | Example Sentence |
|------|-----------|-----------------|
| **Subject line** | The brief header of an email indicating its topic | A clear subject line helps recipients prioritize emails. |
| **CC (Carbon Copy)** | Sending a copy of the email to additional recipients for information | CC your supervisor when sending project updates to the client. |
| **BCC (Blind Carbon Copy)** | Sending a copy without other recipients knowing | Use BCC for large distribution lists to protect privacy. |
| **Attachment** | A file sent along with an email | Always mention attachments in the body of the email. |
| **Follow-up** | A subsequent email sent after not receiving a response | Send a follow-up email if you haven't received a response within a week. |
| **Tone** | The attitude or feeling conveyed in writing | Professional emails should maintain a respectful and courteous tone. |
| **Recipient** | The person or people receiving the email | Consider who the primary recipient is versus who should be CC'd. |
| **Etiquette** | Conventional rules for polite behavior in communication | Email etiquette varies across cultures and professions. |

---

## 9.9 Exercises and Activities

### Activity 1: Write an Email to a Professor Requesting to Join Their Research Group

**Scenario:** You are interested in joining Professor Ahmed Kara's research group at the University of Blida. His group works on smart grid cybersecurity and published a recent paper on "Intrusion Detection Systems for SCADA Networks Using Deep Learning" in IEEE Access (2024). You have relevant skills in Python programming, machine learning (TensorFlow), and network security coursework.

**Write a complete email including:**
- Appropriate subject line
- Proper greeting
- Self-identification (invent realistic details)
- Why you are interested in their specific research
- Your relevant skills and experience
- A clear request
- Professional closing with full signature

---

### Activity 2: Write a Professional Email Requesting Technical Documentation

**Scenario:** You are working on your graduation project: "Design of a 10 kW Off-Grid Solar PV System for a Rural School." You need the technical datasheet for the Victron Energy MultiPlus-II 48/5000 inverter/charger, including efficiency curves, battery charging algorithms, and communication protocol specifications.

**Write a complete email to Victron Energy's technical support team.**

---

### Exercise: Identify and Fix Email Problems

Read the following emails and identify ALL problems. Then rewrite each email correctly.

**Email A:**
```
to: prof.harris@mit.edu
subject: stuff

Hey!

So basically I need a recommendation letter for grad school.
Can you write one? Its due next week. Also can you make it
really good lol. I was in your class 2 years ago btw.

Thx!!
Mike
```

**Problems to identify:** (Students list at least 6 problems, then rewrite)

**Email B:**
```
to: support@texasinstruments.com
subject: URGENT HELP NEEDED ASAP!!!

Dear Texas Instruments,

I am a student and I need help with my project. The chip
doesn't work. I tried everything but it still doesn't work.
I don't know what to do. Can someone help me??? I need this
fixed by tomorrow because my project is due.

Please respond immediately.

A student
```

**Problems to identify:** (Students list at least 6 problems, then rewrite)

---

## 9.10 Homework

**Assignment:** Write 2 complete emails based on the following scenarios:

### Email 1 (Academic):
You want to apply for a summer research internship at a university abroad. Write to Professor Maria Santos at the University of Porto, Portugal. Her research group works on "Energy Storage Systems for Microgrids." You found her work through a recent IEEE Transactions paper. Explain your background, relevant skills, and interest in a specific aspect of her research.

### Email 2 (Professional):
You attended a webinar organized by ABB on "Digital Substations and IEC 61850 Communication." During the Q&A, you asked a question about protocol implementation that wasn't fully answered. Write a follow-up email to the presenter, Mr. Erik Johansson (Senior Engineer, ABB Power Grids, Sweden), thanking him for the presentation and asking your question in detail.

**Requirements for both emails:**
- Professional subject line
- Appropriate greeting and closing
- Clear purpose stated early
- Proper self-identification
- Specific, relevant details (not vague)
- Correct grammar and spelling
- Full signature block
- 150–250 words each (body only)

**Assessment Criteria:**

| Criterion | Marks (per email) |
|-----------|-------------------|
| Appropriate subject line | /1 |
| Proper greeting and closing | /1 |
| Clear purpose and request | /2 |
| Professional tone and language | /2 |
| Specific details and context | /2 |
| Correct grammar/spelling | /1 |
| Proper signature | /1 |
| **Total (per email)** | **/10** |

---

## 9.11 Tips and Common Mistakes

### ✅ Tips for Effective Email Writing

1. **Draft, wait, revise** — never send an important email immediately; review after 10 minutes
2. **One email, one purpose** — if you have multiple unrelated requests, send separate emails
3. **Keep it short** — aim for 3–5 short paragraphs maximum for the body
4. **Make action items clear** — the recipient should know exactly what you need
5. **Use bullet points** for multiple items or questions
6. **Check attachments** before sending — verify the correct file is attached
7. **Use "Reply All" carefully** — only when everyone needs the information
8. **Time your emails** — avoid sending at midnight or weekends for non-urgent matters
9. **Read it from the recipient's perspective** — would you respond positively to this email?
10. **Save templates** for common email types, but always personalize them

### ❌ Common Mistakes Summary

| Category | Mistake | Impact |
|----------|---------|--------|
| **Tone** | Too casual or too demanding | Recipient feels disrespected |
| **Structure** | No clear request | Recipient doesn't know what to do |
| **Subject** | Vague or missing | Email may be ignored or lost |
| **Length** | Too long (> 500 words) | Recipient won't read it all |
| **Timing** | Following up too soon (< 3 days) | Appears impatient |
| **Proofreading** | Typos, wrong name | Appears careless |
| **Attachments** | Forgetting or wrong file | Wastes time, unprofessional |
| **Context** | Assuming recipient remembers you | Include relevant background |

---

## 9.12 AI Tools for Professional Communication

### Using AI to Draft Emails

AI can help you draft professional emails — but you must **always review and personalize** before sending.

**Appropriate workflow:**
1. Write a rough draft or outline of what you want to say
2. Ask AI to help with tone, structure, or grammar
3. Review the AI output and personalize it with YOUR specific details
4. Never send an AI-generated email without reading it carefully

**Example — Using AI to improve an email draft:**

> **Your rough notes:** "Want to email Prof. about joining research group. I know MATLAB, did PV project, interested in their paper on SiC converters."
>
> **Your prompt to AI:** "Help me structure a professional email to a professor asking about research opportunities. I'll provide the details — just help with tone and structure."
>
> **What AI produces:** A template/structure with professional phrasing
>
> **What YOU add:** Your specific name, the professor's specific paper you read, your specific project results, your specific availability

> ⚠️ **Warning:** An email that sounds like AI wrote it (perfectly structured, no personal details, generic compliments) will be obvious to the recipient. Professors receive many AI-generated emails — they recognize them.

### Using AI to Improve CV Bullet Points

AI can help transform weak, passive CV descriptions into strong, action-oriented bullet points:

**Before (weak):**
| Original Bullet Point | Problem |
|----------------------|---------|
| "Was responsible for testing circuits" | Passive, vague |
| "Worked on a power electronics project" | No action verb, no result |
| "Did programming in MATLAB" | Weak verb, no context |

**After (AI-assisted improvement + your personalization):**
| AI Suggestion | Your Final Version (with specific details) |
|--------------|---------------------------------------------|
| "Tested and validated circuit designs to ensure performance specifications" | "Tested and validated a 3-stage RF amplifier across 1–6 GHz, confirming gain flatness within ±0.5 dB" |
| "Developed a power electronics project utilizing simulation and hardware implementation" | "Designed a 500 W boost converter in MATLAB/Simulink, achieving 96.2% efficiency at rated load" |
| "Developed MATLAB scripts for data analysis and system simulation" | "Developed MATLAB scripts automating spectral analysis of 50,000+ measurement points, reducing processing time by 75%" |

> 💡 **Key Point:** AI gives you the structure (action verb + task + result). YOU provide the specific numbers, contexts, and achievements that make it real.

### Using AI to Check Tone and Formality in Cover Letters

AI can help you verify that your cover letter has the right tone:

**Useful prompts:**
- "Is this cover letter too formal or too casual for an internship application?"
- "Does this paragraph sound confident or arrogant?"
- "Is my closing paragraph polite but assertive?"

**Example — Tone check:**

> **Your sentence:** "I really want this job and I think I'd be amazing at it."
>
> **AI feedback:** "This is too informal and sounds overconfident. Consider: 'My experience in [X] and skills in [Y] position me well to contribute to your team's work on [Z].'"
>
> **Your improved version:** "My experience in power system simulation and hands-on skills in embedded C programming position me well to contribute to your team's smart grid deployment projects."

### ⚠️ Warning: AI-Generated Cover Letters Sound Generic

**Signs that a cover letter was AI-generated (recruiters notice these):**
- Generic compliments: "Your esteemed organization is a leader in innovation"
- No specific details: No mention of specific projects, products, or recent news
- Perfect but soulless: Grammatically perfect but no personality or genuine enthusiasm
- Template phrases: "I am confident that my skills and experience make me an ideal candidate"
- No connection to YOUR story: Could be sent by any applicant

**How to fix AI-assisted cover letters:**
1. Add a specific detail about WHY you want this company (a paper they published, a product you used, a project you admire)
2. Connect your specific experiences (with numbers) to their specific needs
3. Show personality: What genuinely excites you about this opportunity?
4. Reference something that shows you researched them (not just read the job posting)

### Exercise: Use AI to Improve CV Bullet Points

**Instructions:** Below are 5 weak CV bullet points from an EE student. For each one:
- (a) Identify the problem(s)
- (b) Write the prompt you would give AI to improve it
- (c) Write the AI-improved version (imagine a reasonable AI response)
- (d) Add YOUR personal details (invent realistic specific numbers and context) to make it authentic

**Weak bullet points:**

1. "Helped with the solar panel project in the lab"
2. "Did some programming for my embedded systems course"
3. "Was part of a team that worked on telecommunications"
4. "Used MATLAB sometimes for analysis"
5. "Participated in a robotics competition"

**Model Answer for #1:**

- (a) **Problems:** Passive ("helped"), vague ("solar panel project"), no result, no action verb
- (b) **Prompt:** "Rewrite this CV bullet point to start with a strong action verb and include a result: 'Helped with the solar panel project in the lab'"
- (c) **AI output:** "Contributed to the design and testing of a solar panel system, supporting data collection and performance analysis"
- (d) **Your personalized version:** "Designed and tested a 2 kW rooftop PV monitoring system using ESP32 sensors, achieving ±2% measurement accuracy for irradiance and power output across 6 months of continuous operation"

**Assessment Criteria:**

| Criterion | Marks |
|-----------|-------|
| Correctly identifies problems in weak bullets | /2 |
| Prompts are specific and appropriate | /2 |
| AI-improved versions use action verbs and results | /3 |
| Personalized versions include specific, realistic details | /3 |
| **Total** | **/10** |

---

---

## 9.13 Email Templates

### Template 1: Requesting a Meeting with Your Supervisor

```
Subject: Meeting Request – [Topic] (Week [X])

Dear Professor [Last Name],

I hope this email finds you well. I am writing to request a
meeting to discuss [specific topic — e.g., "my thesis progress
and the simulation results from Chapter 3"].

I have [completed X / encountered a challenge with Y / prepared Z
for your review]. I would appreciate your guidance on [specific
question or decision].

I am available on:
• [Day 1], [Time range]
• [Day 2], [Time range]
• [Day 3], [Time range]

Please let me know which time would be convenient for you, or
suggest an alternative if none of these work.

Thank you for your time.

Best regards,
[Full Name]
[Program/Year]
[Student ID]
```

### Template 2: Inquiring About a Research Position

```
Subject: Inquiry – [Position Type] in [Research Area]

Dear Professor [Last Name],

My name is [Full Name], and I am a [year/degree] student in
[Department] at [University]. I am writing to inquire about
potential [research assistant / graduate student / intern]
positions in your [Lab/Group Name].

I have read your recent publication on "[Paper Title]" in
[Journal/Conference, Year], and I am particularly interested in
[specific aspect of their work]. My background in [relevant
skills/courses] has prepared me to contribute to [specific area
of their research].

Specifically, I have experience with:
• [Skill/Tool 1] — [brief context]
• [Skill/Tool 2] — [brief context]
• [Relevant project or coursework]

I have attached my CV [and transcript] for your consideration.
I would be grateful for the opportunity to discuss how I might
contribute to your group's research.

Thank you for your time and consideration.

Best regards,
[Full Name]
[Department, University]
[Email] | [Phone]
```

### Template 3: Professional Technical Inquiry

```
Subject: Technical Inquiry – [Product/Topic] for [Application]

Dear [Name / Technical Support Team],

I am [Name], a [position] at [Organization/University]. I am
currently working on [project/application] and am writing to
request technical information regarding [specific product or
topic].

Specifically, I would appreciate:
1. [Specific document/information needed]
2. [Specific document/information needed]
3. [Any additional requirements]

This information will be used for [purpose — e.g., "academic
research," "system design," "product evaluation"].

If there are any forms to complete or procedures to follow for
this request, please let me know.

Thank you for your assistance.

Best regards,
[Full Name]
[Title/Position]
[Organization]
[Email] | [Phone]
```

---

# END OF PART 2

## Summary of Part 2: Writing and Academic Communication

| Week | Topic | Key Skills Developed |
|------|-------|---------------------|
| 5 | Technical Writing Fundamentals | Sentence clarity, paragraph structure, cohesion, scientific style, AI writing tool boundaries |
| 6 | Paraphrasing, Summarizing, Academic Integrity | Paraphrasing techniques, IEEE citation, plagiarism avoidance, ethical AI paraphrasing |
| 7 | Abstracts, Introductions, Conclusions | Academic paper sections, useful phrases, structure, academic integrity in the AI era |
| 8 | CV and Cover Letter | Professional document preparation, self-presentation, responsible AI use in writing |
| 9 | Email Writing | Academic and professional communication, email etiquette, AI tools for professional communication |

---

## Recommended Resources

1. Swales, J.M. & Feak, C.B. (2012). *Academic Writing for Graduate Students*. University of Michigan Press.
2. Glasman-Deal, H. (2010). *Science Research Writing for Non-Native Speakers of English*. Imperial College Press.
3. IEEE Author Center: https://ieeeauthorcenter.ieee.org/
4. Purdue OWL – IEEE Citation Style: https://owl.purdue.edu/owl/research_and_citation/ieee_style.html
5. Grammarly (grammar checking tool): https://www.grammarly.com/
6. IEEE Thesaurus (for keywords): https://www.ieee.org/publications/services/thesaurus.html

---

*Part 2 of 4 — Scientific and Technical English for Electrical Engineering*  
*Next: Part 3 — Oral Communication and Presentations (Weeks 10–13)*
