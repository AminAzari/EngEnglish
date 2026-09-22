# Part 7: LLMs and AI Tools for Engineering Research & Communication

## Module Overview

| Item | Details |
|------|---------|
| **Duration** | 6 weeks (12 sessions × 90 minutes) |
| **Level** | B2–C1 (CEFR) |
| **Prerequisites** | Parts 1–6 of this course (research skills, academic writing, presentations, vocabulary, grammar) |
| **Focus** | Using AI tools effectively and ethically for engineering research and communication |
| **Assessment** | Portfolio of AI-assisted tasks + reflection essay + in-class activities |

### Module Learning Outcomes

By the end of this module, students will be able to:

1. Explain what Large Language Models are and how they work at a conceptual level
2. Use AI-powered tools to enhance (not replace) their research workflow
3. Apply LLMs appropriately for technical writing improvement
4. Evaluate AI output critically, identifying errors, hallucinations, and limitations
5. Navigate ethical considerations of AI use in academic and professional settings
6. Develop a personal AI-assisted workflow that maintains academic integrity
7. Articulate the limitations of AI tools, particularly for engineering applications

### A Note to Students

> **This module is not about replacing your skills with AI.** Throughout Parts 1–6, you developed essential abilities in research, writing, and presentation. Those skills are now *more* important than ever. AI tools are powerful assistants, but they require a knowledgeable human to guide them, verify their output, and take responsibility for the final work. Think of AI as a calculator for language — useful, but you still need to understand the mathematics.

---

## Week 1–2: What Are Large Language Models?

### 1.1 Definition and Core Concepts

A **Large Language Model (LLM)** is an artificial intelligence system trained on massive amounts of text data to understand and generate human language. At its core, an LLM is a sophisticated pattern-recognition system that predicts the most likely next word (or token) in a sequence.

#### How Do They Work? (High-Level Explanation)

Think of it this way: imagine you have read every textbook, research paper, website, and book ever written in English (and many other languages). After all that reading, you develop an intuition for how language works — what words typically follow other words, how arguments are structured, how technical concepts are explained. An LLM does something similar, but mathematically.

**The key components:**

| Component | What It Does | Analogy |
|-----------|--------------|---------|
| **Transformer Architecture** | The underlying structure that allows the model to process text | The "brain structure" of the AI |
| **Attention Mechanism** | Allows the model to focus on relevant parts of input text | Like highlighting key parts of a paper while reading |
| **Training Data** | Massive corpus of text (books, websites, papers, code) | The "education" the model received |
| **Parameters** | Internal mathematical values learned during training | Like synaptic connections in a biological brain |
| **Tokens** | Small pieces of text the model processes | Letters, syllables, or short words |

#### The Transformer Architecture (Simplified)

The **transformer** (introduced in 2017 by Vaswani et al. in the paper "Attention Is All You Need") revolutionized natural language processing. Before transformers, AI language models processed text sequentially — word by word, left to right. Transformers can process all words simultaneously, understanding relationships between distant parts of a text.

**EE Analogy:** Think of the difference between a serial communication protocol (processing one bit at a time) and a parallel bus (processing multiple bits simultaneously). Transformers brought "parallel processing" to language understanding.

The **attention mechanism** is the key innovation. It allows the model to determine which words in a sentence are most relevant to understanding each other word. For example, in the sentence:

> "The power MOSFET failed because its gate oxide was damaged during the ESD event."

The attention mechanism helps the model understand that "its" refers to "MOSFET," that "damaged" relates to "gate oxide," and that "ESD event" is the cause of the failure.

#### Training: How LLMs Learn

LLMs are trained in stages:

1. **Pre-training**: The model reads billions of text documents and learns to predict the next word. This is unsupervised — no human labels the data.
2. **Fine-tuning**: The model is refined on specific, high-quality data with human feedback (RLHF — Reinforcement Learning from Human Feedback).
3. **Alignment**: The model is trained to be helpful, harmless, and honest.

**Important for engineers:** The model does NOT "understand" physics or mathematics the way you do. It has learned *patterns* of how physics and mathematics are *discussed in text*. This is a crucial distinction.

### 1.2 Brief History: The ChatGPT Moment and Beyond

| Year | Milestone | Significance |
|------|-----------|--------------|
| 2017 | Transformer paper published | Foundation architecture for all modern LLMs |
| 2018 | GPT-1 (117M parameters) | First generative pre-trained transformer |
| 2019 | GPT-2 (1.5B parameters) | Surprisingly coherent text generation |
| 2020 | GPT-3 (175B parameters) | Demonstrated few-shot learning capabilities |
| Nov 2022 | **ChatGPT launched** | Made LLMs accessible to general public — 100M users in 2 months |
| Mar 2023 | GPT-4 released | Multimodal, significantly improved reasoning |
| 2023–2024 | Rapid proliferation | Claude, Gemini, Llama, Mistral, and dozens more |
| 2024–2025 | Reasoning models | o1, o3, DeepSeek-R1 — models that "think step by step" |
| 2025–2026 | Current era | Multimodal, agent-capable, domain-specific models |

**The ChatGPT Moment (November 30, 2022):**

This date marks a turning point. Before ChatGPT, LLMs were primarily used by researchers and developers. After ChatGPT, everyone — including students, professors, engineers, and the general public — could interact with a powerful AI through a simple chat interface. This created both tremendous opportunities and significant challenges for education and professional work.

### 1.3 Types of LLMs You Will Encounter

#### Commercial/Closed-Source Models

| Model Family | Developer | Key Strengths | Context Window | Notes |
|--------------|-----------|---------------|----------------|-------|
| **GPT-4 / GPT-4o** | OpenAI | Strong general reasoning, multimodal (text + image) | 128K tokens | Most widely used; available via ChatGPT |
| **o1 / o3 series** | OpenAI | Advanced reasoning, mathematics, coding | 128K–200K tokens | "Thinking" models — slower but more accurate for complex problems |
| **Claude 3.5 Sonnet / Claude 4** | Anthropic | Excellent writing, careful reasoning, long documents | 200K tokens | Strong at following nuanced instructions |
| **Gemini 1.5 Pro / 2.0** | Google | Very long context, multimodal, integrated with Google services | Up to 2M tokens | Can process entire textbooks in one prompt |

#### Open-Source / Open-Weight Models

| Model Family | Developer | Key Strengths | Why It Matters |
|--------------|-----------|---------------|----------------|
| **Llama 3.x** | Meta | Strong general performance, many fine-tuned variants | Free to use; can run locally; large community |
| **Mistral / Mixtral** | Mistral AI (France) | Efficient, strong for size, European data governance | Good balance of performance and resource requirements |
| **DeepSeek (R1, V3)** | DeepSeek (China) | Exceptional reasoning, competitive with top closed models | Free API; strong mathematics and coding capabilities |

#### Domain-Specific Models

| Model | Purpose | Relevance for EE Students |
|-------|---------|---------------------------|
| **Galactica** | Scientific text | Trained on scientific papers; understands LaTeX, citations |
| **SciBERT** | Scientific NLP | Better at understanding scientific terminology |
| **MatBERT** | Materials science | Useful for semiconductor and materials research |
| **Engineering-focused fine-tunes** | Various | Custom models trained on engineering documentation |

### 1.4 How Models Differ: A Comparison Framework

When choosing which AI tool to use, consider these dimensions:

| Dimension | What It Means | Why Engineers Care |
|-----------|---------------|-------------------|
| **Reasoning capability** | How well the model solves complex, multi-step problems | Critical for technical questions involving calculations or logic |
| **Context window** | How much text the model can process at once | Determines if you can paste an entire paper for analysis |
| **Multimodal ability** | Can it process images, diagrams, equations? | Essential for circuit diagrams, graphs, oscilloscope captures |
| **Cost** | Free tier vs. paid subscription vs. API pricing | Student budget considerations |
| **Open vs. Closed** | Can you run it locally? Is the code available? | Privacy, customization, offline use |
| **Training cutoff** | When was the model's knowledge last updated? | Recent papers and technologies may not be known |
| **Accuracy on STEM** | Performance on scientific and mathematical tasks | Not all models handle engineering content equally |

### 1.5 Key Concepts Every User Must Understand

#### Tokens (توکن)

A **token** is the basic unit of text that an LLM processes. Tokens are not exactly words — they are pieces of text that the model has learned to recognize.

- "electrical" = 1–2 tokens
- "semiconductor" = 2–3 tokens
- A typical research paper abstract (250 words) ≈ 350–400 tokens
- Mathematical equations may use many tokens for seemingly short expressions

**Why it matters:** You pay per token (on paid APIs), and there is a maximum context window measured in tokens.

#### Context Window (پنجره زمینه)

The **context window** is the maximum amount of text (in tokens) that a model can "see" at one time — both your input and the model's output combined.

| Model | Context Window | Equivalent to... |
|-------|---------------|------------------|
| GPT-4o | 128K tokens | ~300 pages of text |
| Claude 4 | 200K tokens | ~500 pages of text |
| Gemini 2.0 | 2M tokens | Several textbooks |

**Practical implication:** If you want to ask questions about a 50-page thesis, you need a model with a large enough context window to hold the entire document plus your questions.

#### Temperature (دما)

**Temperature** controls how "creative" or "random" the model's responses are:

- **Temperature 0**: Most predictable, deterministic output (best for factual questions, calculations)
- **Temperature 0.7**: Balanced (good for general use)
- **Temperature 1.0+**: More creative, diverse output (good for brainstorming, but higher hallucination risk)

**EE Analogy:** Temperature is like thermal noise in an electronic system. Higher temperature = more randomness in the output signal.

#### Hallucination (توهم)

**Hallucination** is when an LLM generates information that sounds plausible but is factually incorrect, fabricated, or nonsensical. This is the most dangerous aspect of LLMs for engineers.

**Examples of LLM hallucinations in EE contexts:**
- Citing a paper that does not exist (fabricated DOI, plausible-sounding title and authors)
- Providing an incorrect equation for a transfer function
- Inventing specifications for a component (e.g., claiming a specific op-amp has a bandwidth it does not have)
- Generating a plausible but physically impossible circuit topology

> ⚠️ **CRITICAL WARNING:** Never use AI-generated technical data in a design without independent verification from datasheets, standards, or textbook derivations.

#### Training Cutoff (محدودیت زمانی آموزش)

Every LLM has a **training cutoff date** — the date after which it has no knowledge. If you ask about a paper published after the cutoff, the model either will not know about it or will hallucinate an answer.

**Always check:** "What is your training cutoff date?" when starting important research tasks.

### 1.6 What LLMs Can and CANNOT Do

#### ✅ What LLMs CAN Do Well

| Capability | Example in EE Context |
|------------|----------------------|
| Explain concepts clearly | "Explain the Smith Chart in simple terms" |
| Summarize long documents | Summarize a 30-page IEEE paper |
| Help with English writing | Fix grammar, improve clarity, suggest academic phrasing |
| Generate code | Write MATLAB/Python scripts for signal processing |
| Brainstorm ideas | Suggest research directions for wireless power transfer |
| Convert between formats | Turn bullet points into paragraphs, or vice versa |
| Translate with context | Translate a Persian technical description into academic English |
| Compare and contrast | "What are the differences between OFDM and FBMC?" |

#### ❌ What LLMs CANNOT Do Reliably

| Limitation | Why It Matters for EE |
|------------|----------------------|
| Perform precise calculations | May make arithmetic errors, especially with complex equations |
| Guarantee correct equations | Can produce plausible but wrong transfer functions or derivations |
| Access real-time data | Cannot check current component prices or latest paper publications |
| Verify physical feasibility | May suggest circuit designs that violate physical laws |
| Replace laboratory work | Cannot run actual experiments or simulations |
| Cite reliably | Frequently invents paper titles, authors, or DOIs |
| Understand your specific context | Does not know your lab equipment, your supervisor's preferences, or your specific project |

