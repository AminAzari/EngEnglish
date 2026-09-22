# Part 8: Prompt Engineering for Scientific and Technical English

## مهندسی پرامپت برای انگلیسی علمی و فنی

---

> **Module Overview:** This module treats prompt engineering as what it truly is — a **communication skill**. Just as writing a clear lab report, a precise specification, or an effective research abstract requires structured thinking and careful language use, so does writing prompts for Large Language Models. If you can write a good technical document, you can write a good prompt. If you cannot write a good prompt, it likely means your thinking or communication needs refinement.

> **Prerequisites:** Parts 1–7 of this course (especially: research skills, academic writing conventions, presentation skills, and the introduction to LLMs in Part 7).

> **Learning Outcomes:** By the end of this module, you will be able to:
> - Explain why prompt engineering is a language and communication skill
> - Write structured, precise prompts for research, writing, learning, and presentation tasks
> - Apply iterative refinement techniques to improve AI outputs
> - Use advanced prompting strategies (chain-of-thought, few-shot, meta-prompting)
> - Build a personal prompt library for your academic and professional work
> - Critically evaluate AI-generated content for accuracy and appropriateness

---

## 1. Prompt Engineering as a Communication Skill

### 1.1 Why Prompt Engineering Belongs in a Language Course

Consider these two scenarios:

| Scenario A: Writing to a Human | Scenario B: Writing to an AI |
|---|---|
| You write an email to your supervisor asking for feedback on your thesis draft. | You write a prompt asking an AI to review your thesis draft. |
| You must be clear about *what* you want reviewed, *how* detailed the feedback should be, and *what aspects* matter most. | You must be clear about *what* you want reviewed, *how* detailed the feedback should be, and *what aspects* matter most. |
| Vague request → vague feedback | Vague prompt → vague output |

The skills are **identical**. In both cases, you are:
- Formulating your needs precisely
- Providing relevant context
- Specifying the desired output format
- Anticipating what your reader needs to know

**Prompt engineering is technical communication with a non-human audience.**

### 1.2 The Parallel: Prompts ≈ Specifications

In electrical engineering, you write specifications constantly:

- **Design specifications** for a circuit (input voltage range, output impedance, bandwidth requirements)
- **Requirements documents** for embedded systems (timing constraints, memory limits, interface protocols)
- **Test plans** that define exactly what to measure and how

A well-written prompt follows the same logic as a well-written specification:

| Specification Element | Prompt Equivalent | Example |
|---|---|---|
| System requirements | Context/background | "I am designing a buck converter for a 48V-to-12V application..." |
| Functional requirements | Task specification | "Calculate the inductor value needed to maintain continuous conduction mode..." |
| Performance criteria | Quality constraints | "Show all steps, use standard notation, and verify the result." |
| Interface definitions | Format requirements | "Present the answer as a numbered list with equations in LaTeX format." |
| Acceptance criteria | Success indicators | "The explanation should be understandable to a 3rd-year EE student." |

### 1.3 Clear Thinking → Clear Writing → Clear Prompting

This is the fundamental chain that connects all communication:

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  CLEAR THINKING │ ──→ │  CLEAR WRITING  │ ──→ │ CLEAR PROMPTING │
│                 │     │                 │     │                 │
│ • Know what you │     │ • Structured    │     │ • Specific task │
│   want to learn │     │   paragraphs    │     │ • Defined scope │
│ • Define the    │     │ • Precise terms │     │ • Clear format  │
│   problem       │     │ • Logical flow  │     │ • Constraints   │
│ • Know what you │     │ • Reader        │     │ • Context given │
│   don't know    │     │   awareness     │     │                 │
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

> **Key Insight (نکته کلیدی):** If you cannot write a clear prompt, it often means you have not clearly defined what you actually need. The act of writing a good prompt forces you to clarify your own thinking — just like writing a good research question forces you to understand what you're investigating.

### 1.4 Audience Awareness: The LLM as Your Reader

In Parts 2 and 5 of this course, we discussed **audience awareness** — adapting your writing to your reader's knowledge, expectations, and needs. When prompting an AI, you must understand your "reader":

**What the LLM knows:**
- General knowledge across many domains
- Common patterns, conventions, and formats
- Multiple languages and technical vocabularies

**What the LLM does NOT know:**
- Your specific project details (unless you provide them)
- Your level of expertise (unless you state it)
- What you have already tried
- Your university's specific formatting requirements
- Current events or very recent publications

**What the LLM needs from you:**
- Context that it cannot infer
- Clear boundaries on scope
- Explicit format preferences
- Correction when it misunderstands

> **Analogy (قیاس):** Think of the LLM as a highly knowledgeable colleague who has just joined your lab. They know electrical engineering deeply, but they know nothing about your specific project, your supervisor's preferences, or what you discussed in last week's meeting. You must brief them every time.

---

## 2. Fundamentals of Effective Prompting

### 2.1 The Anatomy of a Good Prompt

Every effective prompt contains some or all of these components:

```
┌──────────────────────────────────────────────────────────────┐
│                    ANATOMY OF A PROMPT                        │
├──────────────────────────────────────────────────────────────┤
│ 1. ROLE/PERSONA    │ Who should the AI "be"?                 │
│ 2. CONTEXT         │ What background does the AI need?       │
│ 3. TASK            │ What exactly should the AI do?          │
│ 4. FORMAT          │ How should the output look?             │
│ 5. CONSTRAINTS     │ What are the boundaries/limitations?    │
│ 6. EXAMPLES        │ What does good output look like?        │
└──────────────────────────────────────────────────────────────┘
```

Let's examine each component with EE examples:

#### Component 1: Role/Persona Assignment (تعیین نقش)

Assigning a role tells the AI what perspective and expertise level to adopt.

| Bad Prompt ❌ | Good Prompt ✅ |
|---|---|
| "Explain PID controllers." | "You are an experienced control systems professor teaching a 3rd-year EE undergraduate course. Explain PID controllers with emphasis on practical tuning methods used in industrial motor control." |

**Why it works:** The role establishes the tone (educational), depth (undergraduate level), and focus (practical, industrial).

**Common roles for EE students:**
- "You are a senior power systems engineer reviewing my analysis..."
- "You are an IEEE journal reviewer providing constructive feedback..."
- "You are a patient tutor explaining signal processing concepts..."
- "You are a technical writer helping me improve my paper's clarity..."

#### Component 2: Context/Background (زمینه و پیش‌زمینه)

Context gives the AI information it cannot infer. Include:
- Your current knowledge level
- The project or course this relates to
- Previous work or attempts
- Specific constraints of your situation

**Example:**

```
CONTEXT: I am a 4th-year electrical engineering student writing my 
bachelor's thesis on "Optimal Placement of Distributed Generation in 
Radial Distribution Networks." I have completed the load flow analysis 
using Newton-Raphson method and now need to formulate the optimization 
problem. My supervisor wants me to use a genetic algorithm approach. 
I am familiar with basic optimization concepts but have not implemented 
metaheuristic algorithms before.
```

#### Component 3: Task Specification (مشخصات وظیفه)

The task must be **specific, actionable, and unambiguous** — the same principles as writing a good research objective.

| Vague Task ❌ | Specific Task ✅ |
|---|---|
| "Help me with my thesis." | "Write an outline for Chapter 3 (Methodology) of my thesis, covering: problem formulation, objective function definition, constraint specification, and GA implementation steps." |
| "Explain filters." | "Compare Butterworth and Chebyshev Type I low-pass filters in terms of: passband ripple, roll-off rate, phase response, and typical applications in audio signal processing." |
| "Fix my code." | "Debug this MATLAB code for DFT computation. The output magnitude spectrum shows unexpected symmetry errors for the test signal x(t) = 3sin(2π·100t) + sin(2π·250t) sampled at 1 kHz." |

#### Component 4: Format Requirements (الزامات قالب‌بندی)

Specifying format prevents the AI from choosing a format that doesn't serve your needs.

**Useful format specifications:**
- "Present as a numbered list with max 2 sentences per point"
- "Use a comparison table with columns for: Method, Advantages, Disadvantages, Complexity"
- "Write in paragraph form suitable for a journal paper's methodology section"
- "Format equations using LaTeX notation"
- "Use bullet points for the summary, then detailed explanations below"
- "Limit your response to 200 words"

#### Component 5: Constraints and Boundaries (محدودیت‌ها و مرزها)

Constraints prevent the AI from going off-track. Think of them as the "do NOT" instructions:

**Examples:**
- "Do not use concepts beyond undergraduate-level electromagnetics"
- "Focus only on analog implementations, not digital"
- "Keep the explanation under 300 words"
- "Do not include code — explain the algorithm in pseudocode only"
- "Use only sources that would be found in IEEE Xplore or Scopus"
- "Assume ideal op-amp conditions for this analysis"

#### Component 6: Examples / Few-Shot Prompting (ارائه نمونه)

Providing examples of desired output is one of the most powerful techniques. It shows rather than tells.

**Example — Generating paper summaries:**

```
I want you to summarize research papers in the following format:

EXAMPLE:
Paper: "A Novel MPPT Algorithm for Partially Shaded PV Arrays"
Summary:
- Problem: Conventional MPPT fails under partial shading (multiple local maxima)
- Method: Modified P&O with periodic global scan every 30 seconds
- Key Result: 12% improvement in energy yield under dynamic shading
- Limitation: Increased computational load on microcontroller
- Relevance to my work: [I would fill this in]

Now summarize this paper using the same format: [paste abstract/paper]
```

### 2.2 Zero-Shot vs. Few-Shot vs. Chain-of-Thought

These are the three fundamental prompting strategies:

| Strategy | Description | When to Use | EE Example |
|---|---|---|---|
| **Zero-shot** | Ask directly, no examples | Simple, well-defined tasks | "What is the skin effect in conductors?" |
| **Few-shot** | Provide 1-3 examples first | When you need a specific format or style | Show 2 example circuit analyses, then ask for a 3rd |
| **Chain-of-thought (CoT)** | Ask AI to reason step by step | Complex calculations, multi-step problems | "Solve this Thevenin equivalent step by step, showing all intermediate calculations" |

#### Zero-Shot Example (بدون نمونه):
```
What are the main differences between NMOS and PMOS transistors 
in terms of mobility, threshold voltage, and typical applications 
in CMOS design?
```

#### Few-Shot Example (با نمونه):
```
Convert these informal descriptions into formal research objectives:

Example 1:
Informal: "I want to make the antenna work better at 5G frequencies"
Formal: "To optimize the radiation pattern and gain of a microstrip 
patch antenna for operation in the 24-28 GHz 5G frequency band."

Example 2:
Informal: "I need to reduce noise in my amplifier circuit"
Formal: "To minimize the noise figure of a two-stage low-noise 
amplifier (LNA) operating in the 1-6 GHz range through optimal 
transistor biasing and impedance matching."

Now convert this:
Informal: "I want to make the solar panel system track the sun better"
```

