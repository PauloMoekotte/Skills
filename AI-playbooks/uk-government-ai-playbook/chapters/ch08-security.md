# Chapter 8: Security

## Core Idea
AI systems must be secure by design and resilient to cyber attack (Government Cyber Security Strategy, Secure by Design principles, Cyber Security Standard). AI adds unique risks — data/model poisoning, data leakage, insecure tool chains, perturbation attacks, prompt injection, hallucinations — while also amplifying generic threats like phishing and cyber attacks, and opening opportunities to improve security.

## Frameworks Introduced
- **Deployment-mode security matrix**: choose controls by how the AI is deployed.
  - **Public AI apps/web services**: can't control inputs; educate users on what data is allowed; no control over outputs; never enter official info unless published or cleared for publication.
  - **Embedded AI (e.g. Copilot, Slack GPT, plugins)**: understand the architecture and vendor mitigations; beware unverified extensions and AI transcription tools silently uploading meeting recordings.
  - **Public AI APIs**: you can intercept data, add PETs and content filters, log/audit; data still goes to the provider (e.g. OpenAI API retains prompt data ~30 days).
  - **Privately hosted models**: full control but you own security, updates, infrastructure and MLOps skills.
  - **Working with organisational data**: increases data-security risk; apply additional controls against leakage; ask where data is sent, whether it trains future models, retention, and who sees logs.
  - **Open vs closed source**: neither is inherently more secure; open source aids audit but exposing weights/training data enables tailored attacks.
- **AI risk taxonomy (2 categories × types)**:
  - **Using AI**: data/model poisoning, data leakage, insecure AI tool chain, exacerbated existing risks, perturbation attacks, prompt injection (direct/indirect), hallucinations.
  - **Adversaries using AI**: misinformation, phishing, cyber attacks, fake official correspondence.

## Key Concepts
- **Data/model poisoning**: tampered training data → incorrect/harmful output; hard to detect in fine-tuned third-party models; test outputs against known-good responses and for bias.
- **Data leakage**: model responses reveal confidential info; RAG/in-context learning preserves access controls but is susceptible to indirect prompt injection.
- **Insecure AI tool chain**: tools (e.g. Pickle serialisation) lack basic security and often run with elevated privileges; have cybersecurity approve tools; use authentication and least privilege.
- **Exacerbated existing risks**: e.g. over-privileged access exposed by AI-enhanced enterprise search — review access controls before and while deploying.
- **Perturbation attack**: stealthy input modification to get a desired response (e.g. fooling a CV system with noise); mitigate with adversarial training.
- **Prompt injection**: crafted prompts circumvent system instructions; comes in direct and indirect forms; filter prompts/outputs, log and audit; keep a human to review actions (ReAct/copilots).
- **Hallucinations**: plausible-but-false responses; generative AI cannot be trusted for facts; outputs to the public are prone to misleading (Canada case held an org liable for a hallucinating chatbot).

## Mental Models
- Use **"never assume default configs are secure"**: treat AI tools like any third-party software; apply secure-by-design even in experimentation.
- Use **"defend in depth"**: layers — PETs for leakage, content filters on prompts and outputs, network controls, validation.
- Use **"treat LLM-generated code as inherently insecure"**: never use directly in production without code review and dependency scanning.
- Use **"AI as a security amplifier"**: the tool exposes pre-existing weaknesses (access controls, credentials, data management) — fix the underlying problem.

## Anti-patterns
- **Putting public LLM chatbots on public-facing sites without assessing direct prompt-injection risk**.
- **Training/fine-tuning on data with differing user access permissions** — model cannot preserve those controls.
- **Entering official/unpublished data into public AI apps**.
- **Letting generative AI take destructive/irreversible actions automatically** (sending emails, modifying records) — require human review.
- **Uncritical reliance on AI advice**: security practitioners who over-rely on generative AI spot novel attacks less effectively.

## Worked Example
**Security checklist for an LLM chatbot on a government website.**
- Prompt injection: meta-prompt on user input, content filters trained to detect injections, choose a more robust model; accept that none fully prevents injection (LLM can't distinguish user vs system input).
- Data leakage: RAG only over data the user can access; exclude unread emails/attachments; filter in-context data; filter response links to known resources; network controls block dangerous URLs.
- Hallucination: never output facts to the public without verification; treat as risk.
- Deploy in limited/controlled conditions first (fewer users) to reduce risk.
Risk rating approach: OWASP methodology, with user harm and misinformation added as impact factors.

## Key Takeaways
1. Match security controls to deployment mode (public app, embedded, API, self-hosted, organisational data).
2. Know and mitigate the AI-specific risks: poisoning, leakage, insecure tool chain, perturbation, prompt injection, hallucinations.
3. Defend in depth: content filters, PETs, logging/auditing, network controls, least privilege.
4. Never enter unpublished official data into public AI tools; never train on data with differing access permissions.
5. Require human review of AI-initiated actions; treat LLM-generated code as insecure until reviewed; expect more phishing and cyber attacks driven by generative AI.

## Connects To
- **Ch 1**: Principle 3 — use AI securely
- **Ch 2**: generative AI limitations (hallucination) feed security risk
- **Ch 5**: safety, security and robustness ethics theme
- **Ch 7**: security principle overlaps data protection
- **Ch 9**: risk management and assurance; OWASP-style risk rating
- **Ch 10**: security scenarios playbook in case studies