#### The Fundamental Rule for Engineers

> **Never trust AI output for any claim that could affect safety, accuracy, or academic integrity without independent verification.**

This is not optional. This is not being overly cautious. This is professional responsibility.

---

### 📝 Worksheet 1.1: Understanding LLM Basics

**Instructions:** Answer the following questions based on Section 1. Use complete sentences.

1. In your own words, explain what a "transformer" is and why it was an improvement over previous approaches. (3–4 sentences)

2. What is the difference between a token and a word? Give an example of a technical term that might be split into multiple tokens.

3. Explain the concept of "hallucination" in AI. Why is this particularly dangerous for electrical engineers compared to, say, creative writers?

4. Your friend says: "ChatGPT knows everything because it was trained on the entire internet." Identify at least THREE things wrong with this statement.

5. You need to analyze a 100-page PDF of IEEE standards. Which model(s) would you consider and why? What factor determines whether the model can handle this task?

---

### 📝 Worksheet 1.2: Model Comparison Exercise

**Instructions:** Complete the following table based on your own research (you may use the AI tools themselves to help verify this information).

| Feature | GPT-4o | Claude 4 | Gemini 2.0 | Llama 3 | DeepSeek R1 |
|---------|--------|----------|------------|---------|-------------|
| Free access available? | | | | | |
| Can process images? | | | | | |
| Context window size | | | | | |
| Best for (your opinion) | | | | | |
| Biggest limitation | | | | | |
| Can run locally? | | | | | |

---



## Week 3–4: LLMs as Research Assistants for Electrical Engineers

### 2.1 The AI-Enhanced Research Landscape

The research process you learned in Part 1 (finding papers, reading critically, synthesizing information) has not changed — but the *tools* available to support that process have multiplied dramatically. This section introduces AI-powered research tools and teaches you to integrate them into your existing workflow.

> **Key Principle:** AI tools accelerate research; they do not replace the researcher's judgment, domain expertise, or critical thinking.

### 2.2 AI-Enhanced Search and Discovery Tools

#### Overview Comparison Table

| Tool | What It Does | Cost | Best For |
|------|--------------|------|----------|
| **Semantic Scholar** | AI-powered academic search engine | Free | Finding relevant papers, citation analysis |
| **Elicit** | AI research assistant | Freemium | Extracting claims from papers, literature mapping |
| **Consensus** | Finds scientific consensus | Freemium | Quick evidence summaries on research questions |
| **Perplexity AI** | AI search with citations | Freemium | Getting answers with source links |
| **Google Scholar + NotebookLM** | Search + AI notebook | Free | Organizing and questioning sources |
| **Connected Papers** | Visual paper graphs | Free (limited) | Discovering related work visually |
| **Research Rabbit** | Paper recommendation | Free | Building literature collections |

#### Semantic Scholar (semanticscholar.org)

**What it is:** An AI-powered search engine specifically for academic papers, developed by the Allen Institute for AI. It indexes over 200 million papers.

**Key features for EE students:**
- **TLDR summaries:** AI-generated one-sentence summaries of papers
- **Citation context:** See how a paper is cited by others (positively, negatively, as background)
- **Relevance-based recommendations:** "More like this" suggestions
- **Research feeds:** Personalized paper recommendations based on your interests
- **API access:** For programmatic literature analysis

**Example workflow for EE research:**

```
Research question: "What are the latest advances in GaN-based power converters for EV charging?"

1. Search Semantic Scholar for: "GaN power converter electric vehicle"
2. Filter by: year (2023–2026), venue (IEEE conferences/journals)
3. Use TLDR summaries to quickly scan 20–30 papers
4. Mark relevant papers → get AI recommendations for similar work
5. Check citation graphs to find seminal papers and latest follow-ups
```

#### Elicit (elicit.com)

**What it is:** An AI research assistant that helps you find papers, extract key information, and synthesize findings.

**Key features:**
- Ask research questions in natural language
- Extracts specific data from papers (methods, results, sample sizes)
- Creates comparison tables across multiple papers automatically
- Identifies methodological approaches used in a field

**Example for EE:**

> **Your question:** "What switching frequencies are used in SiC-based inverters for solar applications?"
>
> **Elicit's output:** A table showing papers, their switching frequencies, efficiency results, and methodologies — extracted automatically from the papers.

#### Consensus (consensus.app)

**What it is:** A search engine that finds and synthesizes scientific consensus on research questions.

**Best for:** Getting a quick overview of what the research community generally agrees (or disagrees) about.

**Example:**
> **Query:** "Does wide-bandgap semiconductor reduce switching losses in power converters?"
>
> **Consensus:** "Yes — 92% of relevant papers report reduced switching losses with WBG devices, with typical improvements of 30–60% compared to silicon-based solutions."

#### Perplexity AI (perplexity.ai)

**What it is:** An AI-powered answer engine that provides responses with inline citations to real sources.

**Advantages over raw ChatGPT:**
- Always provides source links
- Searches the live internet (no training cutoff problem)
- You can verify claims immediately

**Limitations:**
- Sources may not always be academic (may cite blogs, forums)
- Synthesis quality varies
- Not a replacement for proper literature review

#### Google NotebookLM (notebooklm.google.com)

**What it is:** Google's AI notebook that lets you upload documents and ask questions about them.

**Powerful use case for students:**
- Upload 5–10 key papers from your literature review
- Ask questions across all papers simultaneously
- "What methods do these papers use to measure efficiency?"
- "What are the common limitations mentioned across these papers?"
- All answers reference your uploaded sources specifically

#### Connected Papers (connectedpapers.com)

**What it is:** A visual tool that creates a graph of papers related to a seed paper, showing connections based on co-citation and bibliographic coupling.

**How to use it:**
1. Find one highly relevant paper for your research
2. Enter its title or DOI into Connected Papers
3. Explore the visual graph to find related work you might have missed
4. Identify clusters of related research

### 2.3 Using ChatGPT/Claude as Research Assistants

Beyond specialized tools, general-purpose LLMs like ChatGPT and Claude can assist your research in several ways:

#### Generating Search Keywords

**The problem:** When starting research in a new area, you may not know the correct terminology.

**Example prompt:**
```
I'm researching methods to reduce electromagnetic interference in PCB design 
for high-speed digital circuits. What search keywords and phrases should I use 
to find relevant papers on IEEE Xplore and Google Scholar? Include both common 
terms and technical synonyms.
```

**Expected AI output (example):**
- "EMI mitigation PCB layout"
- "electromagnetic compatibility high-speed digital"
- "signal integrity crosstalk reduction"
- "ground plane design EMI"
- "power delivery network noise"
- "decoupling capacitor placement optimization"

**Your job:** Verify these are real terms used in the field (they likely are, but check).

#### Understanding Unfamiliar Concepts

When you encounter a concept outside your specialization:

**Example prompt:**
```
I'm an electrical engineering student reading a paper about neuromorphic computing. 
The paper mentions "spike-timing-dependent plasticity (STDP)" extensively. 
Explain this concept in terms an EE student would understand, using analogies 
to circuits or signal processing where possible. Keep it at 200–300 words.
```

#### Explaining Complex Papers

**Example prompt:**
```
I'm going to paste the abstract and introduction of a paper about topology 
optimization for antenna design. Please:
1. Summarize the main contribution in 2–3 sentences
2. List the key assumptions the authors make
3. Identify what prior work they build on
4. Explain any jargon I might not know as a 3rd-year EE student

[paste text here]
```

#### Identifying Gaps in Literature

**Example prompt:**
```
Based on these 5 paper summaries about wireless power transfer for implantable 
medical devices, what research gaps or unanswered questions do you notice? 
What has NOT been addressed that might be worth investigating?

Paper 1: [summary]
Paper 2: [summary]
...
```

> ⚠️ **Critical note:** The AI's suggestions about "gaps" are hypotheses, not verified facts. The AI cannot know what papers exist that you haven't shown it. Always verify by searching for the "gaps" it identifies.

#### Brainstorming Research Directions

**Example prompt:**
```
I'm starting my B.Sc. thesis in power electronics. My supervisor works on 
resonant converters. I'm interested in renewable energy applications. 
Suggest 5–7 specific, feasible thesis topics that combine these areas. 
For each, indicate: the main challenge, required equipment/simulation tools, 
and whether it's primarily simulation-based or experimental.
```

### 2.4 The Verification Workflow — CRITICAL SECTION

> 🚨 **This is the most important section of this entire module.**

AI tools will confidently present incorrect information. They do not say "I'm not sure" often enough. They do not distinguish between information they "know" well (from extensive training data) and information they are essentially guessing about.

#### The Golden Rule of AI-Assisted Research

```
┌─────────────────────────────────────────────────────────┐
│  AI OUTPUT → VERIFY → TRUST                             │
│                                                         │
│  Never skip the middle step.                            │
│  "Verify" means checking against primary sources:       │
│  datasheets, textbooks, published papers, standards.    │
└─────────────────────────────────────────────────────────┘
```

#### Verification Checklist for AI-Generated Research Content

| AI Claim Type | How to Verify | Risk If Unverified |
|---------------|---------------|-------------------|
| Paper citation | Search for exact title + DOI on publisher website | Citing non-existent papers = academic fraud |
| Technical specification | Check manufacturer datasheet | Wrong specs → failed design |
| Equation or formula | Derive independently or check textbook | Wrong equation → incorrect analysis |
| Statistical claim | Find original source study | Misleading conclusions |
| Historical fact | Check multiple reliable sources | Minor credibility issue |
| Conceptual explanation | Cross-reference with textbook | Misunderstanding propagation |

#### Common Hallucination Patterns in Engineering Contexts

**Pattern 1: Fabricated Citations**
```
AI says: "According to Smith et al. (2023) in IEEE Transactions on Power 
Electronics, GaN converters achieve 99.2% efficiency at 1 MHz switching..."

Reality: This paper may not exist. The author name, journal, year, and 
claims might all be invented. ALWAYS search for the exact paper.
```

**Pattern 2: Plausible but Wrong Equations**
```
AI says: "The resonant frequency of an LLC converter is: f_r = 1/(2π√(L_r × C_r × n²))"

Reality: The n² term should not be there in the standard LLC resonant 
frequency formula. The AI produced something that "looks right" but isn't.
```

**Pattern 3: Invented Component Specifications**
```
AI says: "The TPS65281 from Texas Instruments supports up to 36V input..."

Reality: The TPS65281 might not exist, or it might exist but with different 
specs. Always verify part numbers on the manufacturer's website.
```

**Pattern 4: Outdated Information Presented as Current**
```
AI says: "The latest version of IEEE 802.11 supports up to 9.6 Gbps..."

Reality: This might have been true at the model's training cutoff, 
but newer standards may have been released since then.
```

### 2.5 Practical AI-Assisted Research Workflow

Here is a recommended workflow that integrates AI tools while maintaining academic rigor:

```
┌─────────────────────────────────────────────────┐
│ STEP 1: Define Research Question                 │
│ (Your expertise — AI cannot do this for you)     │
├─────────────────────────────────────────────────┤
│ STEP 2: Generate Keywords (AI-assisted)          │
│ Use ChatGPT/Claude to brainstorm search terms    │
│ → Verify terms exist in real papers              │
├─────────────────────────────────────────────────┤
│ STEP 3: Systematic Search (AI + Traditional)     │
│ - Semantic Scholar / Google Scholar for papers    │
│ - Connected Papers for related work              │
│ - IEEE Xplore with AI-suggested keywords         │
├─────────────────────────────────────────────────┤
│ STEP 4: Initial Screening (AI-assisted)          │
│ - Use TLDR summaries for quick filtering         │
│ - Use NotebookLM to question uploaded papers     │
│ - Use Elicit to extract data across papers       │
├─────────────────────────────────────────────────┤
│ STEP 5: Deep Reading (Human — cannot delegate)   │
│ - Read key papers yourself, fully                │
│ - Use AI to clarify unfamiliar concepts          │
│ - Take your own notes and form your own opinions │
├─────────────────────────────────────────────────┤
│ STEP 6: Synthesis (Human + AI assistance)        │
│ - Organize findings (your structure)             │
│ - Use AI to help with writing clarity            │
│ - Verify all claims against original sources     │
├─────────────────────────────────────────────────┤
│ STEP 7: Write (Human + AI editing support)       │
│ - Draft in your own words                        │
│ - Use AI for grammar/style feedback              │
│ - Ensure all citations are real and accurate     │
└─────────────────────────────────────────────────┘
```