#### Chain-of-Thought Example (زنجیره تفکر):
```
Analyze this RLC series circuit step by step:
Given: R = 100Ω, L = 10mH, C = 1μF, Vs = 10V peak at 5kHz

Step 1: Calculate individual impedances (XL, XC)
Step 2: Calculate total impedance (Z)
Step 3: Find the current magnitude and phase
Step 4: Determine if the circuit is inductive or capacitive
Step 5: Calculate power factor
Step 6: Determine the resonant frequency and compare to 5kHz

Show all calculations with units.
```

### 2.3 The Importance of Specificity and Precision

This connects directly to what you learned in Parts 2 and 3 about **technical writing precision**:

| Technical Writing Principle | Prompting Application |
|---|---|
| Avoid vague quantifiers ("some," "many") | Specify exact numbers: "List 5 advantages" not "List some advantages" |
| Define abbreviations on first use | Provide full context: "OFDM (Orthogonal Frequency-Division Multiplexing) as used in 5G NR" |
| Use precise technical vocabulary | Use correct terminology: "transient response" not "how the circuit behaves at the start" |
| State assumptions explicitly | Tell the AI what to assume: "Assume ideal diode model" |
| Quantify where possible | Set bounds: "between 1 and 10 GHz," "for a 3-phase, 400V system" |

### 2.4 Common Prompting Mistakes

| Mistake | Example | Problem | Fix |
|---|---|---|---|
| **Too vague** | "Tell me about power systems" | No focus, no boundaries | "Explain the difference between symmetrical and asymmetrical faults in three-phase power systems, with phasor diagrams" |
| **Too broad** | "Explain everything about MIMO" | Overwhelming scope | "Explain spatial multiplexing in 2x2 MIMO, focusing on how it doubles throughput" |
| **Ambiguous task** | "Help me with this circuit" | Help how? Analyze? Design? Debug? | "Analyze this common-emitter amplifier for voltage gain, input impedance, and bandwidth" |
| **No context** | "Is this abstract good?" | Good for what? What field? | "Review this abstract for an IEEE conference paper on power electronics. Check for: clarity, structure, and adherence to the IMRaD format" |
| **Information overload** | [Pastes entire 20-page paper] "Summarize" | Too much, no focus | Paste only the abstract + conclusion, specify what aspects to summarize |
| **Leading/biased** | "Explain why solar power is better than wind" | Assumes a conclusion | "Compare the advantages and disadvantages of solar PV and wind generation for a 10kW residential installation in Tehran" |



---

## 3. Prompt Patterns for Research Tasks

Research is at the heart of your academic journey. These prompt patterns will help you use AI effectively throughout the research process — from finding sources to understanding them to identifying gaps.

### 3.1 Generating Keywords for Literature Search

**The Problem:** You have a research idea but struggle to find the right search terms for IEEE Xplore, Scopus, or Google Scholar.

**Pattern:**
```
I am researching [topic description in plain language]. 

My specific focus is on [narrower aspect]. 

Generate a comprehensive list of search keywords and phrases I should 
use to find relevant papers in IEEE Xplore and Scopus. Include:
1. Primary keywords (direct terms)
2. Synonyms and alternative terms
3. Related broader terms
4. Related narrower/specific terms
5. Suggested Boolean search strings combining these terms

Field: Electrical Engineering / [sub-field]
```

**Concrete Example:**

```
I am researching how to detect faults in solar panel systems 
using machine learning.

My specific focus is on identifying hot spots and degradation 
in large-scale PV farms using thermal imaging data.

Generate a comprehensive list of search keywords and phrases I 
should use to find relevant papers in IEEE Xplore and Scopus. Include:
1. Primary keywords (direct terms)
2. Synonyms and alternative terms  
3. Related broader terms
4. Related narrower/specific terms
5. Suggested Boolean search strings combining these terms

Field: Electrical Engineering / Renewable Energy Systems
```

**Expected output includes terms like:**
- Primary: "fault detection," "photovoltaic," "thermal imaging," "machine learning"
- Synonyms: "anomaly detection," "solar array," "infrared thermography," "deep learning"
- Broader: "condition monitoring," "predictive maintenance," "renewable energy"
- Narrower: "hot spot detection," "bypass diode failure," "CNN classification," "PV degradation rate"
- Boolean: `("fault detection" OR "anomaly detection") AND ("photovoltaic" OR "solar") AND ("thermal imag*" OR "infrared") AND ("machine learning" OR "deep learning" OR "CNN")`

### 3.2 Understanding Complex Papers

**Pattern for Targeted Explanation:**
```
I am a [year] electrical engineering student. I understand 
[concepts you know] but I am not familiar with [concepts you 
don't know].

Here is the abstract of a paper I need to understand:
[paste abstract]

Please:
1. Explain the main contribution in 2-3 simple sentences
2. Identify the key technical terms I might not know and define them
3. Explain the methodology at a high level
4. Tell me what background I need to fully understand this paper
```

**Concrete Example:**
```
I am a 3rd-year electrical engineering student. I understand 
basic digital signal processing (DFT, FIR/IIR filters, sampling 
theorem) but I am not familiar with compressed sensing or sparse 
signal recovery.

Here is the abstract of a paper I need to understand:
"This paper proposes a novel compressed sensing framework for 
sub-Nyquist sampling of wideband spectrum in cognitive radio 
networks. By exploiting the inherent sparsity of spectrum 
occupancy, we design a measurement matrix based on random 
demodulation that achieves 70% reduction in sampling rate while 
maintaining detection probability above 95%. The recovery 
algorithm combines OMP with a spectral prior learned from 
historical occupancy data..."

Please:
1. Explain the main contribution in 2-3 simple sentences
2. Identify the key technical terms I might not know and define them
3. Explain the methodology at a high level
4. Tell me what background I need to fully understand this paper
```

### 3.3 Summarizing Papers at Different Levels

**Pattern — Multi-Level Summary:**
```
Summarize the following paper content at three levels:

Level 1 - Tweet (280 characters): What's the one-sentence takeaway?
Level 2 - Elevator Pitch (100 words): What did they do, why, and 
what did they find?
Level 3 - Detailed Summary (300 words): Problem, method, key results, 
limitations, and significance.

Paper content: [paste abstract and conclusion]
```

**Pattern — Summary for Specific Purpose:**
```
I am writing a literature review section for my thesis on 
[your topic]. Summarize this paper focusing specifically on:
- What methodology they used (I need to compare methods)
- What dataset/test system they used
- Their reported accuracy/performance metrics
- Limitations they acknowledge

Paper: [paste relevant sections]
```

### 3.4 Identifying Research Gaps

**Pattern:**
```
I have read these 5 papers on [topic]. Here are their key 
contributions:

Paper 1: [1-2 sentence summary of contribution]
Paper 2: [1-2 sentence summary of contribution]
Paper 3: [1-2 sentence summary of contribution]
Paper 4: [1-2 sentence summary of contribution]
Paper 5: [1-2 sentence summary of contribution]

Based on these existing works, identify:
1. What aspects of [topic] remain unexplored?
2. What limitations do these papers share?
3. What combinations of approaches haven't been tried?
4. What practical/real-world challenges aren't addressed?
5. Suggest 3 potential research questions that would fill these gaps.

Note: I need these for a bachelor's thesis, so they should be 
achievable in 6 months with [available resources].
```

**Concrete Example:**
```
I have read these 5 papers on fault detection in induction motors:

Paper 1: Uses vibration analysis + SVM to detect bearing faults (98% accuracy on CWRU dataset)
Paper 2: Uses stator current signature analysis + FFT for broken rotor bars
Paper 3: Applies CNN to thermal images for overall fault classification
Paper 4: Combines vibration + current data using sensor fusion (random forest)
Paper 5: Uses transfer learning from lab data to real industrial motors

Based on these existing works, identify:
1. What aspects of motor fault detection remain unexplored?
2. What limitations do these papers share?
3. What combinations of approaches haven't been tried?
4. What practical/real-world challenges aren't addressed?
5. Suggest 3 potential research questions that would fill these gaps.

Note: I need these for a bachelor's thesis, so they should be 
achievable in 6 months with access to a university lab, a few 
induction motors, and standard sensors (accelerometer, current probe).
```

### 3.5 Comparing Methodologies Across Papers

**Pattern:**
```
I need to create a comparison table for my literature review. 
Compare the following approaches to [problem]:

Approach A: [name] - used in [Paper X]
Approach B: [name] - used in [Paper Y]  
Approach C: [name] - used in [Paper Z]

Compare them using these criteria:
- Computational complexity
- Accuracy/performance
- Required training data
- Real-time capability
- Hardware requirements
- Scalability
- Ease of implementation for a bachelor's thesis

Present as a table, then write a 150-word paragraph summarizing 
which approach is most suitable for [your specific constraints].
```

### 3.6 Finding Connections Between Papers

**Pattern:**
```
I am trying to connect ideas from two different sub-fields 
for my research:

Field A: [description + key papers/concepts]
Field B: [description + key papers/concepts]

My hypothesis is that [technique from A] could be applied to 
[problem from B] because [your reasoning].

Please:
1. Evaluate whether this connection is reasonable
2. Identify what technical challenges would arise
3. Suggest what search terms I should use to find if anyone 
   has already explored this intersection
4. Recommend what background knowledge I need from both fields
```

---

## 4. Prompt Patterns for Writing Assistance

### 4.1 Improving Grammar and Style

**Pattern — Technical Grammar Check:**
```
Review the following paragraph from my [paper type] for:
1. Grammar errors (especially articles, prepositions, and tense consistency)
2. Passive/active voice balance (academic writing needs both)
3. Sentence length variety
4. Technical term consistency (flag if I use different terms for the same concept)
5. Hedging language appropriateness (for claims vs. established facts)

Do NOT change the technical content. Only improve the language.
Mark each change with [CHANGE: reason].

Paragraph:
[your text]
```

**Concrete Before/After Example:**

