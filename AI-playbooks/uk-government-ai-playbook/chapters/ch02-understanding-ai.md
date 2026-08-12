# Chapter 2: Understanding AI

## Core Idea
AI is a broad, evolving set of fields whose systems infer outputs from inputs; they vary in autonomy and adaptiveness. To use AI well you must know what it can and cannot do — the fields, the government applications, and the specific limitations (especially of generative AI).

## Frameworks Introduced
- **OECD definition of an AI system**: "a machine-based system that, for explicit or implicit objectives, infers, from the input it receives, how to generate outputs such as predictions, content, recommendations, or decisions that can influence physical or virtual environments. Different AI systems vary in their levels of autonomy and adaptiveness after deployment." Use this as the working definition when scoping what is/isn't AI.
- **Fields of AI hierarchy**: Neural networks → machine learning (ML) → deep learning (DL) → specialist fields (speech recognition, computer vision, NLP) → generative AI → agentic AI. Use it to pick the field that matches the task, and to speak precisely about what a tool is.
  - **ML**: learns from data by extracting features and learning relationships; use for pattern detection, prediction, fraud detection.
  - **Deep learning**: more complex structures for complex tasks and large data; use for advanced vision/speech/NLP. ML remains first choice for simpler tasks (less data, less compute).
  - **Generative AI**: probabilistic models that generate text, images, video; use for content generation, drafting, summarising. Strong at plausible generation, weak at facts.
  - **Agentic AI**: autonomous systems that decide and act with minimal human intervention, using tools to achieve objectives; highest abstraction, most autonomy risk.

## Key Concepts
- **AI winter**: recurring cycles of hype and progress followed by waning investment.
- **Supervised vs unsupervised learning**: labelled data with correct answers vs unlabelled data where the model finds structure itself.
- **Hallucination (confabulation)**: LLMs return the most *likely* output for an input, which may be plausible but false.
- **Model bias vs algorithmic bias**: model bias = innate deviation producing error between predicted and actual values; algorithmic bias = systematic inequality in outcomes.
- **Spectrogram**: numeric representation of speech used by speech-recognition models.
- **Embeddings**: numerical representations of text processed by ML models.

## Mental Models
- Use the **"like the internet" limitation check**: generative AI is better at creative tasks than fact retrieval — treat every output as a statistically informed guess, not a fact.
- Use **"right field, right task"**: simpler problems → simpler ML; only escalate to DL or generative AI when the task demands it.
- Use **"two-sided impacts"**: every AI application has benefits and unintended consequences; weigh both before adopting.

## Anti-patterns
- **Expecting 100% accuracy**: no AI system delivers it under all conditions; define objective measures before assessing.
- **Trusting generative AI as a domain expert**: LLMs are not domain experts — not a substitute for legal, medical or critical advice.
- **Assuming real-time data**: many LLMs lack internet access or data beyond their training set.
- **Ignoring sustainability/cost**: training your own model is usually less environmentally sound than using a suitable pre-trained model; ongoing maintenance has real cost.

## Worked Example
**Choosing the right field for a task.** A department wants to triage incoming correspondence.
- Task: classify letters into categories → **classic ML / NLP** classification (supervised learning on labelled examples). Simple, cheap, explainable enough.
- Alternative: an LLM that drafts the reply → **generative AI**, but then plan for hallucination checks, prompt filtering, and human review before anything is sent.
- Decision: start with ML classification; only add generative drafting once the classification is proven and guardrails exist. Right tool for the job (P6).

## Key Takeaways
1. Use the OECD definition to scope "is this AI?" precisely.
2. Match the field to the task: ML for prediction/patterns, DL for complex perception, generative AI for content, agentic AI only where autonomy is acceptable.
3. Know the five AI limitations (bias, data quantity/quality, accuracy, transparency, cost/sustainability) plus the five generative AI limitations (hallucination, no critical thinking, sensitive content, no domain expertise, no real-time data).
4. Treat generative AI outputs as likely-but-not-verified; test everything.

## Connects To
- **Ch 1**: grounds Principle 1 — knowing what AI is and its limitations
- **Ch 3**: feeds use-case identification and right-tool selection
- **Ch 5**: limitations → ethics themes (fairness, transparency)
- **Ch 8**: hallucination and perturbation risks are security concerns