### 📝 Worksheet 2.1: AI Research Tool Exploration

**Instructions:** Complete the following tasks using the AI tools discussed in this section.

**Task A: Tool Comparison**
Choose a topic from your EE courses (e.g., "MPPT algorithms for solar panels" or "filter design for 5G receivers"). Search for this topic using THREE different tools (e.g., Semantic Scholar, Perplexity, ChatGPT). For each tool, record:
- Number of relevant results/quality of answer
- Time taken to find useful information
- Whether sources were provided
- Any errors or irrelevant results

**Task B: Hallucination Detection**
Ask ChatGPT or Claude: "Recommend 5 recent IEEE papers about [your topic]." Then verify EACH paper:
- Does the paper actually exist? (Search the exact title)
- Are the authors correct?
- Is the year correct?
- Is the journal/conference correct?
Record your findings. How many were real? How many were fabricated?

**Task C: Keyword Generation**
Use an LLM to generate search keywords for your research topic. Then:
1. Search IEEE Xplore with the AI-suggested keywords
2. Search with your own keywords
3. Compare: which found more relevant papers?
4. Were any AI-suggested keywords incorrect or misleading?

---

### 📝 Worksheet 2.2: Building Your Personal Research Workflow

**Instructions:** Design your personal AI-assisted research workflow by filling in this template.

| Research Stage | Tool(s) I Will Use | What I Expect from AI | What I Must Do Myself |
|----------------|--------------------|-----------------------|-----------------------|
| Topic exploration | | | |
| Keyword generation | | | |
| Paper discovery | | | |
| Paper screening | | | |
| Deep reading | | | |
| Concept clarification | | | |
| Gap identification | | | |
| Writing first draft | | | |
| Revision and editing | | | |
| Citation verification | | | |

**Reflection questions:**
1. At which stages is AI most helpful for you personally?
2. At which stages must you absolutely NOT rely on AI?
3. What verification steps will you always include?

---



## Week 4–5: Using LLMs for Technical Writing Assistance

### 3.1 Overview: AI as Your Writing Coach

In Parts 2 and 3 of this course, you developed skills in academic writing — structuring papers, writing abstracts, using hedging language, and citing sources properly. AI tools can now assist you in *improving* your writing, but they should not *replace* your writing process.

**The spectrum of AI assistance for writing:**

```
FULLY ACCEPTABLE          GRAY AREA              UNACCEPTABLE
─────────────────────────────────────────────────────────────
Grammar check     │  Paraphrasing    │  AI writes entire
Spell check       │  assistance      │  sections for you
Style suggestions │  Structural      │  
Clarity feedback  │  reorganization  │  Submitting AI text
Word choice help  │  Heavy rewriting │  as your own work
Translation aid   │  of your drafts  │  
                  │                  │  No understanding
                  │                  │  of content
```

### 3.2 Grammar and Style Checking Tools

#### Comparison of Available Tools

| Tool | Best For | Cost | EE-Specific Features |
|------|----------|------|---------------------|
| **Grammarly** | Grammar, punctuation, tone | Free basic / $12/mo premium | Recognizes some technical terms |
| **LanguageTool** | Grammar, style, multilingual | Free / premium | Open-source; supports Persian |
| **ChatGPT/Claude** | Contextual grammar, style, academic tone | Free tier available | Can understand technical context |
| **QuillBot** | Paraphrasing, grammar | Free basic / premium | Good for sentence restructuring |
| **Writefull** | Academic writing specifically | Integrated with Overleaf | Trained on published papers |

#### Using ChatGPT/Claude for Grammar and Style

Unlike Grammarly (which checks rules), LLMs can understand *context* and provide *explanations* for their suggestions.

**Effective prompt for grammar/style feedback:**

```
Please review the following paragraph from my research paper about 
buck converter control. Check for:
1. Grammar errors
2. Academic tone (is it formal enough for IEEE?)
3. Clarity (are any sentences confusing?)
4. Word choice (are there better technical terms?)

Please explain WHY each change is needed, so I can learn.

[paste your paragraph]
```

**Example input:**
> "The buck converter which we designed it has a efficiency of about 94% and this is better than other converters that researchers made before."

**Expected AI feedback:**
> 1. Remove "it" after "designed" — relative clause error (common L1 Persian transfer)
> 2. Change "a efficiency" → "an efficiency" (article before vowel sound)
> 3. Change "about 94%" → "approximately 94%" (more formal)
> 4. "better than other converters that researchers made before" → "superior to previously reported designs in the literature" (more academic)
> 5. Add hedging: "This result suggests improved performance compared to..." (avoid absolute claims without full evidence)
>
> **Corrected version:** "The designed buck converter achieves an efficiency of approximately 94%, which represents an improvement over previously reported topologies in the literature."

### 3.3 Paraphrasing Assistance: When It's OK and When It Crosses the Line

#### Acceptable Uses of AI Paraphrasing

| Situation | Example | Why It's OK |
|-----------|---------|-------------|
| Rewriting YOUR OWN text for clarity | You wrote something unclear → AI suggests clearer version | You own the ideas; you're improving expression |
| Reducing self-plagiarism | Rewording your own previous submission for a new context | Common academic practice |
| Learning alternative expressions | "How else can I say 'this paper investigates'?" | Expanding your vocabulary |
| Converting informal to formal | Your notes → academic prose (but YOU refine it) | You maintain intellectual ownership |

#### Unacceptable Uses

| Situation | Why It's Wrong |
|-----------|---------------|
| Paraphrasing someone else's work to avoid citing them | This is plagiarism regardless of who paraphrases |
| Having AI rewrite an entire section you didn't draft | You cannot claim authorship |
| Using AI to paraphrase in exams or individual assessments | Violates academic integrity |
| Submitting AI paraphrased text without understanding it | Defeats the purpose of education |

#### The Test: "Can I Explain This?"

> **If you cannot explain every sentence, every claim, and every technical choice in your writing to your professor without looking at the paper — you have not written it yourself, regardless of what tools you used.**

### 3.4 Abstract Writing with AI Assistance

Writing a good abstract is one of the hardest writing tasks (as you learned in Part 2). Here's how AI can help — and where it can't.

#### Step-by-Step Process

**Step 1: Write your own rough draft first**
```
Our paper presents a new MPPT algorithm for partial shading conditions. 
We use particle swarm optimization. Results show better tracking than 
conventional P&O method. We tested in MATLAB.
```

**Step 2: Ask AI for structured feedback**
```
I've written a rough draft of my abstract for a paper about MPPT under 
partial shading. Please help me improve it by:
1. Identifying missing elements (background, gap, method, results, conclusion)
2. Suggesting more precise academic language
3. Recommending a better structure
4. Keeping it under 200 words

Do NOT rewrite it entirely — give me suggestions so I can revise it myself.

My draft: [paste above]
```

**Step 3: AI provides structural feedback**
> Your abstract is missing:
> - Background context (why is partial shading a problem?)
> - Specific results (what percentage improvement?)
> - Scope/limitations
>
> Suggested structure:
> 1. One sentence: context and problem (partial shading reduces PV output)
> 2. One sentence: gap (conventional MPPT fails under these conditions)
> 3. Two sentences: your method (PSO-based algorithm, key innovation)
> 4. Two sentences: results (efficiency improvement, comparison metrics)
> 5. One sentence: significance

**Step 4: YOU revise based on feedback**

This workflow ensures YOU do the intellectual work while AI provides editorial guidance.

### 3.5 Getting Feedback on Drafts

#### Effective Prompts for Draft Feedback

**For overall structure:**
```
Read the following Methods section of my paper. Tell me:
- Is the logical flow clear?
- Are there any gaps where a reader would be confused?
- Is anything repeated unnecessarily?
- What would an IEEE reviewer likely criticize?

[paste your Methods section]
```

**For argument strength:**
```
In my Results section, I claim that my proposed filter design has lower 
insertion loss than existing designs. Read my evidence and tell me:
- Is the evidence convincing?
- What objections might a reviewer raise?
- What additional evidence would strengthen the argument?

[paste your Results section]
```

**For language appropriateness:**
```
Is the following paragraph appropriate for IEEE Transactions on Industrial 
Electronics in terms of:
- Formality level
- Hedging language
- Active vs. passive voice balance
- Technical precision

[paste paragraph]
```

### 3.6 Improving Sentence-Level Clarity

Common problems for Persian-speaking EE students (and how AI can help):

| Common Error | Example | AI-Assisted Fix |
|--------------|---------|-----------------|
| Run-on sentences | "The converter operates at 100kHz and the efficiency is 95% and we measured this with a power analyzer and the results confirm the simulation." | Ask AI: "Break this into shorter, clearer sentences appropriate for a journal paper." |
| Article errors (a/an/the) | "We used the MOSFET in circuit" / "A results show..." | Ask AI: "Check article usage in this paragraph and explain the rules for each correction." |
| Relative clause errors | "The circuit which we designed it..." | Ask AI: "Fix the relative clause errors and explain why." |
| Informal language | "The results are pretty good" | Ask AI: "Make this sentence appropriate for an IEEE journal." |
| Verb tense confusion | Mixing past and present in Methods section | Ask AI: "Check verb tense consistency for a Methods section (should be past tense)." |

### 3.7 Translating Technical Ideas from Persian to Academic English

Many Iranian EE students think in Persian first, then translate. AI can help bridge this gap:

**Effective approach:**
```
I want to express the following idea in academic English suitable for 
an IEEE conference paper. The idea (in Persian/informal English):

"ما یک روش جدید برای کنترل اینورتر سه فاز پیشنهاد دادیم که با استفاده از 
کنترل پیش‌بین، THD خروجی را کاهش می‌دهد"

Please provide:
1. A formal English translation suitable for a journal paper
2. Alternative phrasings I could use
3. Key technical terms with their standard English equivalents
```

**Expected output:**
> 1. "This paper proposes a novel three-phase inverter control strategy employing model predictive control (MPC) to minimize output total harmonic distortion (THD)."
> 2. Alternatives:
>    - "A predictive-control-based method is presented for reducing THD in three-phase inverter output..."
>    - "We introduce an MPC-driven approach to three-phase inverter control that achieves reduced harmonic distortion..."
> 3. Key terms: کنترل پیش‌بین = Model Predictive Control (MPC); اینورتر سه فاز = three-phase inverter; THD = Total Harmonic Distortion

### 3.8 What NOT to Do: Red Lines in AI-Assisted Writing

#### ❌ Absolute Don'ts

| Action | Why It's Wrong | Potential Consequences |
|--------|---------------|----------------------|
| Having AI write your entire paper | Academic dishonesty; you learn nothing | Expulsion, grade of zero, damaged reputation |
| Submitting AI output without reading it | You may submit errors, hallucinations | Wrong technical claims in your name |
| Using AI to write exam answers | Cheating | Academic penalties |
| Not disclosing AI use when required | Violation of transparency | Trust violation |
| Pasting confidential research into free AI tools | Data privacy violation | Research compromised |

#### The Professional Standard

In your future career as an engineer, you will sign off on designs, reports, and specifications. **You are legally and ethically responsible for every word and number in documents you author**, regardless of what tools you used to create them.

Start building this professional habit now:
- Read everything before submitting
- Verify every technical claim
- Understand every sentence
- Take responsibility for the final product

---

### 📝 Worksheet 3.1: AI Writing Assistant Practice