Before (student's draft):
```
"The system was tested and results show that the proposed method 
is working better than conventional methods. We can see from 
Table 2 that accuracy is high. The method is good for real-time 
applications because it is fast."
```

Prompt:
```
Rewrite this paragraph for an IEEE journal paper. Maintain the 
same meaning but improve: precision of claims, academic tone, 
specificity (replace vague terms with measurable statements), 
and sentence variety. Keep it concise.

"The system was tested and results show that the proposed method 
is working better than conventional methods. We can see from 
Table 2 that accuracy is high. The method is good for real-time 
applications because it is fast."
```

After (AI-improved):
```
"The proposed method was evaluated against three conventional 
approaches under identical test conditions. As shown in Table 2, 
it achieves a classification accuracy of 96.3%, representing a 
4.7% improvement over the best-performing baseline (k-NN with 
hand-crafted features). With a processing latency of 12 ms per 
frame, the method satisfies real-time constraints for applications 
requiring sub-50 ms response times."
```

### 4.2 Paraphrasing While Maintaining Technical Accuracy

**Pattern:**
```
Paraphrase the following text for my [document type]. Requirements:
- Maintain ALL technical accuracy — do not simplify or change the meaning
- Change the sentence structure and word choice significantly
- Keep the same level of formality
- Maintain all numerical values and specific claims
- Do not add information that isn't in the original
- Flag any terms that should NOT be paraphrased (standard terminology)

Original: [text from source]
Context: This is for my [section] where I am discussing [topic].
```

### 4.3 Writing Abstracts (Iterative Refinement)

Writing an abstract is an iterative process. Use this multi-step approach:

**Step 1 — Generate initial draft:**
```
Write a 250-word abstract for my research paper based on this information:
- Topic: [your topic]
- Problem addressed: [what gap/problem]
- Method used: [your methodology]
- Key results: [main findings with numbers]
- Main conclusion: [what does this mean]

Follow the standard structure: Background → Problem → Method → Results → Conclusion
Write for an IEEE [specific conference/journal] audience.
```

**Step 2 — Refine:**
```
Here is my current abstract draft:
[paste draft]

Please improve it by:
1. Making the opening sentence more engaging (start with the problem's significance)
2. Reducing wordiness — target exactly 200 words
3. Ensuring every sentence adds new information (no redundancy)
4. Strengthening the concluding sentence to emphasize novelty
5. Check that all claims are supported by the specific numbers I mentioned
```

**Step 3 — Final polish:**
```
Compare my abstract against these IEEE abstract conventions:
- Does it avoid "In this paper, we..." as the opening?
- Does it quantify the improvement over state-of-the-art?
- Does it mention the specific application domain?
- Are there any first-person pronouns that should be removed?
- Is it within 150-250 words?

Suggest final edits only. Do not rewrite the entire abstract.
```

### 4.4 Generating Outlines for Papers/Reports

**Pattern:**
```
Generate a detailed outline for a [document type] on [topic].

Requirements:
- Follow [IEEE/university/specific] formatting guidelines
- Target length: [number] pages
- My research contribution is: [specific contribution]
- Include suggested subsection headings
- For each section, write 1 sentence describing what content goes there
- Suggest approximate page allocation per section

The paper should emphasize: [methodological novelty / application / comparison / theoretical contribution]
```

### 4.5 Getting Feedback on Argument Structure

**Pattern:**
```
I am writing the Discussion section of my paper. Here is my argument structure:

1. [First claim]
   Evidence: [what supports it]
2. [Second claim]
   Evidence: [what supports it]
3. [My conclusion/interpretation]

Please evaluate:
- Is the logical flow clear? Would a reader follow my reasoning?
- Are there any logical gaps or unsupported jumps?
- Where should I add hedging language (might, could, suggests) vs. confident claims?
- What counterarguments should I address?
- Does the argument build toward the conclusion effectively?
```

### 4.6 Translation Assistance (Persian Technical → English Academic)

**Pattern:**
```
Translate the following Persian technical text into academic English 
suitable for an IEEE journal paper:

[Persian text]

Requirements:
- Use standard IEEE terminology (not literal translations)
- Maintain formal academic register
- Keep all equations and variable names as they are
- If a Persian technical term has a specific established English 
  equivalent in EE, use that term (not a literal translation)
- Flag any sentences where the meaning is ambiguous and you had 
  to make an interpretation choice

After translation, list any Persian terms that you were unsure about.
```

### 4.7 Email Drafting and Refinement

**Pattern:**
```
Write a professional academic email for this situation:

To: [role/relationship - e.g., "my thesis supervisor," "a professor 
I want to collaborate with," "conference organizers"]
Purpose: [what you need]
Context: [relevant background]
Tone: [formal/semi-formal, how well you know them]
My English level: B2 — please use clear, natural academic English 
that isn't overly complex but is fully professional.

Constraints:
- Keep it under [X] sentences
- Include: [specific things to mention]
- Avoid: [cultural considerations]
```

**Example:**
```
Write a professional academic email for this situation:

To: A professor at TU Munich whose paper on GaN power converters 
I read. I have never contacted them before.
Purpose: Ask if they have any PhD positions available, mention 
that my BSc thesis is related to their work.
Context: I am finishing my BSc at University of Tehran. My thesis 
is on "High-frequency GaN-based DC-DC converters for EV battery 
charging." I have one published conference paper.
Tone: Formal, respectful, concise.

Constraints:
- Keep it under 10 sentences
- Include: specific mention of their paper that I found relevant
- Avoid: being too humble or apologetic (common L1 Persian transfer)
```

### 4.8 CV Bullet Point Improvement

**Pattern:**
```
Improve these CV bullet points for an [application type: PhD application / 
internship / job]. Make them:
- Start with strong action verbs
- Quantify achievements where possible
- Highlight technical skills relevant to [target position/field]
- Be concise (max 1.5 lines each)
- Use the PAR format (Problem/Action/Result) where appropriate

Current bullets:
- [your bullet 1]
- [your bullet 2]
- [your bullet 3]

Context: I am applying for [position] at [type of organization].
My strengths are in [areas].
```



---

## 5. Prompt Patterns for Learning and Comprehension

### 5.1 "Explain Like I'm..." Patterns for EE Concepts

The key is to specify your **exact** current knowledge level, not just "explain simply."

**Pattern:**
```
Explain [concept] to me. Here is what I already know and what I don't:

I KNOW:
- [concept A that I'm comfortable with]
- [concept B that I can use]
- [relevant math I understand]

I DON'T KNOW:
- [specific gap]
- [related concept I haven't studied yet]

Explain [target concept] by building on what I already know. 
Use analogies to [domain I'm familiar with] if helpful.
Do not use [advanced concept] in your explanation.
```

**Concrete Example:**
```
Explain the Smith Chart to me. Here is what I already know and what I don't:

I KNOW:
- Complex impedance (R + jX)
- Reflection coefficient (Γ) and its relationship to impedance mismatch
- Transmission line theory basics (characteristic impedance Z₀)
- How to plot points on a complex plane

I DON'T KNOW:
- Why circles represent constant resistance/reactance
- How to use the chart for impedance matching
- The relationship between Smith Chart regions and circuit behavior

Explain the Smith Chart by building on my knowledge of the complex Γ plane.
Start with WHY it's structured as circles, then show me how to read it.
Use a 50Ω system with a load of 100+j50 Ω as a worked example.
```

### 5.2 Socratic Prompting: Asking AI to Quiz You

**Pattern — Exam Preparation:**
```
Quiz me on [topic] at the level of a [course/exam] exam.

Rules:
- Ask me ONE question at a time
- Wait for my answer before asking the next
- After I answer, tell me if I'm correct and explain any errors
- Mix question types: conceptual, calculation, and application
- Start easier and get progressively harder
- If I get something wrong, ask a follow-up question that helps 
  me understand my mistake
- After 10 questions, give me a summary of my strengths and weaknesses

Topics to cover:
- [subtopic 1]
- [subtopic 2]
- [subtopic 3]

My level: [year of study, what I've covered so far]
```

**Concrete Example:**
```
Quiz me on digital communications at the level of a final exam 
for a 3rd-year undergraduate course.

Rules:
- Ask me ONE question at a time
- Wait for my answer before asking the next
- After I answer, tell me if I'm correct and explain any errors
- Mix question types: conceptual, calculation, and application
- Start easier and get progressively harder
- After 10 questions, summarize my strengths and weaknesses

Topics to cover:
- Baseband modulation (ASK, FSK, PSK)
- Bit error rate calculations
- Nyquist criterion for ISI-free transmission  
- Matched filter and correlator receiver
- Channel capacity (Shannon limit)

My level: I have completed the lectures but haven't practiced 
many calculations yet.
```

### 5.3 Creating Study Materials from Lecture Notes

**Pattern:**
```
I have the following lecture notes on [topic]. Create study materials:

[Paste key points/equations/concepts from your notes]

Please create:
1. A concept map showing how these ideas connect to each other
   (describe it textually with relationships)
2. A "cheat sheet" summary — the essential formulas and 
   definitions in a compact format
3. 5 potential exam questions (with brief answers)
4. A list of "things students often confuse" for this topic
5. 3 real-world EE applications of each concept

Format: Use clear headers and bullet points. Keep it concise 
enough to review in 30 minutes.
```

### 5.4 Generating Practice Problems

**Pattern:**
```
Generate [number] practice problems on [topic] for me.

Requirements:
- Difficulty: [easy/medium/hard/mixed]
- Type: [calculation / conceptual / design / debugging]
- Each problem should test a DIFFERENT aspect of the topic
- Include the answer separately (I want to attempt them first)
- Use realistic component values and practical scenarios
- If calculation is involved, specify all necessary parameters

Topic specifics: [any particular subtopics or types you want to practice]

Format: 
- Problem statement
- Given information
- What to find
- [ANSWER section separated by a line]
```

**Concrete Example:**
```
Generate 5 practice problems on operational amplifier circuits for me.

Requirements:
- Difficulty: medium (3rd-year undergraduate level)
- Type: mix of analysis and design
- Each problem should test a different op-amp configuration
- Include answers separately
- Use realistic resistor values (E12 series preferred)

Topics to cover:
1. Inverting amplifier with multiple inputs (summing)
2. Non-inverting amplifier gain and input impedance
3. Differential amplifier CMRR calculation
4. Integrator circuit with practical DC bias considerations
5. Active filter design (2nd order Sallen-Key)

Format each as: Problem → Given → Find → [Answer below separator]
```

### 5.5 Understanding Equations Step by Step

**Pattern:**
```
Explain this equation to me step by step:

[equation]

For each term/symbol:
1. What does it physically represent?
2. What are its units?
3. What happens to the result if this term increases/decreases?

Then:
- Derive it from [starting point I know] if possible
- Show me a numerical example with realistic EE values
- Tell me when/where this equation is used in practice
- What assumptions does this equation make?
- What are its limitations (when does it break down)?
```

**Concrete Example:**
```
Explain this equation to me step by step:

P_loss = I²R_DS(on) · D + ½V_DS · I · (t_on + t_off) · f_sw

Context: This is for MOSFET power losses in a switching converter.

For each term:
1. What does it physically represent?
2. What are its units?
3. What happens if this term increases?

Then:
- Show a numerical example for a buck converter operating at 
  100kHz, 10A load, using an IRF540N MOSFET
- At what switching frequency do switching losses dominate 
  conduction losses for this example?
- How does this equation change for soft-switching topologies?
```

---

## 6. Prompt Patterns for Presentations

### 6.1 Generating Presentation Outlines from Paper Content

**Pattern:**
```
I need to present this paper in [time limit] minutes to [audience].

Paper information:
- Title: [title]
- Main contribution: [1-2 sentences]
- Method: [brief description]
- Key results: [main findings]

Create a presentation outline with:
- Suggested slide titles and sequence
- Key points per slide (max 3 bullet points each)
- Where to include figures/diagrams (describe what type)
- Time allocation per slide
- Suggested opening hook (first 30 seconds)
- Suggested closing statement

Constraints:
- Audience technical level: [beginner/intermediate/expert]
- They are familiar with: [concepts]
- They are NOT familiar with: [concepts]
- I should spend most time on: [methodology/results/implications]
```

**Concrete Example:**
```
I need to present this paper in 15 minutes to my EE classmates 
(senior undergraduate students).

Paper information:
- Title: "Deep Reinforcement Learning for Real-Time Energy 
  Management in Hybrid Electric Vehicles"
- Main contribution: Uses DRL instead of dynamic programming 
  for HEV energy management — achieves near-optimal fuel 
  economy without requiring a known drive cycle.
- Method: Proximal Policy Optimization (PPO) trained in simulation, 
  tested on real drive cycles
- Key results: Within 2% of global optimum, 10x faster than DP, 
  works for unknown drive cycles

Create a presentation outline with slide titles, key points per slide,
suggested visuals, time allocation (15 min total), and opening hook.

Constraints:
- Audience knows: basic control theory, what EVs/HEVs are, general 
  idea of machine learning
- Audience does NOT know: reinforcement learning details, PPO algorithm,
  Bellman equations
- I should spend most time on: the concept of RL for control (not math details)
  and the results comparison
```

### 6.2 Creating Q&A Preparation Lists

**Pattern:**
```
I am presenting on [topic] to [audience]. Help me prepare for 
the Q&A session.

My presentation covers:
- [Main point 1]
- [Main point 2]
- [Main point 3]

Generate:
1. 10 likely questions the audience might ask (ranging from 
   basic clarification to challenging/critical questions)
2. For each question, suggest a concise answer (2-3 sentences)
3. Identify 3 "difficult questions" — questions that might 
   expose weaknesses in my work — and suggest honest, professional 
   responses
4. Suggest 2 questions where the best answer is "That's a great 
   point for future work" and how to phrase that gracefully

Audience context: [who they are, what they care about]
```

### 6.3 Getting Feedback on Slide Text

**Pattern:**
```
Review these slide bullet points for my technical presentation.
For each slide, tell me:
- Are there too many words? (Rule: max 6 words per bullet, max 6 bullets)
- Is the language clear and direct?
- Should anything be a figure/diagram instead of text?
- Are there any terms the audience might not know?
- Does the flow from this slide to the next make sense?

Slide 1: [title]
- [bullet]
- [bullet]

Slide 2: [title]
- [bullet]
- [bullet]

[etc.]

Audience: [who]
Purpose: [inform/persuade/teach]
```

### 6.4 Simplifying Complex Content for Different Audiences

**Pattern:**
```
I need to explain [complex EE concept] to [specific audience]. 
Help me find the right level of simplification.

The concept (technical version):
[your technical understanding]

Target audience: [e.g., "management team with business background," 
"first-year EE students," "interdisciplinary research group"]

What they likely know: [their background]
What they care about: [their interests/concerns]

Please:
1. Identify what to keep and what to abstract away
2. Suggest an analogy they would understand
3. Write a 3-sentence explanation at their level
4. Suggest one simple visual that would help
5. Identify the ONE number/result I should emphasize
```

### 6.5 Generating Analogies for Technical Concepts

**Pattern:**
```
Generate 3 different analogies to explain [EE concept] to [audience].

The concept involves: [brief technical description]
Key aspects that the analogy must capture:
- [important property 1]
- [important property 2]
- [relationship/behavior to illustrate]

For each analogy:
- Describe the analogy
- Explain which aspects it captures well
- Note where the analogy breaks down (so I don't over-extend it)
- Rate its accessibility for [audience] on a 1-5 scale
```

**Concrete Example:**
```
Generate 3 different analogies to explain impedance matching 
to first-year EE students who haven't taken electromagnetics yet.

The concept involves: Maximum power transfer occurs when source 
and load impedances are conjugate matched.

Key aspects that the analogy must capture:
- The idea of "matching" two things for optimal transfer
- That mismatch causes energy to be reflected/wasted
- That it depends on frequency

For each analogy:
- Describe it clearly
- What aspects it captures well
- Where it breaks down
- Accessibility rating for first-year students (1-5)
```



---

## 7. Advanced Techniques

### 7.1 Chain-of-Thought Prompting for Complex Reasoning

Chain-of-thought (CoT) prompting asks the AI to show its reasoning process. This is particularly valuable for:
- Multi-step calculations
- Design decisions with tradeoffs
- Debugging complex systems
- Understanding cause-and-effect chains

**Basic CoT Trigger Phrases:**
- "Think step by step"
- "Show your reasoning at each stage"
- "Before giving the final answer, work through the problem systematically"
- "Explain your thought process"

**Structured CoT Pattern for EE Problems:**
```
Solve this problem using a structured step-by-step approach:

[Problem statement]

For each step:
1. State what you're trying to find
2. State what equation/principle you're using and WHY
3. Show the calculation
4. Verify the result makes physical sense (correct units, 
   reasonable magnitude, expected behavior)
5. State any assumptions you're making

After solving, provide:
- A sanity check (does this answer make physical sense?)
- What would change if [parameter] were different?
```

**Concrete Example — Power System Fault Analysis:**
```
Analyze a three-phase symmetrical fault at Bus 3 in the following system. 
Use structured step-by-step reasoning.

Given:
- Generator at Bus 1: 100 MVA, X"d = 0.15 pu
- Transformer T1 (Bus 1 to Bus 2): 100 MVA, X = 0.10 pu
- Transmission line (Bus 2 to Bus 3): X = 0.20 pu
- Base: 100 MVA, 220 kV at Bus 2

For each step:
1. State what you're calculating and why
2. Show the per-unit equivalent circuit at that stage
3. Perform the calculation with units
4. Verify physical reasonableness

Find: Fault current magnitude at Bus 3 (in pu and kA)
```

### 7.2 System Prompts and Persistent Instructions

A **system prompt** is an instruction that sets the overall behavior for an entire conversation. Think of it as a "configuration" for the AI that persists across multiple exchanges.

**Pattern — Setting Up a Research Assistant:**
```
SYSTEM INSTRUCTION (use at the start of a new conversation):

You are my research assistant for my bachelor's thesis on 
"[topic]." Throughout our conversation:

- Always assume I'm a senior EE undergrad (know basics, learning advanced)
- When I share text, assume it's from my thesis draft unless I say otherwise
- Prioritize IEEE style and formatting conventions
- When suggesting improvements, explain WHY (so I learn, not just copy)
- If I ask something that requires recent papers (after 2023), 
  remind me that you may not have that information
- Use the following notation conventions: [list your conventions]
- My thesis structure: [Ch1: Intro, Ch2: Lit Review, Ch3: Method, 
  Ch4: Results, Ch5: Conclusion]

Acknowledge these instructions, then wait for my first question.
```

**Pattern — Setting Up a Language Tutor:**
```
SYSTEM INSTRUCTION:

You are my technical English tutor. Your role throughout this conversation:

- Correct my grammar mistakes but ALSO explain the rule behind the correction
- Focus especially on: articles (a/the/ø), prepositions, and tense consistency
- When I write something that's grammatically correct but not natural academic 
  English, suggest a more natural phrasing
- Rate each text I submit: Grammar (1-5), Academic style (1-5), Clarity (1-5)
- Keep track of my recurring mistakes and remind me of them
- All examples should be from electrical engineering contexts

I am a Persian speaker (B2 level English), senior EE student.
My typical errors: article omission, literal Persian translation of 
prepositions, overuse of "very" and "so."
```

### 7.3 Iterative Refinement: Treating Prompting as a Conversation

Effective prompting is rarely one-shot. Just like writing a paper involves multiple drafts, working with AI should be an **iterative conversation**.

**The Iterative Refinement Cycle:**
```
┌───────────────┐
│ Initial Prompt│
└───────┬───────┘
        ▼
┌───────────────┐     ┌───────────────────────────────┐
│   AI Output   │────→│  Evaluate: Is this what I need?│
└───────────────┘     └───────────────┬───────────────┘
                                      │
                          ┌───────────┴───────────┐
                          │                       │
                     YES: Done              NO: Refine
                                                  │
                                                  ▼
                                    ┌─────────────────────────┐
                                    │  Specific feedback:      │
                                    │  "More X, less Y,        │
                                    │   change Z to W"         │
                                    └─────────────┬───────────┘
                                                  │
                                                  ▼
                                         [Back to AI Output]
```

**Refinement Prompt Phrases:**
- "Good, but make it more [specific/concise/formal/technical]"
- "Keep points 2 and 4, but redo points 1 and 3 with [specific change]"
- "The structure is right but the tone is too [informal/complex/vague]"
- "Add more detail about [specific aspect] and remove the section on [irrelevant part]"
- "That's too long. Condense to [N] words while keeping [important elements]"

**Example — Iterative Abstract Writing:**

**Round 1:** "Write an abstract for my paper on MPPT for partial shading"
→ AI produces a generic abstract

**Round 2:** "Too generic. Include these specific numbers: 98.2% tracking efficiency, 15% improvement over P&O, tested on 10-panel array, simulation + hardware validation"
→ Better, but still not quite right

**Round 3:** "Good structure. But: (1) First sentence should emphasize the PROBLEM not the solution. (2) Remove the phrase 'In this paper' — use active voice. (3) Add that the method requires no additional sensors."
→ Nearly there

**Round 4:** "Perfect content. Final tweaks: reduce from 280 to 240 words, and make the last sentence about future applicability to battery storage systems."
→ Done

### 7.4 Combining Multiple AI Tools in a Workflow

Modern research workflows can chain multiple AI-powered tools:

**Example Research Workflow:**
```
1. Use AI to generate search keywords → 
2. Search IEEE Xplore (human step) → 
3. Use AI to summarize found papers → 
4. Use AI to identify research gaps → 
5. Human makes research decisions → 
6. Use AI to help structure methodology chapter → 
7. Human writes content → 
8. Use AI for grammar/style checking → 
9. Human reviews and finalizes
```

**Example Writing Workflow:**
```
1. Brain dump your ideas in Persian (or mixed Persian-English)
2. Prompt: "Translate and organize these notes into an outline"
3. Prompt: "Expand section 3.2 of this outline into full paragraphs"
4. Prompt: "Check this text for grammar and academic style"
5. Prompt: "Does this paragraph logically connect to the previous one?"
6. Human review and revision
7. Prompt: "Final proofread — check for consistency in notation and terminology"
```

> **⚠️ Important Note:** AI assists at each step, but the **intellectual decisions** (what to research, what methodology to choose, what conclusions to draw) remain yours. AI is a language and organization tool — you are the researcher.

### 7.5 Prompt Templates: Reusable Prompts for Repeated Tasks

Create templates with [PLACEHOLDER] fields that you fill in each time:

**Template — Weekly Paper Summary:**
```
Summarize this paper for my literature review log:

Title: [PAPER_TITLE]
Authors: [AUTHORS]
Published: [JOURNAL/CONFERENCE, YEAR]

Abstract: [PASTE_ABSTRACT]

Provide:
1. One-sentence summary of main contribution
2. Methodology used (2-3 sentences)
3. Key quantitative results
4. Relevance to my thesis on [MY_THESIS_TOPIC]: High/Medium/Low + why
5. Potential citations for my: Introduction / Lit Review / Methodology / Discussion
6. Questions I should investigate further

Format: Structured notes I can paste into my research log.
```

**Template — Lab Report Introduction:**
```
Help me write the Introduction section for a lab report:

Experiment: [EXPERIMENT_NAME]
Course: [COURSE_NAME]
Objective: [WHAT_WE_MEASURED/TESTED]
Relevant theory: [KEY_EQUATIONS_OR_PRINCIPLES]
Expected outcome: [WHAT_THEORY_PREDICTS]

Write a 150-word introduction that:
- Starts with the general principle being tested
- Narrows to the specific experiment
- States the objective clearly
- Mentions the methodology briefly
- Uses present tense for established theory, past tense for what was done
```

### 7.6 Meta-Prompting: Asking AI to Help Write Better Prompts

When you're not getting good results, ask the AI to help you prompt better:

**Pattern:**
```
I'm trying to get an AI to [what you want to accomplish] but 
my prompts keep producing [problem with output].

Here's my current prompt:
"[your prompt]"

Help me improve this prompt. Specifically:
1. What information am I missing that the AI needs?
2. How can I make my instructions less ambiguous?
3. What constraints should I add?
4. Would examples (few-shot) help here?
5. Should I restructure the prompt differently?

Write me an improved version of this prompt.
```

**Concrete Example:**
```
I'm trying to get an AI to explain control system stability 
but it keeps giving me overly mathematical explanations that 
I can't follow, or overly simplified ones that don't help me 
solve homework problems.

Here's my current prompt:
"Explain stability in control systems at an intermediate level"

Help me improve this prompt to get explanations that are:
- Mathematical enough to connect to my homework
- But explained in plain language alongside the math
- Focused on Bode plot stability criteria specifically
- Include a worked example

Write me an improved version of this prompt.
```



---

## 8. Common Pitfalls and How to Avoid Them

### 8.1 Over-Trusting AI Output

> **⚠️ CRITICAL WARNING:** AI models can produce plausible-sounding but **incorrect** information. This is especially dangerous in engineering contexts where errors can have real consequences.

**High-Risk Areas for EE Students:**

| Area | Risk | Example of AI Error |
|---|---|---|
| **Equations** | May produce formulas with wrong signs, missing terms, or incorrect units | Giving the transfer function of a Butterworth filter with wrong order polynomial |
| **Citations** | May fabricate paper titles, authors, and DOIs that don't exist | "See Smith et al. (2020), IEEE Trans. Power Electronics" — paper doesn't exist |
| **Numerical data** | May invent performance metrics, component values | "The LM741 has a GBW of 10 MHz" (actual: ~1 MHz) |
| **Standards** | May cite wrong standard numbers or outdated versions | Referencing an IEC standard that was withdrawn |
| **Code** | May generate code with subtle logical errors | Off-by-one errors in DSP implementations, wrong bit ordering |

**Verification Checklist:**
- ✅ Cross-reference any equation with your textbook or lecture notes
- ✅ Verify ALL citations actually exist (search by DOI or title)
- ✅ Check component datasheets for any specific numerical values
- ✅ Run any provided code and verify outputs against known solutions
- ✅ Be especially skeptical of specific numbers, names, and dates

**Healthy Mindset:**
```
Treat AI output like a first draft from a knowledgeable but 
occasionally unreliable colleague — useful starting point, 
always needs verification.
```

### 8.2 Prompt Injection Risks (Awareness Level)

**What it is:** "Prompt injection" means someone hides instructions inside text that the AI processes, causing it to behave differently than intended.

**Why you should know about it:**
- If you paste text from untrusted sources into your prompts, hidden instructions could affect the output
- When building applications that use AI, this is a security concern
- Awareness helps you understand AI limitations

**Practical relevance for students:**
- When you paste text from a website or document into a prompt, be aware that the text might contain hidden instructions
- If AI output suddenly changes style or seems off-topic, this might be why
- This is primarily a software security issue, but awareness is part of digital literacy

### 8.3 Getting Generic Output: How to Force Specificity

**The Problem:** You ask a question and get a textbook-generic answer that doesn't help with your specific situation.

**Why it happens:** Generic prompts get generic answers. The AI defaults to the most common/general response when it lacks specificity.

**Techniques to Force Specificity:**

| Technique | Example |
|---|---|
| **Specify your exact context** | Instead of "How to reduce noise" → "How to reduce EMI in a PCB with a 100MHz clock signal, 4-layer stackup, FR-4, mixed analog/digital design" |
| **Add constraints** | "Assume: budget < $50 for components, must use components available on Digi-Key, Texas Instruments preferred" |
| **Ask for tradeoffs** | "Don't just give me the textbook answer. Explain the tradeoffs between the options and when each is appropriate" |
| **Request specific format** | "Give me a step-by-step procedure I can follow in the lab tomorrow, with specific test equipment settings" |
| **Reject generic and ask again** | "That's too general. I specifically need to know about [narrow aspect]. Focus only on that." |
| **Provide your attempt** | "Here's what I've tried so far: [your work]. Why isn't this working for [specific problem]?" |

**Before and After:**

❌ **Generic prompt:**
```
How do I design a low-pass filter?
```
→ Gets textbook RC filter explanation

✅ **Specific prompt:**
```
I need to design a 4th-order active low-pass filter for an 
ECG signal acquisition circuit. Specifications:
- Cutoff frequency: 150 Hz
- Passband ripple: < 0.5 dB  
- Power supply: ±5V (battery powered, low current)
- Input signal: 0.1-5 mV from instrumentation amplifier
- Noise: must reject 50 Hz powerline harmonic at 250 Hz by at least 40 dB

Should I use Butterworth or Chebyshev topology? What op-amp 
would you recommend given the low-power constraint? Show the 
component calculations for the chosen topology.
```
→ Gets actionable, specific design guidance

### 8.4 The "Garbage In, Garbage Out" Principle

This classic engineering principle applies perfectly to prompting:

| What You Put In | What You Get Out |
|---|---|
| Vague, unfocused question | Vague, unfocused answer |
| Clear question with no context | Correct but generic answer |
| Specific question + context + constraints | Targeted, useful answer |
| Wrong assumptions in your prompt | Confidently wrong answer |
| Contradictory instructions | Confused, inconsistent output |
| Well-structured, precise prompt | Well-structured, precise output |

**The key insight:** The quality of your output is **bounded** by the quality of your input. No AI can give you a great answer to a bad question.

**Self-check before sending a prompt:**
1. Have I clearly stated what I want? (Task)
2. Have I given enough context? (Background)
3. Have I specified the format? (Output requirements)
4. Is my prompt free of contradictions? (Consistency)
5. Would a knowledgeable human understand this without follow-up questions? (Completeness)

### 8.5 When Prompting Fails: Recognizing the Limits

**AI is NOT good at:**
- Verifying if real-world references exist (it may hallucinate citations)
- Performing precise numerical calculations (use MATLAB, Python, calculators)
- Accessing real-time data (stock prices, current sensor readings)
- Understanding your specific physical setup without detailed description
- Replacing peer review or expert judgment for novel research claims
- Making ethical or safety decisions for real engineering systems

**Recognizing when to stop prompting and use other tools:**

| Situation | Better Approach |
|---|---|
| Need exact numerical calculation | Use MATLAB/Python/calculator, ask AI to check your approach |
| Need a specific real paper | Search IEEE Xplore/Scopus/Google Scholar directly |
| AI gives conflicting answers across prompts | Consult textbook, professor, or verified source |
| Problem requires your engineering judgment | Use AI for information gathering, make decision yourself |
| Need to verify a circuit works | Simulate in LTspice/Multisim, don't trust AI simulation claims |
| Output seems too good or too specific | Verify independently — it might be fabricated |

**When to iterate vs. when to give up:**
- If 3 different prompt formulations give the same wrong answer → the AI may not have this knowledge correctly
- If the AI keeps misunderstanding your question → simplify and break into smaller parts
- If the AI explicitly says "I'm not sure" → take that seriously



---

## 9. Practical Exercises

> **Instructions:** These exercises are designed for hands-on practice with actual AI tools. For each exercise, you should write your prompts, test them, evaluate the outputs, and refine. Keep a log of your prompt iterations — the learning is in the refinement process.

---

### Exercise 1: Prompt Comparison — Explaining Beamforming

**Objective:** Understand how different prompts produce different explanations of the same concept.

**Task:**
Write THREE different prompts to get an explanation of **beamforming in antenna arrays**. Each prompt should target a different level or perspective.

**Requirements:**
- **Prompt A:** Write a zero-shot prompt (no examples, no role) for a simple explanation
- **Prompt B:** Write a prompt with role assignment and audience specification
- **Prompt C:** Write a prompt that uses chain-of-thought and requests a specific format

**Template:**

| Prompt Version | Your Prompt | Output Quality (1-5) | What worked | What didn't |
|---|---|---|---|---|
| A (zero-shot) | | | | |
| B (role + audience) | | | | |
| C (CoT + format) | | | | |

**Evaluation criteria:**
1. Which prompt produced the most useful explanation for YOUR level?
2. Which explanation would be best for a presentation to classmates?
3. Which would be best for exam preparation?
4. Write a 50-word reflection on how prompt structure affects output quality.

**Starter (if you're stuck):**
- Prompt A could be: "Explain beamforming."
- Prompt B could start with: "You are a telecommunications professor..."
- Prompt C could include: "Explain step by step how beamforming works, starting from a single antenna element, then showing how adding elements creates directionality..."

---

### Exercise 2: Iterative Abstract Improvement

**Objective:** Practice the iterative refinement approach to improve weak academic writing.

**Task:** Start with this deliberately weak abstract and use a series of prompts to improve it:

**Weak Abstract:**
```
"This paper talks about a new method for detecting faults in 
power systems. We use neural networks to find faults. The method 
works very well and is better than other methods. We tested it 
and got good results. The accuracy is high. This can be used in 
real power systems to help detect faults faster."
```

**Steps:**
1. **First prompt:** Ask the AI to identify ALL problems with this abstract (don't fix yet, just diagnose)
2. **Second prompt:** Ask the AI to fix the structural problems while keeping the same (fake) content
3. **Third prompt:** Now provide "real" data and ask the AI to integrate it:
   - Method: CNN with 3 convolutional layers trained on PMU data
   - Test system: IEEE 39-bus New England test system
   - Results: 98.7% accuracy for fault type classification, 94.2% for fault location (within 2% of line length)
   - Comparison: Outperforms SVM (93.1%) and random forest (95.4%)
   - Speed: 15ms classification time (suitable for real-time protection)
4. **Fourth prompt:** Final polish — ask for word count reduction to exactly 150 words while maintaining all key information

**Deliverable:** Submit all four prompts and the progressive outputs. Write a 100-word reflection on what you learned about iterative improvement.

---

### Exercise 3: Template Creation — IEEE Paper Summary

**Objective:** Create a reusable prompt template that works for any IEEE paper.

**Task:**
1. Find 3 different IEEE papers from different EE sub-fields (e.g., one from power, one from communications, one from control systems)
2. Design a single prompt template with [PLACEHOLDERS] that works for all three
3. Test the template with each paper
4. Refine the template based on what didn't work well

**Requirements for your template:**
- Must extract: main contribution, methodology, key results, limitations
- Must rate relevance to a customizable research topic
- Must identify 3 key terms from the paper with definitions
- Must suggest one follow-up question for deeper understanding
- Output format must be consistent across all papers

**Evaluation:**
- Does the template produce consistent output format for all 3 papers?
- Does it capture the most important information each time?
- Is it concise enough to be practical?
- Could a classmate use your template without modifications?

---

### Exercise 4: Thesis Defense Q&A Preparation

**Objective:** Use prompting to prepare for challenging questions in an academic defense.

**Scenario:** You are defending your bachelor's thesis on ONE of these topics (choose one or use your own):
- A) "Design and Implementation of a MPPT Algorithm for Partial Shading Conditions"
- B) "FPGA-Based Real-Time Power Quality Monitoring System"
- C) "Machine Learning-Based Intrusion Detection for Smart Grid Communication Networks"

