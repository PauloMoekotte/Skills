# Chapter 7: Data Protection and Privacy

## Core Idea
UK data protection law (UK GDPR + Data Protection Act 2018) applies regardless of technology. AI projects must build in data protection by design, run DPIAs, respect the ten data protection principles most relevant to AI, and involve data protection/legal/privacy professionals from the outset.

## Frameworks Introduced
- **The 10 data protection principles for AI** (UK GDPR + DPA 2018, mapped to AI): accountability, lawfulness, purpose limitation, transparency and individual rights, fairness, data minimisation, storage limitation, human oversight, accuracy, security. Use as the compliance checklist for any AI system processing personal data.
- **DPIA (Data Protection Impact Assessment) — 10-step process**:
  1. Describe the purpose of personal data processing.
  2. Assess necessity and proportionality.
  3. Identify all personal data (incl. special category), sources and flows.
  4. Identify the valid lawful basis (Art. 6; Art. 9 for special category).
  5. Identify controller/processor roles and obligations.
  6. Identify stages where AI and automated decisions impact individuals.
  7. Seek and document the views of individuals whose data is processed.
  8. Identify stages where humans are involved in decision-making.
  9. Consider potential detriment from bias or inaccuracy.
  10. Document measures, safeguards and residual risk.
  Mandatory where processing involves systematic evaluation + profiling with legal/significant effects, large-scale special-category data, large-scale systematic monitoring of public areas, or innovative technologies (ICO).

## Key Concepts
- **Purpose limitation & repurposing**: AI often reuses data for new purposes. Repurposing is legitimate only if the new purpose is "compatible" with the original — assess data-subject expectations, data type, impact on interests, and need for extra safeguards.
- **Data minimisation**: process the minimum data needed; if the same outcome is achievable with less personal data, the principle requires you to do so.
- **PETs (privacy-enhancing technologies)**: anonymisation, synthetic data, collaborative analysis without disclosing data copies.
- **Article 22 UK GDPR**: decisions based solely on automated processing with legal/similarly significant effects are prohibited; AI may support, not replace, human decision-makers.
- **Biometric/special category data**: facial images processed for identification are special category; must be overt, accurate, proportionate, fair, with a narrow "zone of recognition".
- **International transfers**: processing outside the UK raises risk; Article 46 safeguards (e.g. international data transfer agreements) needed where the regime is not adequate.

## Mental Models
- Use **"statistically informed guess, not fact"**: never treat AI outputs as factual information about individuals — be explicit about the source and inference.
- Use **"less personal data = less risk"**: justify data use via the DPIA; use de-identification (redaction, pseudonymisation, encryption) and PETs.
- Use **"consult ICO if risk stays high"**: if high risk to rights cannot be sufficiently reduced, consult the ICO before processing.

## Anti-patterns
- **Underestimating AI's interactive qualities**: AI collects new data in real time (touchscreens, audiovisual inputs) and adapts — map these flows.
- **Skipping the DPIA for innovative tech**: ICO requires DPIAs when innovative technologies process personal data.
- **Retaining data "just in case"**: unjustifiably long retention breaches storage limitation.
- **Automated decisions without meaningful human involvement**: Article 22 restricts solely-automated decisions with significant effects.

## Worked Example
**DPIA walkthrough for a facial-recognition attendance tool.**
- Purpose: verify staff identity for attendance (Art. 6 legal basis; special category due to biometrics → Art. 9 condition).
- Data map: captured face images, live camera feeds; processing within UK; retention defined.
- Human oversight: identification alerts reviewed by a human; images below match threshold promptly deleted (narrow zone of recognition).
- Bias/detriment: tested across skin tones/genders; accuracy documented.
- Transparency: clear signage and privacy notices; individuals can object/correct.
- Residual risk documented; safeguards (encryption, deletion, access controls) in place.
Outcome: DPIA signed off; system deployed with human oversight and strict deletion.

## Key Takeaways
1. Run the ten data protection principles as the compliance checklist for any AI system.
2. Do a DPIA whenever AI processes personal data — mandatory in listed scenarios; cover all life-cycle stages.
3. Map data flows including real-time collection; handle international transfers with Article 46 safeguards.
4. Apply data minimisation and PETs; treat outputs as statistically informed guesses.
5. Keep meaningful human oversight in decision-making; Article 22 restricts solely-automated significant decisions.

## Connects To
- **Ch 1**: Principle 2 — data protection compliance
- **Ch 4**: data protection provisions in procurement/PSC
- **Ch 5**: fairness, transparency and human oversight ethics map to DP principles
- **Ch 6**: data protection is the main legal issue for personal data
- **Ch 8**: security principle overlaps with the security chapter