**Instructions:** Complete the following exercises.

**Exercise A: Grammar Improvement**
Take a paragraph from your most recent written assignment (from any course). Ask an LLM to check it for grammar, style, and academic tone. Record:
1. The original paragraph
2. The AI's suggestions (with explanations)
3. Your revised version (incorporating suggestions you agree with)
4. Any suggestions you rejected and why

**Exercise B: Abstract Improvement**
Below is a poorly-written abstract. Use an LLM to get feedback (NOT a rewrite), then revise it yourself.

> "In this paper we study about solar panels. We made a new MPPT method. The method works good. We simulate it in MATLAB and the results are showing that our method is more better than P&O method. The efficiency is increased. We think this method can be used in real systems."

Write your improved version (aim for 150–200 words, proper academic structure).

**Exercise C: Translation Practice**
Write a 4–5 sentence description of your final-year project (or any EE topic you know well) in Persian. Then:
1. Translate it yourself into English (best effort)
2. Ask an LLM to translate the same Persian text
3. Compare the two translations
4. Create a final version combining the best elements of both

---



## Week 5: Using LLMs for Presentations

### 4.1 AI Tools in the Presentation Workflow

In Part 4, you learned how to structure technical presentations, design effective slides, and deliver them confidently. AI tools can enhance each stage of this process:

| Presentation Stage | How AI Can Help | What You Still Must Do |
|-------------------|-----------------|----------------------|
| Planning & outlining | Generate initial structure, suggest flow | Decide what matters, prioritize content |
| Content creation | Draft speaker notes, suggest transitions | Ensure technical accuracy |
| Visual design | Suggest slide layouts, generate simple graphics | Create precise technical diagrams yourself |
| Practice & rehearsal | Simulate Q&A, provide feedback on text | Actually practice speaking aloud |
| Refinement | Identify unclear points, suggest simplifications | Make final judgments on content |

### 4.2 Generating Presentation Outlines

**When this helps:** You have all the technical content but struggle with structuring it into a logical, engaging flow for a specific audience.

**Effective prompt:**
```
I need to create a 15-minute presentation for my undergraduate power electronics 
class about LLC resonant converters. My audience is 3rd-year EE students who 
understand basic converter topologies (buck, boost) but have never seen resonant 
converters.

Please suggest:
1. A slide-by-slide outline (aim for 12–15 slides)
2. The key point for each slide (one main idea per slide)
3. Where I should include diagrams or waveforms
4. A logical flow that builds understanding progressively
5. What to skip (too advanced for this audience)
```

**What you do with the output:**
- Evaluate whether the suggested structure matches YOUR understanding of the topic
- Adjust based on what your professor emphasized
- Add your own examples from lab work
- Remove anything you don't fully understand (never present AI suggestions you can't explain)

### 4.3 Creating Speaker Notes

**The problem:** Students often either read slides verbatim (boring) or have no notes and freeze during the presentation.

**AI-assisted approach:**
```
Here is my slide about the voltage gain characteristics of an LLC converter:
[slide content: "Voltage Gain vs. Normalized Frequency" graph, equations, 
key parameters labeled]

Write speaker notes for this slide (about 60 seconds of speaking time) that:
- Start with a transition from the previous slide (basic topology)
- Explain what the graph shows in plain language
- Highlight the key design insight (operating below/above resonance)
- End with a lead-in to the next slide (design procedure)
- Use natural spoken language (not written academic style)
```

**Important:** Adapt the speaker notes to YOUR speaking style. If the AI generates formal language and you speak casually, rewrite in your own voice.

### 4.4 Practicing Q&A with AI as Mock Audience

This is one of the most valuable uses of AI for presentation preparation. You can practice answering difficult questions without the pressure of a live audience.

**Setup prompt:**
```
I'm preparing for a conference presentation about my research on GaN-based 
wireless power transfer for IoT sensors. My presentation covers:
- System architecture
- GaN PA design at 6.78 MHz
- Rectifier design
- Measured results: 73% end-to-end efficiency at 15 cm

Please act as a critical audience member at an IEEE conference. Ask me 
challenging questions one at a time. Include:
- Questions about methodology
- Questions about comparison with existing work
- Questions that challenge my assumptions
- Questions about practical limitations
- One "hostile" question from a skeptical reviewer

After I answer each question, give me feedback on whether my answer was 
clear, complete, and convincing.
```

**Practice dialogue example:**
> **AI (as reviewer):** "You report 73% efficiency at 15 cm, but how does this compare to existing solutions at the same frequency and distance? What is the state-of-the-art you're comparing against?"
>
> **Your answer:** [practice your response]
>
> **AI feedback:** "Your answer mentioned two comparative works but didn't specify their efficiency numbers. A reviewer would want exact comparisons. Also, mention whether the comparison is fair — same power level, same coil size, etc."

### 4.5 Getting Feedback on Slide Text

**Common problems AI can identify:**
- Too much text on one slide
- Jargon that your audience won't understand
- Inconsistent notation across slides
- Missing transitions between sections
- Unclear figure captions

**Example prompt:**
```
Here is the text from slides 3–7 of my presentation. For each slide, tell me:
1. Is there too much text? (Max 6 lines per slide)
2. Will a 3rd-year EE student understand all the terms?
3. Is the logical connection between slides clear?
4. Any suggestions for better wording?

Slide 3: [text]
Slide 4: [text]
...
```

### 4.6 AI Image Generation: Possibilities and Limitations for Technical Presentations

#### Tools Available

| Tool | Type | Useful For | Limitations for EE |
|------|------|-----------|-------------------|
| DALL-E 3 (in ChatGPT) | Image generation | Conceptual illustrations, backgrounds | Cannot create accurate circuit diagrams |
| Midjourney | Image generation | Aesthetic visuals, concept art | No technical accuracy |
| Mermaid/PlantUML (via AI) | Diagram code | Flowcharts, block diagrams | Limited to supported diagram types |
| AI in PowerPoint/Canva | Slide design | Layout suggestions, design templates | Generic, not field-specific |
| TikZ (via AI) | LaTeX graphics | Circuit diagrams, plots | Requires LaTeX knowledge to verify |

#### What AI Image Tools CAN Do for EE Presentations

- Generate conceptual block diagrams (system-level)
- Create flowcharts for algorithms
- Design attractive slide backgrounds
- Generate illustrative (non-precise) diagrams for introductory slides
- Create comparison visualizations

#### What AI Image Tools CANNOT Do Reliably

- ❌ Accurate circuit schematics (wrong connections, impossible topologies)
- ❌ Precise waveform diagrams (wrong shapes, incorrect relationships)
- ❌ Correct mathematical plots (wrong axes, incorrect curves)
- ❌ PCB layouts (purely aesthetic, not functional)
- ❌ Antenna radiation patterns (incorrect physics)

> **Rule:** For any diagram where technical accuracy matters, use proper tools (LTSpice, MATLAB, KiCad, etc.) and only use AI for non-technical illustrations.

---

### 📝 Worksheet 4.1: AI-Assisted Presentation Preparation

**Instructions:** Choose a technical topic from your courses and complete the following.

**Task A:** Use an LLM to generate a presentation outline for a 10-minute presentation. Then:
1. Mark which suggestions you would keep (✓) and which you would modify or remove (✗)
2. Add at least 3 slides/points that the AI missed
3. Write a brief justification for each change

**Task B:** Write the text for one technical slide yourself. Then ask an LLM:
- "Is this too much text for a single presentation slide?"
- "Would a [target audience] understand all terms used?"
- Record the feedback and create a revised version.

**Task C:** Use the Q&A practice method (Section 4.4) to prepare for questions on your topic. Record:
1. Three questions the AI asked
2. Your answers
3. The AI's feedback on your answers
4. What you learned about gaps in your preparation

---

## Week 5–6: Ethical Framework for AI Use in Academic Settings

### 5.1 The New Academic Landscape

The arrival of powerful AI tools has created unprecedented challenges for academic integrity. This section helps you navigate these challenges with a clear ethical framework.

**The core tension:**
- AI tools can genuinely help you learn and produce better work
- AI tools can also enable cheating and prevent learning
- The difference lies in HOW you use them, not WHETHER you use them

### 5.2 University Policies on AI Use

Most universities are developing policies that fall into one of these categories:

| Policy Type | Description | Example |
|-------------|-------------|---------|
| **Prohibition** | No AI use allowed in any coursework | Rare; mostly for exams |
| **Permitted with disclosure** | AI use allowed if you declare what you used and how | Most common approach |
| **Permitted for specific tasks** | AI allowed for grammar/editing but not content generation | Common in writing courses |
| **Encouraged with guidelines** | AI use actively encouraged with specific frameworks | Forward-thinking programs |
| **Assignment-specific** | Each assignment specifies its own AI policy | Flexible approach |

> **Your responsibility:** Check your university's specific policy AND each instructor's individual policy. When in doubt, ask before using AI tools.

### 5.3 The Spectrum of AI Use: Acceptable to Unacceptable

#### Clearly Acceptable ✅

| Use Case | Why It's Acceptable | Analogy |
|----------|--------------------|---------| 
| Grammar/spell checking | Same as using a dictionary or spellchecker | Using a calculator for arithmetic |
| Clarifying a concept you're studying | Learning assistance | Asking a tutor to explain something |
| Generating search keywords | Research tool | Using a thesaurus |
| Getting feedback on YOUR draft | Editorial assistance | Peer review |
| Practicing Q&A for presentations | Preparation tool | Rehearsing with a friend |
| Translating your ideas to English | Language assistance | Using a dictionary |
| Checking if your English sounds natural | Language verification | Asking a native speaker |

#### Gray Area ⚠️ (Depends on Context and Disclosure)

| Use Case | When It Might Be OK | When It's Problematic |
|----------|---------------------|----------------------|
| Paraphrasing your own text with AI | When you disclose and understand the output | When you can't explain the result |
| Using AI to restructure your paper | When you make all content decisions | When AI determines the argument |
| Generating a first outline | When you substantially modify it | When you just fill in AI's structure |
| Having AI suggest technical approaches | When you evaluate and choose yourself | When you implement without understanding |
| Using AI to debug code | When you understand the fix | When you copy-paste without learning |

#### Clearly Unacceptable ❌

| Use Case | Why It's Unacceptable | Consequence |
|----------|----------------------|-------------|
| Having AI write your essay/paper | Academic fraud — you didn't do the work | Expulsion, zero grade |
| Using AI during closed-book exams | Cheating | Academic penalties |
| Submitting AI output as your own without disclosure | Dishonesty | Integrity violation |
| Using AI to complete assignments meant to build skills | Defeats the purpose of education | You graduate without competence |
| Fabricating data and using AI to write plausible methods | Research misconduct | Career-ending |

### 5.4 Disclosure and Transparency

#### When You Should Disclose AI Use

**Always disclose when:**
- Your institution or instructor requires it
- AI contributed to the content (not just grammar checking)
- You used AI to generate any part of a substantial deliverable
- You're uncertain whether disclosure is needed (err on the side of transparency)

**Typical disclosure format:**

```
AI Use Declaration:
- Tool(s) used: ChatGPT (GPT-4o), Grammarly
- Purpose: Grammar checking, improving sentence clarity, 
  generating initial search keywords for literature review
- Extent: AI suggestions were reviewed and selectively adopted. 
  All technical content, analysis, and conclusions are my own work.
- Verification: All citations were verified against original sources.
```

#### What Good Disclosure Looks Like

| Component | Example |
|-----------|---------|
| Which tool | "Claude 3.5 Sonnet via claude.ai" |
| What for | "Improving English grammar in Results section" |
| How much | "Sentence-level corrections only; no content generated" |
| Verification | "All technical claims verified against original papers" |

### 5.5 Academic Integrity in the AI Era

#### The Fundamental Principle

> **Academic integrity is not about which tools you use — it is about whether YOU have done the intellectual work and can take responsibility for the result.**