**Tasks:**
1. Write a prompt that generates 15 potential defense questions (5 easy, 5 medium, 5 hard)
2. For the 5 hardest questions, write follow-up prompts to get help formulating answers
3. Write a prompt that simulates a hostile examiner who questions your methodology choices
4. Write a prompt that helps you prepare 3-sentence answers for each question (concise, confident, complete)

**Deliverable:** Your prompts, the generated questions, and your prepared answers. Also: one "surprise question" you didn't expect that the AI generated, and how you would handle it.

---

### Exercise 5: Research Question → Search Strategy

**Objective:** Transform vague research interests into effective database search strategies.

**Task:** Start with these vague research interests and use prompts to convert them into effective search strategies:

**Vague Interest A:** "I want to research something about electric vehicle charging"
**Vague Interest B:** "I'm interested in using AI for something in telecommunications"
**Vague Interest C:** "I want to work on renewable energy storage"

**For each interest, write prompts that:**
1. Help narrow the broad topic to 3 specific research questions
2. Generate Boolean search strings for each question
3. Identify 5 key journals/conferences where relevant papers would be published
4. Suggest inclusion/exclusion criteria for a literature review

**Evaluation:** Test at least one Boolean search string in IEEE Xplore or Google Scholar. Report:
- How many results did you get?
- Were the first 5 results relevant?
- How would you refine the search based on initial results?