Consider these questions:
1. Did YOU define the research question?
2. Did YOU understand the methods and choose them deliberately?
3. Did YOU analyze the results and draw conclusions?
4. Can YOU explain and defend every part of your work?
5. Did YOU verify all facts and citations?

If you answer "yes" to all five, you have maintained integrity regardless of which productivity tools you used. If any answer is "no," there is a problem.

#### The "Professor's Office Test"

> Imagine your professor calls you to their office and asks you to explain any part of your submitted work in detail, without notes. If you cannot do this confidently, you have relied too heavily on AI (or any other external help).

### 5.6 AI-Generated Text Detection Tools

#### Available Detection Tools

| Tool | How It Works | Accuracy | Limitations |
|------|-------------|----------|-------------|
| Turnitin AI Detection | Analyzes writing patterns | ~70–85% (varies widely) | High false positive rate for non-native speakers |
| GPTZero | Perplexity and burstiness analysis | Moderate | Struggles with technical writing |
| Originality.ai | Multiple detection methods | Moderate–High | Paid service |
| ZeroGPT | Statistical analysis | Low–Moderate | Many false positives |

#### Critical Limitations of Detection Tools

**Why you should know this (for self-protection, not for cheating):**

1. **False positives for non-native speakers:** Detection tools often flag well-structured writing by non-native English speakers as "AI-generated" because it may lack the "burstiness" (variation in sentence complexity) typical of native speakers. This is a known bias.

2. **False negatives:** Simple techniques (adding personal anecdotes, deliberate errors, paraphrasing) can fool detectors. This means they are not reliable gatekeepers.

3. **Technical writing is inherently "AI-like":** Scientific writing uses standard phrases, formal structures, and consistent patterns — the same features detectors associate with AI. IEEE papers legitimately contain phrases like "In this paper, we propose..." and "The experimental results demonstrate..."

4. **The implication:** Detection tools cannot be the sole arbiter of integrity. Your ability to explain and defend your work remains the gold standard.

### 5.7 Why Understanding Matters More Than Output

#### A Thought Experiment

Consider two students:

**Student A:** Uses AI to generate a perfect literature review. Cannot explain the papers, doesn't understand the methods, can't identify which findings are relevant to their own work. Gets a good grade on the assignment.

**Student B:** Struggles to write the literature review but reads every paper, understands the methods, identifies genuine gaps, and produces a slightly less polished but deeply understood document. Gets a slightly lower grade.

**Who is better prepared for:**
- A thesis defense? → Student B
- A job interview? → Student B
- Solving novel problems in their career? → Student B
- Further research? → Student B

**The lesson:** The grade on the assignment is less important than the knowledge and skills you build by doing it. AI that "helps" you skip the learning process is actually harming your future.

#### The Engineering Responsibility

As engineers, you will eventually:
- Design systems that people depend on for safety
- Sign off on specifications and calculations
- Make decisions under uncertainty with real consequences
- Troubleshoot problems that no AI has been trained on

None of these can be delegated to AI. The skills you build now — critical thinking, deep understanding, verification habits — are what make you a competent engineer.

---

### 📝 Worksheet 5.1: Ethical Scenarios for Discussion

**Instructions:** For each scenario, discuss with your partner/group: Is this acceptable, gray area, or unacceptable? Why? What would you do differently?

**Scenario 1:** Ahmad has an IEEE paper deadline tomorrow. His English grammar is poor, so he writes the entire paper in Persian and asks ChatGPT to translate it to academic English. He then submits it as his work, checking that the translation is accurate.

**Scenario 2:** Fatima uses Elicit to find 15 relevant papers for her literature review. She reads the AI-generated summaries but doesn't read the full papers. She cites all 15 in her review, paraphrasing the AI summaries.

**Scenario 3:** Reza is debugging his VHDL code for a digital design assignment. He pastes his code into Claude and asks "why doesn't this work?" Claude identifies a timing issue and suggests a fix. Reza understands the explanation and implements the fix himself.

**Scenario 4:** Sara's professor says "no AI tools allowed for this assignment." Sara uses Grammarly (which uses AI) to check her grammar before submitting. She reasons that "Grammarly is different from ChatGPT."

**Scenario 5:** Mohammad uses ChatGPT to generate a complete MATLAB simulation of a PID controller for his control systems homework. He runs the code, gets results, writes a report around the results, and submits it. He understands PID controllers conceptually but didn't write the code himself.

**Scenario 6:** Nazanin is writing her thesis. She writes each section herself, then asks Claude: "How can I improve the clarity of this paragraph?" She implements about 50% of Claude's suggestions and discloses this in her thesis acknowledgments.

**Scenario 7:** Ali's company is developing a new power supply design. He pastes the proprietary schematic into ChatGPT and asks for optimization suggestions.

**For each scenario, write:**
1. Your ethical judgment (acceptable / gray / unacceptable)
2. Your reasoning (2–3 sentences)
3. What factors would change your judgment?
4. What the student should do instead (if unacceptable)

---



## Week 6: Limitations and Risks of LLMs for Engineers

### 6.1 Why This Section Matters Most

> **The students who will succeed in the AI era are not those who use AI the most — they are those who understand its limitations the best.**

AI companies have strong incentives to market their tools as capable and reliable. As engineers, you must approach these claims with the same skepticism you apply to any unverified specification. This section details the specific failure modes of LLMs that are particularly dangerous in engineering contexts.

### 6.2 Hallucinations in Engineering Contexts

#### Why Engineering Hallucinations Are Particularly Dangerous

In creative writing, a hallucination might produce an interesting but fictional story — harmless. In engineering, a hallucination can:

- Lead to a design that doesn't meet safety specifications
- Cause you to cite non-existent research (academic fraud, even if unintentional)
- Result in calculations that produce dangerous operating conditions
- Waste weeks of research pursuing a non-existent result
- Create liability issues in professional practice

#### Taxonomy of Engineering Hallucinations