---

### Exercise 6: Chain-of-Thought for Circuit Analysis

**Objective:** Practice chain-of-thought prompting for complex multi-step problems.

**Task:** Use the following circuit problem and write CoT prompts:

**Problem:**
```
A cascaded amplifier consists of:
- Stage 1: Common-emitter BJT amplifier (β = 100, RC = 4.7kΩ, 
  RE = 1kΩ, VCC = 12V, voltage divider bias)
- Stage 2: Common-collector (emitter follower) output stage 
  (β = 150, RE = 100Ω)
- Coupling capacitors between stages: 10μF
- Load: 8Ω speaker

Analyze at f = 1kHz.
```

**Write prompts for:**
1. DC bias point analysis (step by step, showing each assumption)
2. Small-signal AC analysis of each stage separately
3. Combined gain and impedance analysis
4. Frequency response discussion (what limits the bandwidth?)
5. A "check my work" prompt where you provide a deliberately wrong calculation and ask the AI to find your error

**Key requirement:** Each prompt must include "show your reasoning" and "verify physical reasonableness" instructions.

---

### Exercise 7: Paper → Presentation Outline

**Objective:** Convert research paper content into an effective presentation structure.

**Task:**
1. Choose any published IEEE paper (something you've read or are reading for a course)
2. Write a prompt that converts the paper's content into a 15-minute presentation outline
3. Then write a follow-up prompt to generate speaker notes for the 3 most critical slides
4. Write a third prompt to create a "backup slide" Q&A reference

**Your initial prompt must specify:**
- Time limit (15 minutes = approximately 12-14 slides)
- Audience (your classmates — what they know, what they don't)
- Your emphasis (what you find most interesting/novel about the paper)
- Format requirements (slide titles, max bullets per slide, where visuals go)

**Evaluation questions:**
- Does the outline have a logical flow?
- Is the time allocation realistic?
- Would you actually use this outline?
- What did you need to adjust manually?

---

### Exercise 8: Technical Translation (Persian → Academic English)

**Objective:** Practice prompt engineering for translation tasks that require domain expertise.

**Task:** Translate the following Persian technical paragraph into academic English using different prompting approaches:

**Persian Text:**
```
در این پروژه، یک سیستم کنترل سرعت موتور القایی سه‌فاز با استفاده از 
روش کنترل بُرداری طراحی و شبیه‌سازی شده است. هدف اصلی این است که 
سرعت موتور در برابر تغییرات بار ثابت بماند. ابتدا مدل ریاضی موتور 
در قاب مرجع dq استخراج شده و سپس کنترل‌کننده‌های PI برای حلقه جریان 
و سرعت طراحی شده‌اند. نتایج شبیه‌سازی در MATLAB/Simulink نشان می‌دهد 
که پاسخ سرعت دارای زمان صعود ۰.۲ ثانیه و بدون فراجهش است.
```

**Write three different prompts:**
- **Prompt A:** Simple translation request (minimal guidance)
- **Prompt B:** Translation with academic English requirements (specify IEEE style, formal register, standard EE terminology)
- **Prompt C:** Translation + improvement (translate AND enhance for publication quality, with notes on what was changed and why)

**Compare the three outputs:**
- Which maintains technical accuracy best?
- Which sounds most natural in academic English?
- Which would require the least human editing?
- Identify any Persian terms that were translated inconsistently

---

### Exercise 9: Zero-Shot vs. Few-Shot Comparison

**Objective:** Empirically demonstrate the difference between zero-shot and few-shot prompting.

**Task:** Choose this task: **"Convert informal lab observations into formal results statements"**

**Step 1 — Zero-shot prompt:**
```
Convert this informal observation into a formal results statement 
for a journal paper:

"The filter worked pretty well up to about 1kHz but then 
started cutting off the signal. The rolloff was about 20dB 
per decade which is what we expected for a first-order filter."
```

**Step 2 — Few-shot prompt (same task, but with examples first):**
```
Convert informal lab observations into formal results statements 
for a journal paper. Here are examples:

Informal: "The amplifier gain dropped by half at around 150kHz"
Formal: "The measured -3dB bandwidth of the amplifier was 148.3 kHz, 
corresponding to a gain reduction from 26.2 dB to 23.2 dB."

Informal: "The motor speed went up linearly when we increased the voltage"
Formal: "A linear relationship between armature voltage and shaft 
speed was observed (R² = 0.997), with a measured speed constant 
of 142 rpm/V across the tested range of 5-24V."

Now convert this observation:
"The filter worked pretty well up to about 1kHz but then 
started cutting off the signal. The rolloff was about 20dB 
per decade which is what we expected for a first-order filter."
```

**Evaluation:**
- Compare both outputs side by side
- Which is more specific? More accurate in tone? Better formatted?
- Write 3 observations about the differences
- For what types of tasks does few-shot make the biggest difference?

---

### Exercise 10: Diagnostic Exercise — Fix Bad Prompts

**Objective:** Develop your ability to identify and fix problematic prompts.

**Task:** For each of the following bad prompts, identify the problems and write an improved version:

**Bad Prompt 1:**
```
"Tell me about transformers"
```
Problems to identify: _____
Your improved version: _____

**Bad Prompt 2:**
```
"I have a problem with my circuit it doesn't work the output 
is wrong can you help me fix it please"
```
Problems to identify: _____
Your improved version: _____

**Bad Prompt 3:**
```
"You are the world's best electrical engineer with 50 years of 
experience and 200 patents and you know everything about every 
topic in all of electrical engineering and physics and mathematics. 
Now explain how a capacitor works."
```
Problems to identify: _____
Your improved version: _____

**Bad Prompt 4:**
```
"Write my entire thesis chapter 3 on the methodology of using 
deep learning for power system state estimation. Make it 5000 
words with proper citations from real papers."
```
Problems to identify: _____
Your improved version: _____

**Bad Prompt 5:**
```
"Is OFDM better than CDMA? Give me the answer for my exam."
```
Problems to identify: _____
Your improved version: _____

**For each fix, explain:**
1. What specific communication principle was violated (precision? context? scope? format?)
2. How does your fix apply the principles from Section 2 of this module?
3. What different/better output would you expect from the fixed version?



---

## 10. Prompt Library for EE Students

> **How to Use This Library:** These are ready-to-use prompt templates. Copy them, replace the [BRACKETED PLACEHOLDERS] with your specific information, and use directly. Each template has been designed to produce high-quality, specific outputs for common EE student tasks.

---

### 10.1 Research Keyword Generation

```
PROMPT TEMPLATE: Research Keyword Generator

I am researching: [YOUR RESEARCH TOPIC IN 1-2 SENTENCES]

Sub-field: [POWER / CONTROL / COMMUNICATIONS / SIGNAL PROCESSING / 
ELECTRONICS / EMBEDDED / RF / OTHER]

My specific angle/focus: [WHAT MAKES YOUR APPROACH DIFFERENT]

Generate a comprehensive keyword strategy:

1. PRIMARY KEYWORDS (5-8 direct terms)
2. SYNONYMS & ALTERNATIVES (for each primary keyword)
3. BROADER TERMS (for expanding search if too few results)
4. NARROWER TERMS (for focusing if too many results)
5. METHODOLOGY KEYWORDS (terms related to the approach/method)
6. APPLICATION KEYWORDS (terms related to the application domain)
7. BOOLEAN SEARCH STRINGS (3 different combinations for IEEE Xplore)
8. MESH/THESAURUS TERMS (standardized terms used in databases)

Target databases: IEEE Xplore, Scopus, Google Scholar
Time range for search: [LAST 5 YEARS / LAST 10 YEARS / ALL]
```

---

### 10.2 Paper Summarization

```
PROMPT TEMPLATE: Paper Summary for Literature Review

Paper Title: [TITLE]
Authors: [AUTHORS]
Source: [JOURNAL/CONFERENCE, YEAR]
DOI: [DOI IF AVAILABLE]

Content to summarize: [PASTE ABSTRACT + CONCLUSION, OR KEY SECTIONS]

Summarize using this EXACT format:

## Quick Reference
- **One-sentence summary:** [max 30 words]
- **Category:** [theoretical / experimental / simulation / review / hybrid]
- **Relevance to my work:** [HIGH / MEDIUM / LOW] — because [reason]

## Detailed Summary (200 words max)
- **Problem addressed:**
- **Proposed solution/method:**
- **Key innovation (what's new):**
- **Validation approach:**
- **Main results (with numbers):**
- **Acknowledged limitations:**

## For My Thesis
- **Useful for my section:** [Introduction / Lit Review / Method / Discussion]
- **Key citation sentence:** [A sentence I could write in my paper citing this work]
- **Builds on:** [What prior work this paper extends]
- **Extended by:** [What future work it suggests]

## Key Terms Defined
- [Term 1]: [Definition in context of this paper]
- [Term 2]: [Definition]
- [Term 3]: [Definition]
```

---

### 10.3 Concept Explanation

```
PROMPT TEMPLATE: EE Concept Explainer

Concept: [THE CONCEPT YOU WANT EXPLAINED]
Course/Context: [WHERE YOU ENCOUNTERED IT]

My current knowledge:
- I understand: [RELATED CONCEPTS YOU'RE COMFORTABLE WITH]
- I don't understand: [SPECIFIC GAPS OR CONFUSING ASPECTS]
- Math level: [ALGEBRA / CALCULUS / DIFFERENTIAL EQUATIONS / LINEAR ALGEBRA / ALL]

Please explain using this structure:

1. INTUITION (2-3 sentences — what IS this, conceptually?)
2. WHY IT MATTERS (real-world motivation in EE — when/where is this used?)
3. THE MATH (build up from what I know, define every new symbol)
4. WORKED EXAMPLE (realistic EE values, show every step)
5. COMMON MISCONCEPTIONS (what do students typically get wrong?)
6. CONNECTION TO OTHER CONCEPTS (how does this relate to things I already know?)
7. PRACTICE PROBLEM (for me to try — include answer)

Constraints:
- Do not use concepts I listed as "don't understand" without explaining them first
- Use [SI / CGS / STANDARD EE] units throughout
- Include physical intuition alongside mathematical derivation
```

---

### 10.4 Grammar Checking

```
PROMPT TEMPLATE: Technical Grammar Review

Text type: [ABSTRACT / METHODOLOGY / RESULTS / DISCUSSION / EMAIL / REPORT]
Target style: [IEEE JOURNAL / CONFERENCE PAPER / THESIS / INFORMAL REPORT]
My L1: Persian (Farsi)

Review the following text for:
1. Grammar errors (especially articles, prepositions, subject-verb agreement)
2. Common Persian-speaker errors (article omission, wrong prepositions, 
   literal translations)
3. Academic register issues (too informal? too formal? inconsistent?)
4. Tense consistency (appropriate use of present/past/present perfect)
5. Technical term consistency (same concept = same term throughout)
6. Sentence structure variety (avoid repetitive patterns)
7. Hedging/boosting appropriateness (claims vs. facts vs. speculation)

Format your feedback as:

| Line | Original | Corrected | Error Type | Rule/Explanation |
|------|----------|-----------|-----------|-----------------|
| ...  | ...      | ...       | ...       | ...             |

After the table: Overall assessment (strengths + top 3 areas to focus on)

TEXT:
[PASTE YOUR TEXT HERE]
```

---

### 10.5 Paraphrasing

```
PROMPT TEMPLATE: Technical Paraphraser

Purpose: I need to paraphrase this text for [my literature review / 
to avoid self-plagiarism / to simplify / to make more formal]

Original text:
"[PASTE TEXT]"

Source: [WHERE THIS TEXT IS FROM]

Requirements:
- Change sentence structure significantly (not just synonym swapping)
- Maintain 100% technical accuracy — do not change the meaning
- Keep the same level of specificity (don't generalize or add detail)
- Preserve all numerical values, measurements, and specific claims
- Use standard EE terminology (don't invent new terms)
- Target word count: [APPROXIMATELY SAME / SHORTER BY X% / LONGER BY X%]
- Do NOT change these terms (they are standard): [LIST TERMS TO KEEP]

Provide:
1. The paraphrased text
2. A similarity check: how different is it from the original? (score 1-10, where 10 = completely different wording)
3. Flag any places where changing the wording might change the meaning
```

---

### 10.6 Email Writing

```
PROMPT TEMPLATE: Academic/Professional Email

Scenario: [DESCRIBE THE SITUATION IN 2-3 SENTENCES]

Recipient: [ROLE + RELATIONSHIP TO YOU]
(e.g., "Professor I've never met," "My thesis supervisor," 
"Conference organizers," "Company HR for internship")

Purpose: [WHAT DO YOU NEED FROM THEM?]

Key information to include:
- [Point 1]
- [Point 2]
- [Point 3]

My name: [YOUR NAME]
My title/position: [YOUR POSITION]
My relevant credential: [WHAT GIVES YOU CREDIBILITY FOR THIS EMAIL]

Tone: [FORMAL / SEMI-FORMAL]
Length: [SHORT (5 sentences) / MEDIUM (8-10 sentences) / LONGER]

Cultural notes: 
- Avoid excessive hedging or apology (common in Persian academic culture 
  but sounds unconfident in English)
- Be direct about what you need
- Be specific about why you're contacting THEM specifically

Write the email with:
- Clear subject line
- Appropriate greeting
- Body with clear purpose in first 2 sentences
- Specific request/action item
- Professional closing
```

---

### 10.7 CV Improvement

```
PROMPT TEMPLATE: CV Bullet Point Optimizer

Target: [PHD APPLICATION / INDUSTRY JOB / INTERNSHIP / SCHOLARSHIP]
Field: [SPECIFIC EE SUB-FIELD]
Target country/culture: [COUNTRY — to adjust formality and style]

Current bullet points (from my [Education / Experience / Projects / Skills] section):

1. [YOUR BULLET 1]
2. [YOUR BULLET 2]
3. [YOUR BULLET 3]
4. [YOUR BULLET 4]
5. [YOUR BULLET 5]

Improve each bullet point to:
- Start with a strong, specific action verb (designed, implemented, 
  analyzed, optimized — not "responsible for" or "worked on")
- Include quantifiable achievements (%, numbers, comparisons)
- Highlight technical skills with specific tools/technologies
- Use PAR format where applicable (Problem/Action/Result)
- Be concise: max 1.5 lines, no unnecessary words
- Be tailored to [TARGET POSITION/FIELD]

For each improved bullet, show:
[Original] → [Improved] + brief note on what changed and why
```

---

### 10.8 Presentation Outline

```
PROMPT TEMPLATE: Technical Presentation Outline Generator

Topic: [YOUR PRESENTATION TOPIC]
Source material: [PAPER / THESIS CHAPTER / PROJECT REPORT / RESEARCH PROPOSAL]
Time limit: [X] minutes
Audience: [WHO + WHAT THEY KNOW + WHAT THEY DON'T KNOW]

Key content to cover:
- [MAIN POINT 1]
- [MAIN POINT 2]
- [MAIN POINT 3]
- [KEY RESULT OR MESSAGE]

Generate a presentation outline with:

For each slide:
| Slide # | Title | Key Message (1 sentence) | Content (max 4 bullets) | Visual Suggestion | Time (seconds) |

Also provide:
- Opening hook: first 30 seconds to grab attention
- Transition sentences between major sections
- Conclusion slide: 3 take-home messages
- Backup slides: 3 anticipated questions with prepared slide content
- Total time check: does it fit in [X] minutes at ~1 min/slide pace?

Style preferences:
- [TECHNICAL DEPTH LEVEL]
- [VISUAL HEAVY vs TEXT HEAVY]
- [FORMAL vs CONVERSATIONAL delivery style]
```

---

### 10.9 Q&A Preparation

```
PROMPT TEMPLATE: Q&A Defense/Presentation Preparation

Presentation topic: [TOPIC]
Context: [THESIS DEFENSE / CONFERENCE / CLASS PRESENTATION / JOB INTERVIEW]
My main claims/contributions: 
1. [CLAIM 1]
2. [CLAIM 2]
3. [CLAIM 3]

Potential weaknesses I'm aware of:
- [LIMITATION 1]
- [LIMITATION 2]

Audience composition: [WHO WILL ASK QUESTIONS — supervisors? peers? experts in other fields?]

Generate:

## Likely Questions (15 total)
### Clarification Questions (5) — testing if audience understood
### Technical Questions (5) — testing depth of knowledge
### Critical Questions (5) — challenging methodology or claims

For each question provide:
- The question
- Why someone might ask this (what are they really checking?)
- A concise answer (3-4 sentences max — confident, honest, specific)
- If relevant: "I don't know, but..." response framework
- Redirect phrase if the question is outside your scope

## "Difficult Question" Strategies
- 3 questions where admitting limitations is the best answer
- How to say "that's future work" professionally
- How to handle a question about something you didn't study
```

---

### 10.10 Technical Translation

```
PROMPT TEMPLATE: Persian Technical → English Academic Translation

Source language: Persian (Farsi)
Target: Academic English suitable for [IEEE PAPER / THESIS / REPORT]
Field: Electrical Engineering — [SUB-FIELD]

Persian text:
[PASTE PERSIAN TEXT]

Translation requirements:
1. Use STANDARD English EE terminology (not literal translations)
   - Example: "کنترل‌کننده" → "controller" (not "controlling device")
   - Example: "بهره" → "gain" (not "profit" or "benefit")
2. Maintain academic register throughout
3. Keep all equations, variable names, and units unchanged
4. Follow English academic conventions:
   - Article usage (a/an/the) — critical for Persian speakers
   - Passive voice where appropriate for methodology descriptions
   - Hedging language for claims (suggest, indicate, may)
5. Restructure sentences for English word order if the Persian 
   structure would be unnatural in English

Output format:
1. Translation
2. Terminology table: | Persian Term | English Equivalent | Notes |
3. Flags: Any ambiguous phrases where interpretation was needed
4. Style suggestions: Ways to further improve for publication
```



---

## 11. Vocabulary Box: Prompt Engineering Terminology

> **مفردات مهندسی پرامپت** — Key terms with definitions, Persian equivalents, and usage examples in EE contexts.

| # | Term (English) | Persian Equivalent | Definition | Example in EE Context |
|---|---|---|---|---|
| 1 | **Prompt** | پرامپت / دستور ورودی | The text instruction given to an AI model to elicit a response | "Design a low-pass filter with 1kHz cutoff" is a prompt |
| 2 | **Zero-shot prompting** | پرامپت بدون نمونه | Asking the AI to perform a task without providing examples | Asking "What is skin effect?" without showing example answers |
| 3 | **Few-shot prompting** | پرامپت با چند نمونه | Providing 1-5 examples of desired input-output pairs before the actual task | Showing 2 example circuit analyses before asking for a 3rd |
| 4 | **Chain-of-thought (CoT)** | زنجیره تفکر | Prompting the AI to show reasoning steps, improving accuracy on complex tasks | "Analyze this Thevenin circuit step by step, showing each calculation" |
| 5 | **System prompt** | پرامپت سیستمی | A persistent instruction that sets the AI's behavior for an entire conversation | "You are a power systems tutor. Always use per-unit calculations." |
| 6 | **Temperature** | دمای تولید | A parameter controlling output randomness (low=focused, high=creative) | Low temperature for precise calculations; higher for brainstorming research ideas |
| 7 | **Token** | توکن | The basic unit of text processed by the AI (roughly ¾ of an English word) | "Electromagnetic interference" ≈ 3-4 tokens |
| 8 | **Token limit / Context window** | حد توکن / پنجره زمینه | Maximum amount of text (input + output) the model can process at once | If window is 8K tokens, a very long paper may not fit entirely |
| 9 | **Hallucination** | توهم / خروجی ساختگی | When the AI generates plausible-sounding but factually incorrect information | AI claims a paper exists with a fabricated DOI — the paper is not real |
| 10 | **Grounding** | پایه‌گذاری / اتصال به واقعیت | Techniques to anchor AI output in verified facts or provided documents | Pasting actual paper text and asking AI to summarize only what's there |
| 11 | **Retrieval-Augmented Generation (RAG)** | تولید تقویت‌شده با بازیابی | A system that retrieves relevant documents before generating a response | A tool that searches IEEE Xplore first, then answers your question using found papers |
| 12 | **Fine-tuning** | تنظیم دقیق | Further training a model on specific data to specialize its behavior | A model fine-tuned on power systems papers would know more specialized terminology |
| 13 | **Role prompting** | نقش‌دهی به مدل | Assigning a specific identity/expertise to the AI to shape its response | "You are an experienced PCB layout engineer reviewing my design..." |
| 14 | **Prompt template** | قالب پرامپت | A reusable prompt structure with placeholders for customization | A standard format for requesting paper summaries with [TITLE] and [ABSTRACT] fields |
| 15 | **Iterative refinement** | بهینه‌سازی تدریجی | The process of improving AI output through multiple rounds of feedback | First draft → "make it more concise" → "add quantitative data" → final version |
| 16 | **Context** | زمینه / بافت | Background information provided to help the AI understand the situation | "I am a 4th-year student; my thesis is on MPPT algorithms" |
| 17 | **Constraint** | محدودیت / قید | Boundaries or limitations specified in the prompt | "Use only passive components" or "Keep explanation under 200 words" |
| 18 | **Meta-prompting** | فرا-پرامپت‌نویسی | Asking the AI to help you write better prompts | "How can I improve this prompt to get more specific results?" |
| 19 | **Prompt injection** | تزریق پرامپت | A security concern where hidden text manipulates AI behavior | Malicious text in a document that changes AI behavior when processed |
| 20 | **Output format** | قالب خروجی | Specification of how the response should be structured | "Present as a table with columns: Parameter, Value, Unit" |
| 21 | **Persona** | شخصیت / نقش | The character or expert identity assigned to the AI | "Act as an IEEE reviewer" vs "Act as a patient tutor" |
| 22 | **Specificity** | دقت / مشخص بودن | The degree of detail and precision in a prompt | "Explain capacitors" (low) vs. "Explain MLCC derating curves for X7R dielectric at 50V DC bias" (high) |
| 23 | **Ambiguity** | ابهام | Unclear language that could be interpreted multiple ways | "Make it better" — better how? Style? Accuracy? Length? |
| 24 | **Scope** | دامنه / محدوده | The boundaries of what the prompt asks the AI to address | "Focus only on the thermal design aspects, not electrical" |
| 25 | **Inference** | استنتاج | The AI's process of generating output from input | The computational step where the model processes your prompt and produces text |

---

### Additional Terminology: Useful Phrases for Prompting

| Purpose | English Phrase | When to Use |
|---|---|---|
| Setting difficulty | "at the level of a [year] undergraduate" | When you need appropriately leveled explanations |
| Requesting structure | "organize your response as..." | When you need specific formatting |
| Limiting scope | "focus exclusively on..." | When you want to prevent off-topic content |
| Requesting honesty | "if you're not sure, say so" | When accuracy is critical |
| Asking for alternatives | "provide 3 different approaches" | When exploring options |
| Checking understanding | "explain my error in reasoning" | When learning from mistakes |
| Requesting depth | "go deeper on point 3" | During iterative refinement |
| Requesting brevity | "in 50 words or fewer" | When you need concise answers |
| Requesting comparison | "compare X and Y in terms of..." | When evaluating options |
| Setting format | "present as a table with columns:" | When you need structured data |

---

## Summary: Key Principles to Remember

```
┌─────────────────────────────────────────────────────────────────┐
│            THE 10 COMMANDMENTS OF EFFECTIVE PROMPTING            │
├─────────────────────────────────────────────────────────────────┤
│                                                                  │
│  1. BE SPECIFIC — Vague input = vague output                    │
│                                                                  │
│  2. PROVIDE CONTEXT — The AI doesn't know your situation        │
│                                                                  │
│  3. DEFINE THE TASK CLEARLY — What exactly should it DO?        │
│                                                                  │
│  4. SPECIFY FORMAT — How should the output look?                │
│                                                                  │
│  5. SET CONSTRAINTS — What are the boundaries?                  │
│                                                                  │
│  6. GIVE EXAMPLES — Show, don't just tell                       │
│                                                                  │
│  7. ITERATE — First output is a draft, not final answer         │
│                                                                  │
│  8. VERIFY — Never trust AI output without checking             │
│                                                                  │
│  9. THINK FIRST — Confused prompts = confused outputs           │
│                                                                  │
│  10. CONNECT TO COMMUNICATION SKILLS — Good prompter =          │
│      good technical communicator                                 │
│                                                                  │
└─────────────────────────────────────────────────────────────────┘
```

---

## Connection to Course Learning Outcomes

| Course Skill (Parts 1-7) | Prompt Engineering Application (Part 8) |
|---|---|
| Academic writing structure (IMRaD) | Structuring prompts with clear components |
| Audience awareness | Understanding the LLM as "reader" |
| Precision in technical vocabulary | Using specific terms in prompts |
| Research methodology | Systematic prompt design and iteration |
| Critical reading | Critically evaluating AI output |
| Presentation skills | Using AI to prepare and refine presentations |
| Grammar accuracy | Using AI as a grammar tool with proper instructions |
| Literature review skills | Using AI to organize and synthesize sources |
| Professional communication | Using AI for email and CV drafting |
| Persian → English translation | Using AI as a domain-aware translation tool |

---

## Recommended Practice Schedule

| Week | Focus | Key Exercise |
|---|---|---|
| Week 1 | Sections 1-2: Fundamentals | Exercise 10 (diagnose bad prompts) |
| Week 2 | Section 3: Research prompts | Exercise 5 (search strategy) |
| Week 3 | Section 4: Writing assistance | Exercise 2 (iterative abstract) |
| Week 4 | Sections 5-6: Learning & Presentations | Exercise 7 (presentation outline) |
| Week 5 | Section 7: Advanced techniques | Exercise 6 (chain-of-thought) + Exercise 9 (zero vs. few-shot) |
| Week 6 | Sections 8-10: Integration | Exercise 4 (thesis defense) + Build personal prompt library |

---

## References and Further Reading

1. White, J., et al. (2023). "A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT." *arXiv preprint arXiv:2302.11382.*
2. Liu, P., et al. (2023). "Pre-train, Prompt, and Predict: A Systematic Survey of Prompting Methods in Natural Language Processing." *ACM Computing Surveys.*
3. Wei, J., et al. (2022). "Chain-of-Thought Prompting Elicits Reasoning in Large Language Models." *NeurIPS 2022.*
4. OpenAI. (2023). "Best Practices for Prompt Engineering." *OpenAI Documentation.*
5. Giray, L. (2023). "Prompt Engineering with ChatGPT: A Guide for Academic Writers." *Annals of Biomedical Engineering.*

---

> **Final Note (یادداشت پایانی):** Prompt engineering is not a fixed skill — it evolves as AI models improve. The principles in this module (clarity, specificity, structure, iteration) are timeless communication principles that will serve you regardless of which AI tools you use. Master the communication fundamentals, and you will adapt naturally to any new tool.

---

*End of Part 8 — Prompt Engineering for Scientific and Technical English*
*© STE Course, Electrical Engineering Department*
*Last updated: 2026*