| Type | Example | Danger Level | How to Detect |
|------|---------|-------------|---------------|
| **Fabricated citations** | "See Zhang et al., IEEE TPEL, 2024" (paper doesn't exist) | 🔴 High | Search for exact paper title/DOI |
| **Wrong equations** | Incorrect transfer function with plausible structure | 🔴 High | Derive independently; check dimensions |
| **Invented specifications** | "The LM358 has a 10 MHz bandwidth" (actual: 1 MHz) | 🔴 High | Check manufacturer datasheet |
| **Plausible but wrong explanations** | Incorrect description of how a Zener diode regulates | 🟡 Medium | Cross-reference with textbook |
| **Outdated information** | "The latest Wi-Fi standard is 802.11ax" (may be outdated) | 🟡 Medium | Check current IEEE standards |
| **Incorrect assumptions** | Assuming ideal components in a real-world analysis | 🟡 Medium | Engineering judgment |
| **Mixed-up concepts** | Confusing EMI with EMC, or MOSFET with IGBT characteristics | 🟡 Medium | Domain knowledge check |

#### Real Examples of Dangerous Hallucinations

**Example 1: Wrong Component Rating**
```
Student asks: "What is the maximum drain-source voltage of IRF540N?"
AI answers: "The IRF540N has a maximum VDS of 200V"
Actual value: VDS(max) = 100V

Consequence: If used in a design at 150V → component destruction, 
possibly fire or injury.
```

**Example 2: Incorrect Formula**
```
Student asks: "What is the formula for the 3dB bandwidth of a 
first-order RC low-pass filter?"
AI answers: "f_3dB = 1/(2πRC) × √2"

Actual: f_3dB = 1/(2πRC) — no √2 factor for first-order.
(The √2 appears in different contexts, like -3dB power relationships)

Consequence: Filter designed with wrong cutoff frequency.
```

**Example 3: Fabricated Reference**
```
Student asks: "Can you recommend papers about matrix converters 
for EV chargers?"
AI provides: "See 'High-Efficiency Matrix Converter Topology for 
Electric Vehicle Fast Charging' by Park, J. and Kim, H., published 
in IEEE Transactions on Industrial Electronics, vol. 71, no. 4, 
pp. 3421-3432, 2024."

Reality: This paper may not exist. Title, authors, volume, pages — 
all potentially fabricated. The AI generates realistic-looking 
citations from patterns in its training data.
```

### 6.3 Outdated Training Data

Every LLM has a knowledge cutoff date. This creates specific problems:

| Situation | Problem | Solution |
|-----------|---------|----------|
| New component releases | AI doesn't know about latest parts | Always check manufacturer websites |
| Updated standards | AI references old standard versions | Check IEEE/IEC current editions |
| Recent research | AI can't cite papers after cutoff | Use Semantic Scholar, Google Scholar |
| Price/availability | AI gives outdated market information | Check distributors directly |
| Software versions | AI references old tool versions/features | Check official documentation |
| Regulatory changes | AI may cite superseded regulations | Verify current regulations |

### 6.4 Lack of True Understanding of Physics and Mathematics

**This is perhaps the most subtle and dangerous limitation.**

LLMs do NOT understand physics or mathematics. They have learned *patterns of how physics and mathematics are discussed in text*. This means:

#### What This Looks Like in Practice

**The model can:** Reproduce well-known equations and standard derivations that appear frequently in textbooks.

**The model cannot:**
- Verify that an equation is dimensionally consistent
- Recognize when an assumption in a derivation is violated
- Solve truly novel problems that require physical intuition
- Detect when a mathematical result violates physical constraints
- Understand why a particular approximation is valid in one context but not another

**Concrete example:**
```
You ask: "Design an antenna for 2.4 GHz with 10 dBi gain that fits 
in a 1 cm × 1 cm area."

AI might: Provide a seemingly complete design.

Reality: This may be physically impossible given the relationship 
between antenna aperture, gain, and wavelength. The AI doesn't 
"know" it's impossible because it doesn't understand the physics — 
it just generates text that looks like antenna design discussions.
```

#### The "Confident Nonsense" Problem

LLMs are trained to generate fluent, confident text. They do not express uncertainty proportionally to their actual knowledge. A model is equally confident when:
- Explaining Ohm's law (definitely correct — massive training data)
- Describing a rare failure mode of a specific GaN transistor (possibly hallucinated)

**There is no visible difference in confidence level.** This is why YOUR domain knowledge is essential.

### 6.5 Confidentiality and Data Privacy Concerns

#### What Happens When You Paste Data into an LLM?

| Service Type | What Happens to Your Data | Risk Level |
|--------------|--------------------------|------------|
| Free ChatGPT | May be used for training; stored on servers | 🔴 High for sensitive data |
| ChatGPT Plus (with opt-out) | Not used for training if opted out; still processed | 🟡 Medium |
| Enterprise APIs | Contractual data protection; not used for training | 🟢 Lower |
| Local/self-hosted models | Data stays on your computer | 🟢 Lowest |
| Perplexity, Gemini, etc. | Varies — read privacy policy | 🟡 Varies |

#### What You Should NEVER Paste into Public LLMs

| Category | Examples | Why |
|----------|----------|-----|
| Proprietary designs | Circuit schematics, PCB layouts, firmware code | Trade secret violation |
| Unpublished research | Novel algorithms, experimental results before publication | Scooping risk |
| Confidential business data | Client specifications, NDA-protected information | Legal liability |
| Personal data | Student records, personal details of others | Privacy law violations |
| Security-sensitive information | Passwords, API keys, access credentials | Security breach |

#### Safe Alternatives

- Use enterprise versions with data protection agreements
- Run open-source models locally (Llama, Mistral) for sensitive work
- Anonymize data before using AI tools
- Use general descriptions instead of exact proprietary values
- Ask about general concepts rather than pasting specific designs

### 6.6 Bias in Training Data

LLMs reflect biases present in their training data:

| Bias Type | How It Manifests in EE Context | Example |
|-----------|-------------------------------|---------|
| **Language bias** | Better at English-language references; may miss important work in other languages | Ignoring strong Chinese or European research |
| **Recency bias** | Favors information from web-heavy recent sources | May not properly represent established fundamentals |
| **Popularity bias** | Favors well-known approaches over newer alternatives | Always suggesting PI controllers when MPC might be better |
| **Geographic bias** | More familiar with American/European standards than others | May default to FCC instead of CE regulations |
| **Publication bias** | Trained mostly on published positive results | May overstate effectiveness of methods |

### 6.7 Over-Reliance Risk: The Dependency Trap

#### Signs You're Becoming Over-Reliant on AI

- ❌ You can't start writing without AI generating a first draft
- ❌ You don't check AI calculations manually
- ❌ You feel uncomfortable working without internet/AI access
- ❌ Your understanding of topics is "one prompt deep"
- ❌ You can't explain your own work without looking at the AI conversation
- ❌ You use AI for tasks you could do faster yourself (simple calculations, basic grammar)
- ❌ You've stopped reading textbooks because "AI can explain it"

#### The Long-Term Professional Risk

```
NOW (as a student):
┌─────────────────────────────────────────────────┐
│ Over-reliance on AI → good grades (maybe)        │
│ But: shallow understanding, weak problem-solving │
└─────────────────────────────────────────────────┘
         │
         ▼
FUTURE (as an engineer):
┌─────────────────────────────────────────────────┐
│ Cannot solve novel problems                      │
│ Cannot work in secure/offline environments       │
│ Cannot verify AI output (don't know enough)      │
│ Cannot innovate (lack deep understanding)        │
│ Cannot mentor juniors (don't truly understand)   │
└─────────────────────────────────────────────────┘
```

#### Building Healthy AI Habits

| Healthy Habit | Description |
|---------------|-------------|
| "AI second" rule | Try to solve/write yourself first; use AI to improve |
| Verification always | Never accept AI output without independent check |
| Understanding check | Can you explain the AI's answer to someone else? |
| Offline capability | Periodically work without AI to test your independent skills |
| Source-first | For technical facts, check primary sources (datasheets, standards) before/after AI |

### 6.8 When NOT to Use AI

#### Absolute No-Go Situations

| Situation | Why |
|-----------|-----|
| During closed-book exams | Academic dishonesty — immediate consequence |
| For safety-critical calculations | Lives depend on verified, traceable calculations |
| When instructor explicitly prohibits it | Respect academic policies |
| For ethical/legal decisions | AI has no moral judgment or legal accountability |
| When you don't understand enough to verify | Garbage in, garbage out |

#### Situations Requiring Extra Caution

| Situation | Required Caution |
|-----------|-----------------|
| Citing sources in academic papers | Verify every single citation independently |
| Component selection for real designs | Always verify against manufacturer datasheets |
| Regulatory compliance questions | Check current official standards/regulations |
| Novel research claims | Independent verification through derivation/simulation/experiment |
| Financial or contractual decisions | Get professional human advice |

---

### 📝 Worksheet 6.1: Finding AI Failures

**Instructions:** This exercise helps you develop your ability to detect AI errors.

**Task A: The Hallucination Hunt**
Ask an LLM the following EE questions. For each answer, identify whether the response is correct, partially correct, or contains hallucinations. Verify against reliable sources.

1. "What is the maximum junction temperature of the STM32F407 microcontroller?"
2. "Explain the Barkhausen stability criterion for oscillators."
3. "What is the typical efficiency of a Class-E power amplifier at 2.4 GHz?"
4. "Recommend three IEEE papers published in 2025 about federated learning for smart grid."
5. "What is the minimum feature size of TSMC's most advanced process node?"

For each answer:
- Rate accuracy (1–5 scale)
- Identify specific errors
- Provide the correct information with source

**Task B: The Impossible Question**
Ask an LLM to design something that is physically impossible or extremely challenging (without telling it so). Document:
- What you asked
- Whether the AI recognized the impossibility
- If it provided a "design" anyway, what physical laws it violated

Suggestions:
- "Design a 100% efficient power converter" (violates thermodynamics)
- "Design a 1 cm² antenna with 30 dBi gain at 100 MHz" (aperture limitation)
- "Design an amplifier with infinite bandwidth and zero noise" (fundamental limits)

**Task C: Bias Detection**
Ask the same technical question to three different LLMs. Compare:
- Do they give the same answer?
- Do they cite the same sources?
- Do they recommend the same approaches?
- Where do they disagree? Who is right?

---



## Hands-On Activities and Exercises

### Activity 1: Compare Answers from 3 Different LLMs on an EE Topic

**Objective:** Understand that different LLMs produce different outputs, and develop the habit of seeking multiple perspectives.

**Time:** 45 minutes (in-class or homework)

**Materials needed:** Access to at least 3 different LLMs (e.g., ChatGPT, Claude, Gemini — all have free tiers)

**Instructions:**

1. Choose ONE of the following EE questions:
   - "Explain the difference between MOSFET and IGBT for high-power applications. When would you choose each?"
   - "What are the main challenges in designing a millimeter-wave 5G antenna array?"
   - "Explain model predictive control (MPC) for a three-phase inverter to a student who knows classical PID control."
   - "What causes electromagnetic interference in switch-mode power supplies, and how can it be mitigated?"

2. Ask the SAME question to 3 different LLMs (use the exact same wording).

3. Complete the comparison table:

| Criterion | LLM 1: _________ | LLM 2: _________ | LLM 3: _________ |
|-----------|-------------------|-------------------|-------------------|
| Accuracy of technical content | /5 | /5 | /5 |
| Completeness (covered all key points?) | /5 | /5 | /5 |
| Clarity of explanation | /5 | /5 | /5 |
| Appropriate for B.Sc. EE student? | /5 | /5 | /5 |
| Included equations/examples? | Yes/No | Yes/No | Yes/No |
| Any errors detected? | | | |
| Unique insight not in others? | | | |
| Response length (words) | | | |
| Overall preference rank | | | |

4. **Reflection questions:**
   - Which LLM gave the best answer and why?
   - Did any LLM make factual errors? What were they?
   - Did the LLMs contradict each other on any point? Who was right?
   - What does this exercise teach you about relying on a single AI source?

---

### Activity 2: Fact-Check AI-Generated Content About a Familiar EE Topic

**Objective:** Develop critical evaluation skills for AI output by testing AI on topics where YOU are the expert.

**Time:** 60 minutes

**Instructions:**

1. Choose a topic you studied thoroughly in a previous course (one where you are confident in your knowledge). Examples:
   - Thevenin's theorem
   - PID controller tuning
   - Shannon's channel capacity
   - Buck converter steady-state analysis
   - FFT (Fast Fourier Transform) algorithm
   - Transmission line impedance matching

2. Ask an LLM to explain this topic in detail (500+ words with equations).

3. Systematically fact-check the response:

| Element | AI's Claim | Correct? | If Wrong, What's Right? | Source |
|---------|-----------|----------|------------------------|--------|
| Definition | | ✓/✗ | | |
| Equation 1 | | ✓/✗ | | |
| Equation 2 | | ✓/✗ | | |
| Example/numbers | | ✓/✗ | | |
| Application claim | | ✓/✗ | | |
| Limitation mentioned | | ✓/✗ | | |
| Historical fact | | ✓/✗ | | |

4. **Grade the AI's response:** Give it a mark as if it were a student submission in your class. What grade would this get on an exam?

5. **Key takeaway:** If AI makes errors on topics you know well, imagine how many errors it might make on topics you DON'T know well — where you can't detect them.

---

### Activity 3: Use AI to Help Understand a Real IEEE Paper

**Objective:** Practice using AI as a learning assistant for reading complex academic papers.

**Time:** 90 minutes

**Materials:** One published IEEE paper (your instructor will provide one, or choose from recent issues of a relevant IEEE journal in your field).

**Instructions:**

1. **First pass (without AI):** Read the paper's abstract, introduction, and conclusion. Note:
   - Main contribution (in your own words)
   - Terms/concepts you don't understand
   - Methods you're not familiar with
   - Questions you have

2. **AI-assisted pass:** For each concept you didn't understand, ask an LLM:
   ```
   I'm reading an IEEE paper about [topic]. The paper mentions 
   "[specific term/concept]" in the context of [brief context]. 
   Please explain this concept in a way a 3rd-year EE student 
   would understand. Use analogies to fundamental EE concepts 
   if possible.
   ```

3. **Verification:** For each AI explanation, find at least one other source that confirms or contradicts it (textbook, another paper, lecture notes).

4. **Complete this table:**

| Unknown Concept | AI Explanation (summary) | Verified? | Additional Source Used |
|----------------|--------------------------|-----------|----------------------|
| | | ✓/✗ | |
| | | ✓/✗ | |
| | | ✓/✗ | |
| | | ✓/✗ | |
| | | ✓/✗ | |

5. **Second reading:** Re-read the paper with your new understanding. Write a 200-word summary of the paper's main contribution and significance.

6. **Reflection:** How much did AI help you understand the paper? Were there things it explained incorrectly? What parts still require human help (professor, TA, lab partner)?

---

### Activity 4: Generate and Refine Search Keywords Using AI

**Objective:** Use AI to improve your literature search strategy, then verify the results.

**Time:** 45 minutes

**Instructions:**

1. Define a research topic relevant to your current studies or thesis. Write it as a clear question:
   ```
   Example: "What machine learning methods have been applied to 
   predictive maintenance of power transformers?"
   ```

2. **Your keywords (first attempt):** Before using AI, write down 5–7 search keywords you would use for IEEE Xplore or Google Scholar.

3. **AI-generated keywords:** Ask an LLM:
   ```
   I'm searching for academic papers on: [your research question]
   
   Please suggest:
   - 10 specific search queries for IEEE Xplore
   - Alternative technical terms and synonyms
   - Related subtopics I might be missing
   - Boolean search strings that would work well
   ```

4. **Test and compare:**

| Source | Search Query | Results on IEEE Xplore | Relevant Papers Found |
|--------|-------------|----------------------|---------------------|
| My keyword 1 | | # results | # relevant |
| My keyword 2 | | # results | # relevant |
| My keyword 3 | | # results | # relevant |
| AI keyword 1 | | # results | # relevant |
| AI keyword 2 | | # results | # relevant |
| AI keyword 3 | | # results | # relevant |

5. **Analysis:**
   - Which keywords (yours or AI's) found more relevant papers?
   - Did AI suggest any terms you hadn't considered?
   - Were any AI suggestions too broad, too narrow, or incorrect?
   - What's your optimal search strategy combining both?

---

### Activity 5: Use AI to Improve a Poorly-Written Technical Paragraph

**Objective:** Learn to use AI as an editing tool while maintaining your own voice and technical accuracy.

**Time:** 30 minutes

**Instructions:**

Below are three poorly-written technical paragraphs. For EACH paragraph:
1. Identify the problems yourself first (grammar, clarity, structure, technical accuracy)
2. Ask an LLM for improvement suggestions (NOT a full rewrite)
3. Write your own improved version
4. Compare your version with the AI's suggestions

**Paragraph A (Grammar and Clarity Issues):**
> "In the this paper we are presenting a new topology of converter which is having a high efficiency that is more better than the other converters which published in previous papers. The simulation is done in MATLAB and it is showing that the efficiency improved. We used the MOSFET switches and the frequency is 100 kHz and the power is 1 kW."

**Paragraph B (Structure and Academic Tone Issues):**
> "So basically what we did was we took the regular PLL circuit and made it better. The thing is, the old PLL had a lot of jitter and that's not great for clock recovery in optical comms. Our new approach kind of uses a bang-bang phase detector but with a twist - we added a digital loop filter that adapts. Results? Pretty good actually - 0.3 ps RMS jitter which beats most of the stuff out there."

**Paragraph C (Technical Vagueness and Unsupported Claims):**
> "The proposed antenna design achieves very good performance metrics across all parameters. It has high gain, low return loss, wide bandwidth, and compact size. These characteristics make it suitable for many applications in modern communication systems. The simulated results confirm the effectiveness of our design approach."

**For each paragraph, submit:**
1. Problems you identified (before using AI)
2. AI suggestions (what the AI recommended)
3. Your improved version (combining your judgment + AI suggestions)
4. Brief note on any AI suggestions you rejected and why

---

### Activity 6: Identify Hallucinations in AI Output About Engineering

**Objective:** Build your hallucination-detection skills by analyzing AI output for specific errors.

**Time:** 60 minutes

**Instructions:**

The following passages were generated by LLMs answering EE questions. Each passage contains 2–4 errors (hallucinations, inaccuracies, or misleading claims). Your job is to find and correct them.

**Passage 1: (Power Electronics)**
> "The LLC resonant converter is widely used in server power supplies due to its ability to achieve zero-voltage switching (ZVS) across the entire load range. The resonant tank consists of a series inductor (Lr), a parallel inductor (Lm), and a resonant capacitor (Cr). The converter operates most efficiently at exactly the resonant frequency fr = 1/(2π√(Lr×Cr)), where the voltage gain is always unity regardless of load. The LLC converter was first proposed by Steigerwald in 1988 and has since become the dominant topology for 48V bus converters in data centers."

**Your task:** Identify the errors. (Hints: Is ZVS achieved across the ENTIRE load range? Is gain always unity at resonance regardless of load? Was it really 1988? Is 48V bus the dominant application?)

**Passage 2: (Communications)**
> "5G NR (New Radio) operates in two primary frequency ranges: FR1 (sub-6 GHz, specifically 450 MHz to 6 GHz) and FR2 (millimeter-wave, 24.25 GHz to 52.6 GHz). The maximum channel bandwidth in FR2 is 400 MHz, enabling peak data rates of up to 20 Gbps using 256-QAM modulation. OFDM is used exclusively for both uplink and downlink in 5G NR. The path loss in FR2 follows the standard Friis equation without additional correction factors, making coverage planning straightforward."

**Your task:** Identify the errors. (Hints: Check the maximum channel bandwidth, whether OFDM is used exclusively for uplink, and the path loss claim for mmWave.)

**Passage 3: (Control Systems)**
> "The Nyquist stability criterion states that a closed-loop system is stable if and only if the Nyquist plot of the open-loop transfer function does not encircle the point (-1, 0) in the complex plane. This criterion can only be applied to systems with rational transfer functions and requires that the open-loop system be stable. The gain margin is defined as the reciprocal of the magnitude of the open-loop transfer function at the phase crossover frequency, while the phase margin is the additional phase shift that would bring the system to instability."

**Your task:** Identify the errors. (Hints: Does Nyquist require the open-loop system to be stable? Is "does not encircle" always the stability condition? Check the exact statements of the criterion.)

**Submission format:**
For each passage:
- List each error you found
- Explain what's wrong
- Provide the correct information
- Cite your source (textbook, datasheet, standard)

---

### Activity 7: Ethical Scenario Discussions and Role-Play

**Objective:** Develop a nuanced understanding of AI ethics in engineering through group discussion.

**Time:** 45 minutes (in-class group activity)

**Format:** Groups of 3–4 students. Each group discusses 2–3 scenarios and presents their conclusions.

**Scenarios for Discussion:**

**Scenario A: The Thesis Deadline**
Your thesis submission deadline is in 48 hours. You have all the simulation results but haven't written the discussion chapter yet. You're tempted to ask AI to write the discussion based on your results and then edit it. Your supervisor hasn't explicitly prohibited AI use.

*Discussion questions:*
- What would you do?
- What are the ethical considerations?
- What practical problems might this cause?
- What if you disclosed the AI use — would that make it acceptable?

**Scenario B: The Industry Internship**
You're an intern at a power electronics company. Your manager asks you to "quickly check" whether a competitor's topology infringes on your company's patent. You want to paste the competitor's schematic into ChatGPT for analysis.

*Discussion questions:*
- What are the confidentiality concerns?
- What data protection issues arise?
- What should you do instead?
- Who should you consult?

**Scenario C: The Group Project**
In a group project, one team member has been secretly using AI to write their sections. The text is well-written but contains a subtle technical error that nobody caught until the final presentation when the professor asks a question.

*Discussion questions:*
- Who is responsible for the error?
- Should the team report the AI use?
- What could have prevented this situation?
- What's the right team policy on AI use?

**Scenario D: The Future Job Interview**
You're applying for a design engineer position. The company gives you a take-home design problem: "Design a feedback controller for a DC-DC converter with these specifications." They say you can use "any tools available to you." Does this include AI?

*Discussion questions:*
- What do you think the company's intent is?
- What's the difference between using MATLAB (a tool) and using ChatGPT (a tool)?
- How would you approach this honestly?
- What would happen if you got the job based on AI-assisted work but can't perform independently?

---



## Vocabulary Box: AI and LLM Terminology for Engineers

### Core AI/LLM Vocabulary

| English Term | Persian Equivalent (فارسی) | Definition | Example Sentence |
|-------------|---------------------------|------------|------------------|
| **Large Language Model (LLM)** | مدل زبانی بزرگ | An AI system trained on massive text data to understand and generate human language | "We used a large language model to help refine the search keywords for our literature review." |
| **Transformer** | ترنسفورمر (معماری هوش مصنوعی) | The neural network architecture underlying modern LLMs, based on self-attention | "The transformer architecture processes all input tokens in parallel, unlike earlier sequential models." |
| **Attention mechanism** | مکانیزم توجه | A component that allows the model to focus on relevant parts of the input when generating each output | "The attention mechanism enables the model to understand long-range dependencies in text." |
| **Token** | توکن | The smallest unit of text processed by an LLM (typically a word or part of a word) | "GPT-4o can process up to 128,000 tokens in a single conversation." |
| **Context window** | پنجره زمینه | The maximum amount of text (in tokens) that an LLM can process at one time | "With a 200K-token context window, Claude can analyze an entire thesis in one prompt." |
| **Hallucination** | توهم | When an LLM generates confident but factually incorrect or fabricated information | "The model hallucinated a citation — the paper it referenced does not exist." |
| **Prompt** | دستور / پرامپت | The input text or instruction given to an LLM to generate a response | "A well-crafted prompt produces more useful and focused AI output." |
| **Fine-tuning** | تنظیم دقیق | Additional training of a pre-trained model on specific data for a particular task | "SciBERT was fine-tuned on scientific papers to better understand academic text." |
| **Inference** | استنتاج | The process of generating output from a trained model (as opposed to training) | "Running inference on a local LLM requires a GPU with at least 8GB of VRAM." |
| **Training data** | داده‌های آموزشی | The large corpus of text used to train an LLM | "The quality and diversity of training data determines the model's capabilities and biases." |
| **Parameter** | پارامتر | A learnable value in the neural network (billions of these define the model's behavior) | "GPT-4 is estimated to have over one trillion parameters." |
| **Neural network** | شبکه عصبی | A computational system inspired by biological neural networks, consisting of interconnected nodes | "Deep neural networks with many layers can learn complex patterns in data." |
| **Generative AI** | هوش مصنوعی مولد | AI systems that can create new content (text, images, code, audio) | "Generative AI tools can assist with drafting text but cannot replace critical thinking." |
| **Retrieval-Augmented Generation (RAG)** | تولید تقویت‌شده با بازیابی | A technique that combines LLMs with external database search for more accurate responses | "RAG-based systems can provide citations from real documents, reducing hallucination." |
| **Embedding** | بردار تعبیه / امبدینگ | A numerical representation of text that captures semantic meaning | "Semantic search uses embeddings to find papers related by meaning, not just keywords." |
| **Temperature** | دما (پارامتر) | A parameter controlling the randomness/creativity of LLM outputs | "Setting temperature to 0 gives the most deterministic response for factual questions." |
| **Training cutoff** | تاریخ قطع آموزش | The date after which the model has no knowledge of world events | "Always check the model's training cutoff before asking about recent publications." |
| **Open-source model** | مدل متن‌باز | An LLM whose weights and/or code are publicly available | "Llama 3 is an open-source model that can be run on local hardware." |
| **Multimodal** | چندوجهی | Able to process multiple types of input (text, images, audio, video) | "GPT-4o is multimodal — it can analyze circuit diagrams uploaded as images." |
| **Prompt engineering** | مهندسی پرامپت | The skill of crafting effective inputs to get better outputs from LLMs | "Good prompt engineering includes providing context, constraints, and examples." |
| **Zero-shot / Few-shot** | بدون نمونه / با چند نمونه | Asking an LLM to perform a task without examples (zero-shot) or with a few examples (few-shot) | "In a few-shot approach, we provided three example abstracts before asking the model to improve ours." |
| **Chain of thought** | زنجیره استدلال | A prompting technique that asks the model to show its reasoning step by step | "Chain-of-thought prompting improves accuracy for mathematical and logical problems." |
| **API** | رابط برنامه‌نویسی | Application Programming Interface — a way to access LLMs programmatically | "Using the OpenAI API, we integrated GPT-4 into our automated test report generator." |
| **Benchmark** | معیار ارزیابی | A standardized test used to measure and compare LLM performance | "The MMLU benchmark tests models across 57 academic subjects including physics and engineering." |

### Extended Vocabulary: AI in Academic and Research Contexts

| English Term | Persian Equivalent | Definition | Usage Context |
|-------------|-------------------|------------|---------------|
| **AI-assisted writing** | نگارش به کمک هوش مصنوعی | Using AI tools to improve (not generate) written text | "AI-assisted writing tools helped me improve my grammar without changing my ideas." |
| **Academic integrity** | صداقت علمی | Honesty and responsibility in academic work | "Using AI without disclosure may violate academic integrity policies." |
| **Disclosure** | افشا / اعلام | Transparently declaring the use of AI tools in your work | "Full disclosure of AI tool use is required in all submitted assignments." |
| **Plagiarism** | سرقت علمی | Presenting someone else's work (or AI's work) as your own | "Submitting AI-generated text without attribution is a form of plagiarism." |
| **Verification** | راستی‌آزمایی | The process of confirming that information is accurate | "Every AI-generated citation requires manual verification before inclusion in a paper." |
| **Bias** | سوگیری | Systematic errors or unfairness in AI outputs due to training data | "AI models may exhibit bias toward solutions popular in American engineering practice." |
| **Reproducibility** | تکرارپذیری | The ability to recreate results using the same methods | "AI-generated content may not be reproducible since models update and responses vary." |
| **Data privacy** | حریم خصوصی داده‌ها | Protection of sensitive information from unauthorized access | "Data privacy concerns prevent sharing proprietary designs with public AI tools." |
| **Intellectual property** | مالکیت فکری | Legal rights over creative and technical work | "When AI generates code, intellectual property ownership can be unclear." |

### Technical Vocabulary: Using AI Tools

| English Term | Persian Equivalent | Definition | Example |
|-------------|-------------------|------------|---------|
| **Chat interface** | رابط گفتگو | The conversational UI through which users interact with LLMs | "Most students access LLMs through a chat interface like ChatGPT." |
| **System prompt** | دستور سیستمی | Hidden instructions that define an AI's behavior | "The system prompt tells the AI to act as a research assistant." |
| **Token limit** | محدودیت توکن | Maximum number of tokens for input + output combined | "If your document exceeds the token limit, you must split it into sections." |
| **Rate limiting** | محدودیت نرخ | Restrictions on how many requests you can make per time period | "The free tier has rate limiting — you can only send 10 messages per hour." |
| **Streaming** | پخش جریانی | Displaying AI output progressively as it's generated | "Streaming allows you to read the beginning of a response while the model is still generating the end." |
| **Context overflow** | سرریز زمینه | When a conversation exceeds the model's context window | "After a long conversation, context overflow causes the model to forget earlier messages." |

---

## Prompt Engineering Guide for EE Students

### Effective Prompting Principles

Writing good prompts is a skill. Better prompts produce better AI output. Here are principles specifically for engineering students:

### Principle 1: Provide Context

**Weak prompt:**
> "Explain OFDM."

**Strong prompt:**
> "Explain OFDM to a 3rd-year electrical engineering student who understands basic Fourier transforms and has taken a signals and systems course, but has never studied communication systems. Focus on the physical intuition of why OFDM helps with multipath channels. Use analogies to concepts from signals and systems where possible."

### Principle 2: Specify the Format

**Weak prompt:**
> "Tell me about power converter topologies."

**Strong prompt:**
> "Create a comparison table of the following DC-DC converter topologies: buck, boost, buck-boost, SEPIC, and Ćuk. Include columns for: voltage conversion ratio, number of components, input current (continuous/discontinuous), output current (continuous/discontinuous), typical efficiency range, and common applications. Use standard notation."

### Principle 3: Request Verification Information

**Weak prompt:**
> "What is the thermal resistance of a TO-220 package?"

**Strong prompt:**
> "What is the typical junction-to-case thermal resistance of a TO-220 package? Please specify: (1) the typical range, (2) what factors affect it, and (3) which datasheet I should check for exact values. Note any information you're uncertain about."

### Principle 4: Constrain the Output

**Weak prompt:**
> "Help me with my antenna design."

**Strong prompt:**
> "I'm designing a microstrip patch antenna for 5.8 GHz on FR-4 substrate (εr = 4.4, thickness = 1.6 mm). I need: (1) the calculated patch dimensions using the standard rectangular patch equations, (2) an explanation of each equation used, (3) expected bandwidth and gain, and (4) known limitations of this approach that I should simulate in HFSS. Show all calculations step by step."

### Principle 5: Ask for Limitations and Caveats

**Add to any technical prompt:**
> "After your response, please list: (1) any assumptions you made, (2) conditions where this answer might not apply, (3) anything you're uncertain about, and (4) what I should verify independently."

### Prompt Templates for Common EE Tasks

#### Template 1: Understanding a Paper
```
I'm reading the paper "[title]" from [journal/conference, year].
I'll paste the [section name] below.

Please help me understand by:
1. Summarizing the key point in 2-3 sentences
2. Explaining any specialized terminology
3. Identifying the main equation(s) and what each variable represents
4. Noting what prior knowledge is assumed
5. Flagging anything that seems unusual or noteworthy

[paste section]
```

#### Template 2: Improving Technical Writing
```
Please review this paragraph from my [paper type] about [topic].
My target venue is [journal/conference name].

Check for:
- Grammar errors (explain the rule for each correction)
- Academic tone (flag any informal language)
- Clarity (identify confusing sentences)
- Hedging (identify claims that need qualification)
- Technical precision (flag vague terms that should be specific)

Do NOT rewrite the entire paragraph. Give me specific, numbered 
suggestions that I can implement myself.

[paste paragraph]
```

#### Template 3: Brainstorming Research Approaches
```
I'm working on: [problem statement]

Constraints:
- Available equipment: [list]
- Software: [list]
- Timeline: [duration]
- Level: [B.Sc./M.Sc. thesis]

Please suggest 5 different approaches to this problem. For each:
- Brief description (2-3 sentences)
- Key advantage
- Main challenge or risk
- What I would need to learn
- Estimated complexity (beginner/intermediate/advanced for my level)

Note: I'll evaluate these myself — please present options, not a 
single recommendation.
```

#### Template 4: Debugging/Troubleshooting
```
I'm experiencing [problem description] in my [circuit/simulation/code].

Setup:
- [hardware/software details]
- [what I've already tried]
- [what I expected vs. what happened]

Please help me systematically troubleshoot by:
1. Listing possible causes (most likely to least likely)
2. For each cause, suggesting a specific test I can perform
3. Indicating what result would confirm or eliminate each cause
4. Suggesting what information I should gather for further diagnosis
```

---

## Assessment Guide for Part 7

### Portfolio Assessment (60% of module grade)

Students compile a portfolio throughout the module containing:

| Item | Description | Weight |
|------|-------------|--------|
| Tool Exploration Report | Written report comparing 3+ AI tools for a specific research task | 15% |
| Hallucination Analysis | Documentation of AI errors found, with corrections and sources | 15% |
| AI-Assisted Writing Sample | Before/after comparison showing AI-aided improvement of your own text | 15% |
| Ethical Reflection Essay | 800-word essay on your personal framework for AI use in engineering (must be written WITHOUT AI assistance) | 15% |

### In-Class Participation (20% of module grade)

| Activity | Description |
|----------|-------------|
| Group discussions | Active participation in ethical scenario discussions |
| Peer review | Providing feedback on classmates' AI-assisted work |
| Presentations | Short presentation on one AI tool and its EE applications |
| Live demonstrations | Showing your AI workflow to the class |

### Final Practical Exam (20% of module grade)

A supervised, in-class exercise where students:
1. Receive a short technical text with errors
2. Use an AI tool (with instructor oversight) to identify and fix the errors
3. Verify the AI's suggestions and justify their acceptance/rejection
4. Document their process, including any AI mistakes they detected

This tests the PROCESS (critical evaluation, verification) rather than the OUTPUT.

---

## Recommended Resources

### Essential Reading

| Resource | Type | Focus | Access |
|----------|------|-------|--------|
| "Attention Is All You Need" (Vaswani et al., 2017) | Paper | Original transformer architecture | arXiv (free) |
| OpenAI documentation | Website | Understanding GPT capabilities | openai.com |
| Anthropic research blog | Website | AI safety and capabilities | anthropic.com |
| IEEE AI ethics guidelines | Standard | Professional ethics framework | IEEE.org |
| Your university's AI policy | Document | Local rules and expectations | University website |

### Tools to Explore (All Have Free Tiers)

| Category | Tools |
|----------|-------|
| General LLMs | ChatGPT (free), Claude (free), Gemini (free) |
| Research-specific | Semantic Scholar, Elicit, Connected Papers, Research Rabbit |
| Writing assistance | Grammarly (free basic), LanguageTool, Writefull |
| Search + synthesis | Perplexity AI, Consensus |
| Local/private models | Ollama + Llama 3, LM Studio |

### Further Learning (Optional)

| Topic | Resource | Level |
|-------|----------|-------|
| How transformers work (visual) | "3Blue1Brown: Attention in transformers" (YouTube) | Beginner |
| Prompt engineering | "Prompt Engineering Guide" (dair-ai on GitHub) | Intermediate |
| AI ethics in engineering | IEEE Ethics in Action series | Intermediate |
| Running local LLMs | Ollama documentation | Intermediate–Advanced |
| RAG systems | LangChain documentation | Advanced (for interested students) |

---

## Module Summary and Key Takeaways

### The Five Rules of AI Use for Engineering Students

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│  1. VERIFY EVERYTHING                                                │
│     Never trust AI output without checking primary sources.          │
│                                                                      │
│  2. UNDERSTAND BEFORE USING                                          │
│     If you can't explain it yourself, you haven't learned it.        │
│                                                                      │
│  3. DISCLOSE TRANSPARENTLY                                           │
│     Always be honest about what tools you used and how.              │
│                                                                      │
│  4. MAINTAIN YOUR SKILLS                                             │
│     AI augments your abilities — ensure you still have abilities     │
│     to augment.                                                      │
│                                                                      │
│  5. PROTECT SENSITIVE DATA                                           │
│     Never paste confidential, proprietary, or personal data          │
│     into public AI tools.                                            │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### What This Module Taught You

| Before This Module | After This Module |
|-------------------|-------------------|
| "AI can do anything" | "AI is powerful but has specific, predictable failure modes" |
| "I should use AI for everything" | "I should use AI strategically for specific tasks" |
| "AI output is probably correct" | "AI output requires verification, especially for engineering" |
| "Using AI is cheating" or "Using AI is fine" | "The ethics depend on how, what, and whether you disclose" |
| "AI will replace engineers" | "AI will augment engineers who understand both AI and their domain" |

### Final Reflection

The engineers who will thrive in the coming decades are not those who avoid AI tools, nor those who blindly depend on them. They are the ones who:

- Have deep domain knowledge (the foundation that makes AI useful)
- Use AI tools efficiently (saving time on routine tasks)
- Verify AI output rigorously (catching errors before they matter)
- Maintain their independent problem-solving ability (for novel challenges)
- Act with integrity (earning trust in an age of AI-generated content)

You are being educated not just to use today's tools but to adapt to tomorrow's. The critical thinking skills, verification habits, and ethical awareness you develop in this module will remain relevant regardless of how AI evolves.

---

## Appendix A: Quick Reference Card — AI Tools for EE Students

### When to Use Which Tool

| Task | Recommended Tool | Alternative | Caution |
|------|-----------------|-------------|---------|
| Find relevant papers | Semantic Scholar | Google Scholar, Connected Papers | Verify papers exist |
| Understand a concept | ChatGPT, Claude, Gemini | YouTube, textbook | Verify accuracy |
| Improve English grammar | Grammarly, Claude | LanguageTool, ChatGPT | Read all suggestions critically |
| Generate search keywords | Any general LLM | Elicit | Test keywords actually work |
| Summarize a long paper | Claude (long context) | Gemini, NotebookLM | May miss nuances |
| Check scientific consensus | Consensus | Perplexity AI | Limited to indexed papers |
| Practice Q&A for presentation | ChatGPT, Claude | Gemini | Prepare real answers too |
| Translate Persian → Academic English | ChatGPT, Claude | DeepL + manual editing | Check technical terms |
| Explore related papers visually | Connected Papers | Research Rabbit | Only shows connected work |
| Organize and question sources | NotebookLM | Elicit | Upload actual PDFs |
| Run LLM privately (confidential data) | Ollama + Llama 3 | LM Studio, local Mistral | Lower performance than cloud |
| Debug MATLAB/Python code | ChatGPT, Claude | Gemini, DeepSeek | Verify the fix works |

### Emergency Checklist: Before Submitting AI-Assisted Work

- [ ] I have read every word of the final document
- [ ] I can explain every sentence to my professor
- [ ] All citations are verified (they exist, details are correct)
- [ ] All equations/numbers are verified against primary sources
- [ ] All technical claims are accurate to my knowledge
- [ ] I have disclosed AI use as required by my institution
- [ ] I have not pasted any confidential data into public AI tools
- [ ] The work represents MY understanding and MY ideas
- [ ] I could reproduce this work quality independently if needed
- [ ] I have learned something from the process (not just produced output)

---

## Appendix B: Common Prompts Reference Sheet for EE Students

### For Literature Review
```
"I'm researching [topic] for my [thesis/paper]. Help me identify 
the main sub-topics and research themes in this area so I can 
structure my literature search systematically."
```

### For Understanding Equations
```
"Explain the physical meaning of each term in the following equation 
from [context]. I understand [what you know] but I'm confused about 
[specific part]. Use an EE analogy if possible.

Equation: [paste equation]"
```

### For Academic Writing Improvement
```
"I'm a non-native English speaker writing for [target journal]. 
Review this paragraph for naturalness and academic appropriateness. 
For each suggestion, explain the rule so I learn for next time.

[paste paragraph]"
```

### For Presentation Preparation
```
"I'm giving a [duration] presentation about [topic] to [audience]. 
I have these key points: [list]. Suggest a logical ordering and 
identify where my audience might get confused or have questions."
```

### For Exam Preparation (Studying, Not Cheating)
```
"I'm studying [topic] for my [course name] exam. Ask me 5 
challenging questions about this topic. After I answer each one, 
tell me if I'm correct and what I might be missing."
```

---

*End of Part 7: LLMs and AI Tools for Engineering Research & Communication*

*This module is part of the Scientific and Technical English course for Electrical Engineering undergraduates. It should be updated regularly as AI tools evolve rapidly.*

*Last updated: August 2026*
*Course version: 7.1*
