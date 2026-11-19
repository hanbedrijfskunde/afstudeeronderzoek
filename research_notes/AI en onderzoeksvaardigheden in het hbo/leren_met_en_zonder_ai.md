# Learning with and without generative AI: evidence on learning, critical thinking, retention, sequencing and self-assessment (2024–2026)

Evidence file for a curriculum memo (HAN, business administration). Compiled 18 November 2026.

**Claim codes used throughout**
- **(a)** Students should do research skills first without AI, then with AI.
- **(b)** AI makes weak work look convincing, so the final product says less about what a student can do.
- **(c)** Students misjudge their own AI-assisted performance.
- **(d)** Problem framing and judgment erode under uncritical AI use.

**Status labels**
- **[PR]**: peer-reviewed journal or conference paper.
- **[PREPRINT]**: arXiv, PsyArXiv or SSRN, not peer-reviewed.
- **[WP]**: working paper (NBER), not peer-reviewed.
- **[RETRACTED]**: withdrawn by the publisher.
- **[REVIEW/CONCEPTUAL]**: review or position paper.
- **[PRESS]**: press or secondary coverage.

**Verification method.** Every DOI below was resolved against Crossref (`api.crossref.org`) and/or OpenAlex. arXiv records were checked against the arXiv API, the NBER paper against nber.org, and the Lancet study against PubMed (PMID 40816301). Items I could not confirm against a primary record are marked **UNVERIFIED**.

---

## 1. What do RCTs and meta-analyses (2024–2026) find about learning outcomes when students use GenAI with and without guardrails?

### Takeaway
The strongest causal evidence shows a split between performance and learning:
- **Unrestricted GenAI** raises in-task performance and the quality of the delivered product. Unaided performance afterwards stays the same or gets worse. Examples:
  - Bastani: +48% on practice, −17% on the exam.
  - Shen & Tamkin: 50% vs 67% on a mastery quiz.
  - Fan et al.: better essays, no extra knowledge gain.
  - ALEKS data: about 25% lower odds of a correct answer on proctored items.
- **Pedagogically constrained AI tutors** avoid the harm (Bastani's "GPT Tutor") or produce large gains (Kestin et al.).
- **The positive meta-analyses are weak.** Wang & Fan (2025) was **retracted on 22 April 2026**. Deng et al. (2025) is criticised, including by its own authors, for confusing the quality of the AI output with student learning.

### Cited Findings

**Bastani, H., Bastani, O., Sungu, A., Ge, H., Kabakcı, Ö., & Mariman, R. (2025).** *Generative AI without guardrails can harm learning: Evidence from high school mathematics.* PNAS, 122(26), e2422633122. https://doi.org/10.1073/pnas.2422633122 [PR]
- **Publication:** published 25 June 2025. A **correction** appeared 20 Aug 2025: PNAS 122(34), e2518204122, https://doi.org/10.1073/pnas.2518204122. I did not check what the correction changes.
- **Design:** field experiment (RCT) with "nearly a thousand high school math students". Students got either "GPT Base" (a standard ChatGPT-like interface) or "GPT Tutor" (prompts designed to safeguard learning). [Source](https://doi.org/10.1073/pnas.2422633122)
- **Country:** Türkiye, according to press coverage of the OECD Digital Education Outlook. [PRESS: Hurriyet Daily News](https://www.hurriyetdailynews.com/oecd-warns-ai-boosts-grades-but-not-lasting-learning-218598)
- **Findings:**
  - With GPT-4 access during practice, grades improved by **48% (GPT Base)** and **127% (GPT Tutor)**.
  - When access was removed, GPT Base students did **17% worse** than students who never had access.
  - The GPT Tutor safeguards "largely mitigated" the negative effect.
  - Students used GPT-4 "as a 'crutch'". [Source](https://doi.org/10.1073/pnas.2422633122)
- **Limitations:** one country, one subject (secondary maths), GPT-4-era interface. Note that GPT Tutor *mitigated* harm; the abstract reports no learning gain over the control group.
- **Bears on:** (a) strongly; (b) strongly, since practice performance overstated what students could do alone.

**Kestin, G., Miller, K., Klales, A., Milbourne, T., & Ponti, G. (2025).** *AI tutoring outperforms in-class active learning: an RCT introducing a novel research-based design in an authentic educational setting.* Scientific Reports, 15, 17458. https://doi.org/10.1038/s41598-025-97652-6 [PR]
- **Design:** randomised crossover RCT. Each student had one lesson with the AI tutor and one in an active-learning class. Topics were surface tension and fluids, with A/B test versions.
- **Sample:** Harvard Physical Sciences 2 (introductory physics for life sciences), Fall 2023. Of 233 enrolled students, 194 were eligible. [Source (PMC full text)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/)
- **Tutor design:** a custom tutor "informed by the same pedagogical best practices as employed in the in-class lessons". It was scaffolded, not an open chatbot. [Source](https://doi.org/10.1038/s41598-025-97652-6)
- **Findings:**
  - Post-test gains were significantly larger with the AI tutor (p < 10⁻⁸).
  - Effect size was 0.63 in linear regression, which the authors call an underestimate due to a ceiling effect. Quantile regression gives **0.73–1.3 SD**.
  - Median AI lesson time was 49 minutes, against an assumed 60 minutes of in-class learning.
  - Time on task did not correlate with post-test score. [Source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/)
- **Limitations (authors):**
  - Students were meeting the material for the first time.
  - The post-test was immediate, with no delayed retention measure.
  - It was a single elite institution and a purpose-built tutor. [Source](https://pmc.ncbi.nlm.nih.gov/articles/PMC12179260/)
- **Bears on:** nuances (a). Structured AI that makes students do the thinking can beat good teaching. This argues for constrained, scaffolded AI, not for "no AI". It does not test open-ended research tasks.

**Shen, J. H., & Tamkin, A. (2026).** *How AI Impacts Skill Formation.* arXiv:2601.20245 (v2, 1 Feb 2026). https://arxiv.org/abs/2601.20245 [PREPRINT; both authors are at Anthropic, which builds AI products]
- **Design:** randomised experiment. 52 mostly junior software engineers learned a new Python library (Trio), with or without an AI assistant, then took a quiz without AI. [Source](https://www.anthropic.com/research/AI-assistance-coding-skills)
- **Findings:**
  - The AI group scored **50%** on the quiz, against **67%** for the no-AI group (Cohen's d = 0.738, p = 0.01).
  - The AI group was about 2 minutes faster, which was not significant (p = 0.391).
  - Debugging showed the largest gap. [Source](https://www.anthropic.com/research/AI-assistance-coding-skills)
  - Abstract: "AI use impairs conceptual understanding, code reading, and debugging abilities, without delivering significant efficiency gains on average"; "AI-enhanced productivity is not a shortcut to competence". [Source](https://arxiv.org/abs/2601.20245)
- **Interaction patterns:**
  - Patterns that preserved learning (average quiz ≥65%): "generation-then-comprehension", "hybrid code-explanation" and "conceptual inquiry" (asking conceptual questions while fixing one's own errors).
  - Patterns linked to poor learning (<40%): full delegation, progressive reliance, and iterative AI debugging.
  - The subgroups are tiny (n = 2–7) and the analysis is associative. [Source](https://www.anthropic.com/research/AI-assistance-coding-skills)
- **Limitations:**
  - Small sample.
  - Immediate test only.
  - Sidebar assistant, not agentic tools.
  - Industry authors.
- **Bears on:** (a), (b), (d).

**Kreijkes, P., Kewenig, V., Kuvalja, M., Lee, M., Hofman, J. M., Vitello, S., Sellen, A., Rintel, S., Goldstein, D. G., & Rothschild, D. (2026).** *Effects of LLM use and note-taking on reading comprehension and memory: A randomised experiment in secondary schools.* Computers & Education, 243, 105514. https://doi.org/10.1016/j.compedu.2025.105514 [PR] (SSRN preprint 2025: 10.2139/ssrn.5095149)
- **Design:** pre-registered randomised experiment with within- and between-participant elements.
- **Sample:** 405 students aged 14–15 in schools in England. Comprehension and retention were tested 3 days later.
- **Findings:**
  - Note-taking alone, and note-taking combined with the LLM, had significantly positive effects on retention and comprehension compared with the LLM alone.
  - Yet most students *preferred* the LLM and perceived it as *more helpful*. [Source](https://doi.org/10.1016/j.compedu.2025.105514)
- **Limitations:**
  - Secondary pupils, not higher education.
  - Reading tasks, not research tasks.
  - Short 3-day delay.
- **Bears on:**
  - (a): own processing first, or alongside, is better than LLM-only.
  - (c): preference and perceived helpfulness diverge from actual retention.

**Rismanchian, S., Uzun, H., Matayoshi, J., Cosyn, E., & Kurd-Misto, E. (2026).** *Faster Completion, Less Learning: Generative AI Reduced Study Time on Math Problems and the Knowledge They Build.* arXiv:2605.21629 (v3). https://arxiv.org/abs/2605.21629 [PREPRINT]
- **Design:** quasi-experimental. A ten-year panel of 3.2 million ALEKS learning interactions, plus ALEKS PPL placement data. It compares AI-susceptible text word problems with less susceptible interactive graph problems.
- **Findings:**
  - Among college students, learning time on AI-susceptible problems fell 2.8% per quarter after ChatGPT's release, a cumulative **26.9%** over eleven quarters.
  - The divergence "vanishes entirely under proctoring".
  - On randomly assigned **proctored** retention items, the odds of a correct answer fell **25%** cumulatively.
  - On **non-proctored** assessment, the same estimator showed a large *increase*. [Source](https://arxiv.org/abs/2605.21629)
- **Limitations:**
  - Not peer-reviewed.
  - AI use is inferred, not observed.
  - Authors appear to be affiliated with the platform; affiliation is not verified.
- **Bears on:** (b) very directly, since unsupervised scores rose while supervised knowledge fell. Also (a).

**Dickey, E., Mertzanidis, M., & Psomas, A. (2026).** *Is Solving Better Than Evaluating GenAI Solutions?* arXiv:2607.27586. https://arxiv.org/abs/2607.27586 [PREPRINT]
- **Design:** randomised A/B crossover study, N = 220, junior-level algorithms course. Groups either solved problems themselves or evaluated "often-flawed GenAI-generated solutions", swapping roles mid-semester.
- **Findings:**
  - No significant differences on midterm, final exam, course grade or aligned exam problems.
  - Homework scores were significantly higher when *evaluating* AI solutions, but "this localized advantage did not translate into downstream summative gains". [Source](https://arxiv.org/abs/2607.27586)
- **Bears on:**
  - (b): homework scores inflated without a learning gain.
  - Nuances (a): evaluating AI output did not harm exam results, but did not help either.

**Lira, B., Rogers, T., Goldstein, D. G., Ungar, L., & Duckworth, A. L. (2025).** *Coach not crutch: Evidence that AI can improve writing skill despite reducing effort.* arXiv:2502.02880 (v4). https://arxiv.org/abs/2502.02880 [PREPRINT]. Earlier circulated as "Learning not cheating…"; that title is **UNVERIFIED**.
- **Design:** several pre-registered experiments plus a survey of young adults. Task: writing professional cover letters.
- **Findings:**
  - People who practised with AI exerted less effort, "yet wrote better cover letters in no-AI writing tests".
  - AI access improved writing more than googling examples or getting feedback from human editors.
  - Simply *viewing* an AI-revised letter produced the same gain, so AI "can teach by example". [Source](https://arxiv.org/abs/2502.02880)
- **Limitations:**
  - Online participants, not students in a curriculum.
  - A narrow, genre-like writing skill.
  - Not peer-reviewed.
- **Bears on:** **contradicts a strong form of (a)** for template-like skills where worked examples help. It does not address open problem framing.

**Wecks, J. O., Voshaar, J., Plate, B. J., & Zimmermann, J. (2024).** *Generative AI Usage and Exam Performance.* SSRN. https://doi.org/10.2139/ssrn.4812513 [PREPRINT/WP]. Semantic Scholar lists a later version titled "Generative AI Usage and Academic Performance".
- **Design:** observational. GenAI users were identified with AI-detection software applied to student essays, followed by multivariate regression.
- **Findings:**
  - GenAI users scored on average **6.71 points (out of 100) lower** than non-users.
  - The effect was "particularly detrimental to students with high learning potential". [Source](https://api.semanticscholar.org/graph/v1/paper/DOI:10.2139/ssrn.4812513?fields=title,abstract)
- **Limitations:**
  - Detector-based classification is error-prone.
  - Not causal.
  - Not peer-reviewed.
  - The cohort is reportedly accounting students; country and course are **UNVERIFIED**.
- **Bears on:** (a), (b). This is the business-school-relevant evidence.

**Scarfe, P., Watcham, K., Clarke, A., & Roesch, E. (2024).** *A real-world test of artificial intelligence infiltration of a university examinations system: A "Turing Test" case study.* PLOS ONE, 19(6), e0305354. https://doi.org/10.1371/journal.pone.0305354 [PR]
- **Design:** blind field test. Fully AI-written submissions were injected into take-home exams in five undergraduate psychology modules at a UK university.
- **Findings:**
  - **94%** of AI submissions went undetected.
  - AI submissions scored "on average half a grade boundary higher" than real students.
  - There was an **83.4%** chance that AI submissions would outperform a random equal-sized set of student submissions. [Source](https://doi.org/10.1371/journal.pone.0305354)
- **Bears on:** (b) very directly. Unsupervised products no longer separate competent from AI-assisted work.

**Doshi, A. R., & Hauser, O. P. (2024).** *Generative AI enhances individual creativity but reduces the collective diversity of novel content.* Science Advances, 10(28), eadn5290. https://doi.org/10.1126/sciadv.adn5290 [PR]
- **Design:** online experiment on short-story writing.
- **Findings:**
  - Access to AI ideas made stories rated "more creative, better written, and more enjoyable, especially among less creative writers".
  - AI-enabled stories were "more similar to each other". [Source](https://doi.org/10.1126/sciadv.adn5290)
- **Bears on:** (b). AI lifts weaker producers most, which compresses visible quality differences and makes the product less diagnostic.

**Brynjolfsson, E., Li, D., & Raymond, L. (2025).** *Generative AI at Work.* Quarterly Journal of Economics, 140(2), 889–942. https://doi.org/10.1093/qje/qjae044 [PR]
- **Design:** staggered rollout of an AI assistant.
- **Sample:** 5,172 customer-support agents.
- **Findings:**
  - Productivity rose **15%** on average.
  - Less experienced and lower-skilled workers improved in speed and quality.
  - The most skilled workers saw "small declines in quality".
  - There is some evidence that AI "facilitates worker learning". [Source](https://doi.org/10.1093/qje/qjae044)
- **Bears on:** context for (b), since the skill gap shrinks in output. Partly **nuances** the learning concerns.

**Meta-analyses and their critiques**

**Wang, J., & Fan, W. (2025).** *The effect of ChatGPT on students' learning performance, learning perception, and higher-order thinking: insights from a meta-analysis.* Humanities and Social Sciences Communications, 12, 621. https://doi.org/10.1057/s41599-025-04787-y — **[RETRACTED]**
- **Retraction:** Retraction Note, HSSC 13, 528, dated **22 April 2026**: https://doi.org/10.1057/s41599-026-07310-z. Crossref and Retraction Watch both record the retraction (record 70475). [Source](https://api.crossref.org/works/10.1057/s41599-025-04787-y)
- **Original claim:** "ChatGPT has a large positive impact on improving learning performance (g = 0.867)" and a call for "broad use of ChatGPT at various grade levels". [Source (critique quoting it)](https://doi.org/10.31234/osf.io/wgu56_v2)
- **Stated reason (press summary):** the editor cited "concerns relating to discrepancies in the meta-analysis". The concerns were first raised by Ingebrigtsen and Lukic, and the authors did not respond. [PRESS: Plagiarism Today](https://www.plagiarismtoday.com/2026/07/15/study-claiming-ai-helps-students-learn-retracted/); [PRESS: GovTech](https://www.govtech.com/education/nature-retracts-oft-cited-paper-on-positive-impact-of-chatgpt)
- **Do not cite as evidence.** If it is mentioned at all, mention it only as a cautionary example.

**Ingebrigtsen, M., & Lukic, M. (2026).** *Substantial Errors Invalidate the Conclusion from Wang and Fan (2025) About ChatGPT and Learning Outcomes.* PsyArXiv. https://doi.org/10.31234/osf.io/wgu56_v2 [PREPRINT/COMMENTARY]
- The paper reports "numerous data extraction errors, inconsistent reporting and several analytical issues" and urges retraction. [Source](https://doi.org/10.31234/osf.io/wgu56_v2)
- Press reports that the critics argue the forest plot implies an effect nearer 0.5. That figure is **UNVERIFIED** against the preprint text. [PRESS](https://www.plagiarismtoday.com/2026/07/15/study-claiming-ai-helps-students-learn-retracted/)

**Jafri, B. (2026).** *The Effect That Didn't Survive: ChatGPT, Higher-Order Thinking, and Scaffolding.* SSRN abstract 7089498. https://papers.ssrn.com/sol3/papers.cfm?abstract_id=7089498 [PREPRINT]
- The re-analysis reportedly finds the higher-order-thinking effect drops to g = 0.309, 95% CI [−0.021, 0.640], with coding errors that "ran in one direction".
- These numbers come from a search summary only and are **UNVERIFIED** against the document.

**Deng, R., Jiang, M., Yu, X., Lu, Y., & Liu, S. (2025).** *Does ChatGPT enhance student learning? A systematic review and meta-analysis of experimental studies.* Computers & Education, 227, 105224. https://doi.org/10.1016/j.compedu.2024.105224 [PR]
- **Scope:** 69 experimental studies, 2022–2024. Most were at university level and many in language education.
- **Findings:** ChatGPT "improves academic performance, affective-motivational states, and higher-order thinking propensities; it reduces mental effort and has no significant effect on self-efficacy". [Source](https://doi.org/10.1016/j.compedu.2024.105224)
- **The authors' own warning** is crucial for (b). They call for distinguishing "between the quality of ChatGPT outputs and the positive effects of interventions on academic performance". They recommend complex, project-based assessments "that require skill demonstration", proctored assessments, and long-term evaluation, and they flag missing power analyses. [Source](https://doi.org/10.1016/j.compedu.2024.105224)
- The pooled effect sizes (Hedges' g) are **UNVERIFIED**: I could not access the full text, so no g values are cited here.

**Weidlich, J., Gašević, D., Drachsler, H., & Kirschner, P. (2025).** *ChatGPT in Education: An Effect in Search of a Cause.* Journal of Computer Assisted Learning, 41(5), e70105. https://doi.org/10.1111/jcal.70105 [PR, conceptual + audit]
- The authors revisit the media/methods debate, using Deng et al. as the case. They set three "non-negotiable" requirements:
  1. A precise description of the treatment.
  2. A description of what the control group did.
  3. Outcome measures that are valid indicators of durable learning.
- An audit of a subset of Deng et al.'s primary studies found "only a small minority" met all three.
- Their conclusion: "Observed gains cannot, at this time, be confidently attributed to ChatGPT, and meta-analytic effect sizes may over- or understate its benefits." [Source](https://api.semanticscholar.org/graph/v1/paper/DOI:10.1111/jcal.70105?fields=title,abstract)

**Reviews and policy**

**OECD (2026).** *OECD Digital Education Outlook 2026* (theme: exploring effective uses of generative AI in education). OECD Publishing, published 19 January 2026. https://doi.org/10.1787/062a7394-en [REVIEW/POLICY]
- The existence, date and scope are verified via Crossref.
- **UNVERIFIED wording:** press coverage summarises the core message as "AI boosts grades but not lasting learning". It reports that the OECD argues general-purpose GenAI raises task performance without necessarily producing learning gains, while purpose-built educational tools (guided questioning, hints) support more durable learning. [PRESS: Hurriyet Daily News](https://www.hurriyetdailynews.com/oecd-warns-ai-boosts-grades-but-not-lasting-learning-218598); [Blog: CAQA "Performance without learning"](https://caqa.com.au/blogs/news/performance-without-learning-what-the-oecd-digital-education-outlook-2026-means-for-vet)
- The OECD page is JavaScript-rendered, so I could not quote the report directly.

**Bauer, E., Greiff, S., Graesser, A. C., Scheiter, K., & Sailer, M. (2025).** *Looking Beyond the Hype: Understanding the Effects of AI on Learning.* Educational Psychology Review, 37(2), 45. https://doi.org/10.1007/s10648-025-10020-8 [REVIEW/CONCEPTUAL]
- The authors propose the **ISAR model**, which describes four possible effects of AI compared with learning without AI:
  - **Inversion:** over-reliance reduces cognitive engagement.
  - **Substitution:** AI replaces an existing approach with equivalent function.
  - **Augmentation:** AI adds cognitive learning support.
  - **Redefinition:** AI redefines tasks to foster deep learning.
- Effects depend on instructional implementation, students' AI literacy and teachers' skills. [Source](https://doi.org/10.1007/s10648-025-10020-8)
- This is a useful framework for the memo: "AI first" risks *inversion*.

### Inferences
- Across designs, the pattern is consistent. Measures taken *with* AI (practice grades, essays, homework, unproctored tests) go up. Measures taken *without* AI (exam, quiz, delayed or proctored retention) stay flat or go down. The evidence comes from:
  - Bastani (field RCT)
  - Shen & Tamkin (lab RCT)
  - Fan et al. (lab RCT)
  - Kreijkes et al. (school RCT)
  - Rismanchian et al. (large quasi-experiment)
  - Dickey et al. (course RCT)
  - Scarfe et al. (field test)

  This is the core empirical support for **(b)**: a product made with AI is a poor measure of unaided competence.
- Guardrails matter more than the tool itself. The two strongest pro-AI RCTs (Kestin; Bastani's GPT Tutor) used tutors designed to make students generate answers. Neither tested open-ended research or problem-framing tasks.
- The headline meta-analytic claim of a "large positive effect" should not be used. Wang & Fan is retracted, and Deng et al. is methodologically contested; its own authors warn that output quality is confounded with learning.
- Lira et al. is the main counter-evidence to a strict "never AI first" position. Where a skill is learnable from good worked examples (a cover letter), AI-assisted practice can transfer to unaided performance. The memo should frame (a) as "attempt first, then AI" for *judgment-heavy* skills, not as a ban.

### Gaps
- Pooled effect sizes for Deng et al. (2025) could not be verified, because the full text was paywalled.
- The content of the Bastani et al. PNAS correction (Aug 2025) was not checked.
- Lehmann, Cornelius & Sting, *AI Meets the Classroom: When Does ChatGPT Harm Learning?* (SSRN, https://doi.org/10.2139/ssrn.4941259) exists, but I could not retrieve its abstract. Its findings are **UNVERIFIED** and not used.
- The verbatim OECD 2026 key messages could not be retrieved from the primary source.
- I found no RCT on business-administration students doing applied research tasks (problem definition, research design, source evaluation) with and without AI.

---

## 2. What is the evidence on cognitive offloading and critical thinking?

### Takeaway
The evidence comes in three tiers:
1. **Experiments** with students: less mental effort and shallower reasoning or knowledge gain when an LLM does the information work (Stadler et al.; Fan et al.; Darvishi et al.).
2. **Large surveys:** confidence in AI is associated with less critical-thinking effort (Lee et al.) and heavy AI use with lower critical thinking (Gerlich, which is correlational and corrected).
3. **A neural preprint** (Kosmyna et al.) that is widely cited but small, not peer-reviewed and methodologically criticised.

Taken together, this supports a *risk* of offloading judgment, not proof of lasting decline in critical thinking.

### Cited Findings

**Lee, H.-P. (Hank), Sarkar, A., Tankelevitch, L., Drosos, I., Rintel, S., Banks, R., & Wilson, N. (2025).** *The Impact of Generative AI on Critical Thinking: Self-Reported Reductions in Cognitive Effort and Confidence Effects From a Survey of Knowledge Workers.* In Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems (pp. 1–22). ACM. https://doi.org/10.1145/3706598.3713778 [PR; Microsoft Research and Carnegie Mellon]
- **Design:** survey of **319 knowledge workers**, who gave **936 first-hand examples** of GenAI use at work.
- **Findings:**
  - "Higher confidence in GenAI is associated with less critical thinking, while higher self-confidence is associated with more critical thinking."
  - GenAI "shifts the nature of critical thinking toward information verification, response integration, and task stewardship". [Source](https://doi.org/10.1145/3706598.3713778)
- **Limitations:**
  - Self-reported perceptions of effort, not measured critical-thinking ability.
  - Cross-sectional.
  - Knowledge workers, not students.
- **Bears on:** (d), since judgment shifts from framing and solving to verifying. Also (c), through the role of confidence.

**Kosmyna, N., Hauptmann, E., Yuan, Y. T., Situ, J., Liao, X.-H., Beresnitzky, A. V., Braunstein, I., & Maes, P. (2025).** *Your Brain on ChatGPT: Accumulation of Cognitive Debt when Using an AI Assistant for Essay Writing Task.* arXiv:2506.08872 (v1 10 June 2025; v2 31 Dec 2025). https://arxiv.org/abs/2506.08872 [PREPRINT; MIT Media Lab]
- **Status:** no peer-reviewed version was found as of Nov 2026.
- **Design:**
  - Three groups (LLM, search engine, brain-only) wrote essays over three sessions, measured with EEG.
  - In session 4, groups switched: LLM-to-Brain and Brain-to-LLM.
  - **54 participants** took part in sessions 1–3 and **18** completed session 4. [Source](https://arxiv.org/abs/2506.08872)
- **Findings:**
  - Brain-only participants showed the strongest, most distributed brain networks; LLM users showed the weakest connectivity.
  - LLM-to-Brain participants showed "reduced alpha and beta connectivity, indicating under-engagement".
  - Brain-to-LLM participants showed "higher memory recall" and more prefrontal and occipito-parietal activation.
  - LLM users had the lowest sense of ownership and "struggled to accurately quote their own work". [Source](https://arxiv.org/abs/2506.08872)
- **Critique:** Stankovic, M., Hirche, E., Kollatzsch, S., & Doetsch, J. N. (2025). *Comment on: Your Brain on ChatGPT…* arXiv:2601.00856 (posted 29 Dec 2025), https://arxiv.org/abs/2601.00856 [PREPRINT]. Its concerns:
  - limited sample size;
  - reproducibility of the analyses;
  - EEG methodology;
  - inconsistencies in reporting;
  - limited transparency. [Source](https://arxiv.org/abs/2601.00856)
  - Press summaries add that 55 participants were reported as completing, against 54 analysed, and that the definition of "significant connections" was ambiguous. [PRESS](https://maketecheasier.com/mit-researchers-wired-eeg-sensors-onto-54-people-writing-essays-and-found-that-the-group-using-chatgpt-not-only-thought-the-least-measured-by-brain-connectivity-but-afterwards-mostly-could-not-recal/)
- The frequently quoted figure that "83% could not quote their essay" is **UNVERIFIED**: it is not in the abstract.
- **Bears on:**
  - (a): Brain-to-LLM looked better than LLM-to-Brain, but with n = 18.
  - (c), (d).
- Use only as illustrative and preliminary.

**Gerlich, M. (2025).** *AI Tools in Society: Impacts on Cognitive Offloading and the Future of Critical Thinking.* Societies, 15(1), 6. https://doi.org/10.3390/soc15010006 [PR]
- **Correction:** Societies 15(9), 252 (10 Sep 2025), "Error in Table". https://doi.org/10.3390/soc15090252
- **Design:** mixed methods, with surveys and interviews of **666 participants** of varied ages and education levels. Analysis used ANOVA and correlations.
- **Findings:**
  - There is a "significant negative correlation between frequent AI tool usage and critical thinking abilities, mediated by increased cognitive offloading".
  - Younger participants showed higher AI dependence and lower critical-thinking scores.
  - Higher education was associated with better critical thinking "regardless of AI usage". [Source](https://doi.org/10.3390/soc15010006)
- **Limitations:**
  - Cross-sectional and correlational, so no causal claim is possible.
  - Self-report measures.
  - Published correction to a table.
  - Single author.
- The commonly cited coefficients (e.g. r ≈ −0.68) are **UNVERIFIED**: MDPI blocked full-text retrieval.
- **Bears on:** (d), weakly, as correlational evidence.

**Fan, Y., Tang, L., Le, H., Shen, K., Tan, S., Zhao, Y., Shen, Y., Li, X., & Gašević, D. (2025).** *Beware of metacognitive laziness: Effects of generative artificial intelligence on learning motivation, processes, and performance.* British Journal of Educational Technology, 56(2), 489–530. https://doi.org/10.1111/bjet.13544 [PR] (online 10 Dec 2024)
- **Design:** randomised experiment with **117 university students** on a writing task. Support conditions: ChatGPT, a human expert, writing-analytics tools, or no tool. Multi-channel process data were collected.
- **Findings:**
  - No difference in intrinsic motivation.
  - Self-regulated learning processes differed.
  - The ChatGPT group "outperformed in the essay score improvement but their knowledge gain and transfer were not significantly different".
  - ChatGPT "may promote learners' dependence on technology and potentially trigger 'metacognitive laziness'". [Source](https://doi.org/10.1111/bjet.13544)
- **Limitations:**
  - Single short session.
  - One writing task.
  - Country is **UNVERIFIED**; the lead author is based in China.
- **Bears on:** (b) strongly, since a better product came without more knowledge. Also (d) and (c).

**Stadler, M., Bannert, M., & Sailer, M. (2024).** *Cognitive ease at a cost: LLMs reduce mental effort but compromise depth in student scientific inquiry.* Computers in Human Behavior, 160, 108386. https://doi.org/10.1016/j.chb.2024.108386 [PR]
- **Design:** randomised experiment. **91 university students** used ChatGPT-3.5 or Google to research a socio-scientific issue (nanoparticles in sunscreen) and wrote recommendations with justifications.
- **Findings:**
  - The LLM group had "significantly lower cognitive load" but "lower-quality reasoning and argumentation".
  - Homogeneity of recommendations did not differ. [Source](https://doi.org/10.1016/j.chb.2024.108386)
- **Limitations:**
  - Single session.
  - GPT-3.5.
  - Country not verified.
- **Bears on:** (d) and (a). This is the closest analogue to a *research-skills* task.

**Darvishi, A., Khosravi, H., Sadiq, S., Gašević, D., & Siemens, G. (2024).** *Impact of AI assistance on student agency.* Computers & Education, 210, 104967. https://doi.org/10.1016/j.compedu.2023.104967 [PR]
- **Design:** randomised controlled experiment with **1,625 students across 10 courses**, in peer-feedback writing.
- **Procedure:** four weeks with AI prompts, then four weeks in four conditions: AI prompts, none, self-monitoring checklists, or both.
- **Findings:**
  - "Students tended to rely on rather than learn from AI assistance."
  - When AI was removed, self-regulation checklists partly filled the gap but were less effective.
  - The hybrid of AI plus checklists was not better than AI alone. [Source](https://doi.org/10.1016/j.compedu.2023.104967)
- **Bears on:** (a), (d). It also shows removal effects, see section 3.

**Zhai, C., Wibowo, S., & Li, L. D. (2024).** *The effects of over-reliance on AI dialogue systems on students' cognitive abilities: a systematic review.* Smart Learning Environments, 11, 28. https://doi.org/10.1186/s40561-024-00316-7 [PR, REVIEW]
- **Design:** PRISMA review of only **14 articles**.
- **Findings:** over-reliance affects decision-making, critical thinking and analytical reasoning, because users "favor fast and optimal solutions over slow ones". [Source](https://doi.org/10.1186/s40561-024-00316-7)
- **Limitations:** small, heterogeneous evidence base.
- **Bears on:** (d).

**Dell'Acqua, F., McFowland, E., Mollick, E., Lifshitz, H., Kellogg, K. C., Rajendran, S., Krayer, L., Candelon, F., & Lakhani, K. R. (2026).** *Navigating the Jagged Technological Frontier: Field Experimental Evidence of the Effects of Artificial Intelligence on Knowledge Worker Productivity and Quality.* Organization Science, 37(2), 403–423. https://doi.org/10.1287/orsc.2025.21838 [PR] (HBS working paper 2023, SSRN 4573321)
- **Design:** pre-registered field experiment with **758 BCG consultants**, using realistic consulting tasks.
- **Findings:**
  - For 18 tasks inside AI's capability "frontier", AI users completed 12.2% more tasks, 25.1% faster, at higher quality.
  - For a complex managerial task outside the frontier, AI users were "19% less likely to produce correct solutions". [Source](https://doi.org/10.1287/orsc.2025.21838)
- **Bears on:** (d). Business-relevant evidence that AI can degrade judgment on problems where the tool is confidently wrong. Also (b), since quality looks higher where AI is competent.

**Tankelevitch, L., Kewenig, V., Simkute, A., Scott, A. E., Sarkar, A., Sellen, A., & Rintel, S. (2024).** *The Metacognitive Demands and Opportunities of Generative AI.* CHI '24 Proceedings (pp. 1–24). https://doi.org/10.1145/3613904.3642902 [PR, CONCEPTUAL]
- GenAI imposes high metacognitive demands (monitoring and control) when prompting, evaluating and relying on outputs. [Source](https://doi.org/10.1145/3613904.3642902)
- **Bears on:** (c), (d). Novices who lack domain knowledge have least capacity to meet these demands.

### Inferences
- The best *experimental* student evidence (Stadler; Fan; Darvishi) shows **less effort and shallower processing in the moment**, with no knowledge gain or with weaker reasoning.
- The *survey* evidence (Lee; Gerlich) links confidence in AI and frequent use with less critical-thinking effort, but cannot establish causation.
- The memo should phrase (d) as "uncritical use shifts students from framing and reasoning to accepting and assembling AI output". It should not say "AI damages the brain".
- Kosmyna et al. should be cited only with explicit caveats: preprint, n = 54 (18 in session 4), and an open methodological critique.
- Dell'Acqua et al. adds a business-school angle. Where AI is plausibly but wrongly competent, judgment fails, and users cannot tell where the frontier lies.

### Gaps
- No longitudinal study measures students' *problem-framing* ability (as distinct from essay quality or recall) before and after sustained AI use.
- The Gerlich correlation coefficients and the critical-thinking instrument used could not be verified from the full text.
- I found no confirmed peer-reviewed version of Kosmyna et al. as of Nov 2026.

---

## 3. Is there evidence on retention and skill loss when AI is removed ("deskilling")?

### Takeaway
Yes, and it is growing:
- **Education:** removal or delayed-test designs consistently show lower unaided performance after unrestricted AI use (Bastani; Barcaui; Darvishi; Kreijkes; Rismanchian; Shen & Tamkin).
- **Professional settings:**
  - Endoscopists' unaided adenoma detection fell after AI exposure (observational, Lancet Gastroenterol Hepatol 2025).
  - In Autor et al.'s 2026 RCT, AI improved everyone's drafts. Lasting unaided skill gains, however, went only to **senior** patent lawyers; **juniors** showed no average gain and a split into good and poor performers.
- **Implication:** foundational expertise looks like a precondition for learning from AI.

### Cited Findings

**Autor, D., Rodchenko, T., Martin, J., Iscenko, Z., Strand, S., Pearl, D., & Ferere, M. (2026).** *Does AI Assistance Enhance or Erode Expertise? Evidence from a Three-Month Field Experiment in Patent Drafting.* NBER Working Paper No. 35720. https://doi.org/10.3386/w35720 | https://www.nber.org/papers/w35720 [WP, not peer-reviewed]
- **Publication:** issued Sept 2026, revised Oct 2026. Correction to the brief: the study concerns *patent lawyers*, not "junior attorneys" in general.
- **Design:** pre-registered three-month RCT with blinded expert scoring. **133 practising patent lawyers** at **11 US IP law firms**. [Source](https://www.nber.org/papers/w35720)
- **Findings:**
  - With AI, the quality of benchmark drafting tasks rose by **0.34 SD at 10 days** and **0.38 SD at 90 days**, with larger gains for juniors.
  - On an **unaided** redlining test after three months, treated lawyers outperformed controls by **0.32 SD**. This was concentrated among **seniors (0.45 SD)**.
  - **Juniors showed no average gain.** Their scores "bifurcated": fewer mediocre scores, more poor and more good ones.
  - Authors' conclusion: "Foundational expertise may be a prerequisite for extracting durable skill from AI-assisted practice." [Source](https://www.nber.org/papers/w35720)
- **Conflicts of interest:** conducted and funded by Google, which built the tool; several authors are Google employees or contractors. [Source](https://www.nber.org/papers/w35720)
- **Related coverage:** Google Research blog post, "Does better work always mean better workers?" https://research.google/blog/does-better-work-always-mean-better-workers/ [PRESS/industry]
- **Autor's reported advice** is that novices should frame the argument unassisted first and then use AI as a critic. This comes from secondary summaries only and is **UNVERIFIED** as a direct quote. [PRESS: AI Weekly](https://aiweekly.co/alerts/autor-nber-trial-ai-lifts-patent-lawyers-splits-juniors); [PRESS: Fortune](https://fortune.com/2026/10/10/david-autor-china-shock-nber-google-paper-illusion-of-competence-gen-z/)
- **Bears on:**
  - (a) strongly: expertise first, then AI.
  - (b): AI-assisted drafts overstated junior skill.
  - (d).

**Budzyń, K., Romańczyk, M., Kitala, D., Kołodziej, P., Bugajski, M., Adami, H. O., Blom, J., Buszkiewicz, M., Halvorsen, N., Hassan, C., Romańczyk, T., Holme, Ø., Jarus, K., Fielding, S., Kunar, M., Pellise, M., Pilonis, N., Kamiński, M. F., Kalager, M., Bretthauer, M., & Mori, Y. (2025).** *Endoscopist deskilling risk after exposure to artificial intelligence in colonoscopy: a multicentre, observational study.* The Lancet Gastroenterology & Hepatology, 10(10), 896–903. https://doi.org/10.1016/S2468-1253(25)00133-5 [PR]
- **Publication:** epub 12 Aug 2025; PMID 40816301.
- **Erratum:** Lancet Gastroenterol Hepatol 10(11), e12. https://doi.org/10.1016/S2468-1253(25)00294-8
- **Letters (Dec 2025):** from Lam; Levartovsky & Kopylov; and van de Sande, Sleijfer, Buijsman & Gommers; plus an authors' reply (PMIDs 41205614–41205617). I did not review their content.
- **Design:** retrospective observational before/after study at **4 endoscopy centres in Poland** taking part in the ACCEPT trial. It compares non-AI colonoscopies in the 3 months before and the 3 months after AI introduction. [Source (PubMed)](https://pubmed.ncbi.nlm.nih.gov/40816301/)
- **Findings:**
  - 1,443 non-AI colonoscopies were analysed: 795 before and 648 after.
  - Adenoma detection rate (ADR) fell from **28.4% (226/795) to 22.4% (145/648)**, an absolute difference of **−6.0% (95% CI −10.5 to −1.6; p = 0.0089)**.
  - In multivariable analysis, AI exposure had an OR of **0.69 (0.53–0.89)**.
  - Authors' interpretation: continuous AI exposure "might reduce the ADR of standard non-AI assisted colonoscopy". [Source (PubMed)](https://pubmed.ncbi.nlm.nih.gov/40816301/)
- **Limitations:**
  - Observational before/after design with a short window.
  - Possible confounders (fatigue, case mix, workload).
  - Several authors report industry fees.
  - The number of endoscopists (often reported as 19) is **UNVERIFIED** here.
- **Caution:** a 2026 scoping review mislabels this study as a "multicenter randomized trial". Heudel, P. E., et al. (2026), ESMO Real World Data and Digital Oncology, 12, 100693, https://doi.org/10.1016/j.esmorw.2026.100693. The same review reports ADR with AI as 25.3%. Use the primary paper. [Source (PubMed record of review)](https://pubmed.ncbi.nlm.nih.gov/41890350/)
- **Bears on:** analogical support for (a) and (d). Experienced professionals lose unaided vigilance after AI exposure.

**Barcaui, A. (2025).** *ChatGPT as a cognitive crutch: Evidence from a randomized controlled trial on knowledge retention.* Social Sciences & Humanities Open, 12, 102287. https://doi.org/10.1016/j.ssaho.2025.102287 [PR] (SSRN preprint: 10.2139/ssrn.5353041)
- **Design:** RCT, **n = 120 undergraduates** learning about AI. One group studied with ChatGPT, the other with traditional methods. A **surprise retention test came 45 days later**.
- **Findings:** the ChatGPT group scored **57.5%** against **68.5%** for traditional study; t(83) = −3.19, p = .002, **Cohen's d = 0.68**. [Source](https://doi.org/10.1016/j.ssaho.2025.102287)
- **Limitations:**
  - df = 83 implies roughly 85 analysed of 120, so attrition was likely.
  - Single author.
  - Country is **UNVERIFIED**.
- **Bears on:** (a).

**Removal and delayed-test results reported in section 1** (repeated here for completeness):
- Bastani et al.: −17% on the unaided exam after GPT Base. [Source](https://doi.org/10.1073/pnas.2422633122)
- Darvishi et al.: students relied on AI rather than learning from it, and a gap appeared when it was removed. [Source](https://doi.org/10.1016/j.compedu.2023.104967)
- Kreijkes et al.: LLM-only gave lower comprehension and retention after 3 days than note-taking. [Source](https://doi.org/10.1016/j.compedu.2025.105514)
- Rismanchian et al.: about a 25% decline in odds of a correct answer on proctored retention items. [Source](https://arxiv.org/abs/2605.21629)
- Kosmyna et al.: LLM-to-Brain participants were "under-engaged" when AI was removed. [Source](https://arxiv.org/abs/2506.08872)

### Inferences
- The professional evidence points the same way as the education RCTs: practice with AI does not automatically build unaided skill. Autor et al. adds a key moderator: **prior expertise**. Seniors converted AI-assisted practice into lasting skill; juniors, who most resemble students, did not on average.
- This is arguably the strongest current support for sequencing claim (a): build the foundation first, then use AI. The caveats are that it is a Google-funded working paper on patent lawyers, not students.
- The endoscopy study shows that even trained experts lose unaided vigilance after a few months of AI support. That is a reason to keep periodic unaided performance in the curriculum, not only at the start.

### Gaps
- No study was found that measures *research-skill* retention (e.g. formulating a research question, choosing methods) in higher-education students after AI is removed.
- Autor et al. is not yet peer-reviewed. The content of the Lancet letters and the authors' reply was not reviewed.

---

## 4. What does learning science say about sequencing, and have "attempt first, then AI" designs been tested with GenAI?

### Takeaway
- **Classic learning science supports "struggle first, then support":**
  - productive failure: problem solving before instruction beats instruction first, g = 0.36, rising to 0.37–0.58 with high-fidelity designs;
  - the generation effect;
  - desirable difficulties.
- **Direct GenAI tests are few but mostly consistent:**
  - Kumar et al.: LLM explanations helped most when learners attempted first.
  - Kosmyna et al. (preprint): Brain-to-LLM looked better than LLM-to-Brain.
  - Autor et al.: expertise before AI.
  - Shen & Tamkin: "generation-then-comprehension" and conceptual-inquiry patterns preserved learning.
- **Caveats:** Lira et al. show AI-first practice can transfer for template-like writing. Kumar found benefits even for explanation-first.

### Cited Findings

**Background learning science (pre-2024; cited briefly)**

**Sinha, T., & Kapur, M. (2021).** *When Problem Solving Followed by Instruction Works: Evidence for Productive Failure.* Review of Educational Research, 91(5), 761–798. https://doi.org/10.3102/00346543211019105 [PR, META-ANALYSIS]
- **Scope:** 53 studies with 166 comparisons.
- **Findings:**
  - Problem solving followed by instruction (PS-I) beat instruction followed by problem solving (I-PS): **Hedges' g = 0.36 [0.20; 0.51]**.
  - With high fidelity to productive-failure principles, g ranged **0.37–0.58**.
  - After correcting for publication bias, the estimated true effect was g = 0.87.
  - **Boundary conditions:** effects favoured I-PS for young learners (grades 2–5) and for *domain-general* skills. [Source](https://doi.org/10.3102/00346543211019105)
- **Bears on:** (a). Note the boundary condition: research skills are partly domain-general, which tempers the claim.

**Bertsch, S., Pesta, B. J., Wiscott, R., & McDaniel, M. A. (2007).** *The generation effect: A meta-analytic review.* Memory & Cognition, 35(2), 201–210. https://doi.org/10.3758/BF03193441 [PR, META-ANALYSIS]
- Generating information yields better memory than reading it. The pooled effect size is **UNVERIFIED** here, because no abstract was retrievable. [Source](https://doi.org/10.3758/BF03193441)

**Bjork, R. A., & Bjork, E. L. (2020).** *Desirable difficulties in theory and practice.* Journal of Applied Research in Memory and Cognition, 9(4), 475–479. https://doi.org/10.1016/j.jarmac.2020.09.003 [PR]
- Background for the claim that conditions which make learning feel harder can improve long-term retention. [Source](https://doi.org/10.1016/j.jarmac.2020.09.003)

**GenAI-specific sequencing evidence**

**Kumar, H., Rothschild, D. M., Goldstein, D. G., & Hofman, J. M. (2025).** *Math Education With Large Language Models: Peril or Promise?* In Artificial Intelligence in Education (AIED 2025), Lecture Notes in Computer Science (pp. 60–75). Springer. https://doi.org/10.1007/978-3-031-98459-4_5 [PR conference] (SSRN 2023: 10.2139/ssrn.4641653)
- **Design:** pre-registered experiment with **1,200 participants**. Two factors were manipulated:
  - attempting a problem *before* vs *after* seeing the answer;
  - answer only vs answer plus an LLM-generated explanation.

  Testing was on new problems.
- **Findings:**
  - LLM explanations improved learning compared with answers alone.
  - "The benefits were largest for those who attempted problems on their own first before consulting LLM explanations." Surprisingly, the benefit also held for explanation-first.
  - Exposure to LLM explanations "increased the amount people felt they learned and decreased the perceived difficulty of the test problems". [Source](https://api.semanticscholar.org/graph/v1/paper/DOI:10.2139/ssrn.4641653?fields=title,abstract)
- **Limitations:**
  - Online adult participants.
  - Short maths problems.
  - Microsoft Research authors.
- **Bears on:** (a) supports "attempt first, then AI" as optimal, but not as the only route. Also (c), on perceived learning.

**Kosmyna et al. (2025), session 4** (see section 2)
- **Brain-to-LLM** participants showed "higher memory recall" and more prefrontal activation.
- **LLM-to-Brain** participants showed under-engagement. [Source](https://arxiv.org/abs/2506.08872)
- Preprint with n = 18 in this session, so it is directional only.
- **Bears on:** (a).

**Autor et al. (2026)** (see section 3)
- Lasting gains from AI-assisted practice occurred only among seniors, which suggests foundational expertise as a prerequisite. [Source](https://www.nber.org/papers/w35720)
- **Bears on:** (a).

**Shen & Tamkin (2026)** (see section 1)
- Patterns that made learners generate or reason themselves preserved learning: "generation-then-comprehension", "conceptual inquiry" and "hybrid code-explanation".
- Delegation patterns did not. [Source](https://www.anthropic.com/research/AI-assistance-coding-skills)
- **Bears on:** (a), showing that the *order and type* of AI interaction matter.

**Bastani et al. (2025)** and **Kestin et al. (2025)** (see section 1)
- AI designed to give hints rather than answers (GPT Tutor) or to scaffold students' own reasoning (Kestin) avoided harm or produced gains.
- This supports the model "students generate, AI scaffolds", rather than "AI produces, students consume". [Source](https://doi.org/10.1073/pnas.2422633122); [Source](https://doi.org/10.1038/s41598-025-97652-6)

**Kreijkes et al. (2026)** (see section 1)
- Note-taking plus LLM did as well as note-taking alone and better than LLM alone, so the student's own processing must stay in the loop. [Source](https://doi.org/10.1016/j.compedu.2025.105514)

**Dickey, Mertzanidis & Psomas (2026)** (see section 1)
- Replacing "solve it yourself" with "evaluate flawed AI solutions" produced no summative difference. Evaluation tasks are not automatically a substitute for generation; the authors say "deliberate scaffolding" is needed. [Source](https://arxiv.org/abs/2607.27586)

**Lira et al. (2025)** (see section 1)
- AI-assisted practice, and even just viewing AI-revised examples, improved unaided cover-letter writing.
- This counters a universal "no AI first" rule for example-learnable skills. [Source](https://arxiv.org/abs/2502.02880)

**Brcic, M., & Frljic, S. (2026).** *The Effortless Trap: Productive Struggle, AI, and the Illusion of Learning.* arXiv:2606.26181. https://arxiv.org/abs/2606.26181 [PREPRINT, CONCEPTUAL]
- Proposes a six-step sequence: Prime, Probe, Point, Attach, Strengthen, Test.
- Its rule: "Secure the first hard attempt and the final unaided check, scaffold with guarded AI in between". Its diagnostic: "if letting AI in makes the task feel effortless, it is in the wrong place." [Source](https://arxiv.org/abs/2606.26181)
- **Bears on:** (a), as opinion and framework, not evidence.

### Inferences
- The evidence supports a refined version of claim (a):
  1. First an unaided attempt (generation, problem framing).
  2. Then AI as explainer, critic or scaffold.
  3. Then an unaided check (an assessment without AI).
- The strongest direct support comes from Kumar et al. (peer-reviewed conference paper), Autor et al. (working paper) and the productive-failure meta-analysis.
- "First without AI" should be framed as *first attempt and first framing without AI* within each learning cycle, not necessarily a whole semester without AI. The Lira and Kumar results show AI explanations can add value, even early, once students have their own attempt to compare against.
- The productive-failure boundary condition (I-PS favoured for domain-general skills) is a real caveat for "research skills". The memo can argue that problem framing in a *specific business context* is domain-specific enough for struggle-first to apply. That is an argument, not a tested finding.

### Gaps
- I found no RCT that tests "research skills without AI, then with AI" against "with AI from the start" in higher education. No study on business or management programmes was found.
- No published study tests productive failure with GenAI as the instruction phase. The search returned only design tools (e.g. ProductiveMath) and conceptual papers.
- The effect size for the generation effect (Bertsch et al.) is not verified here.

---

## 5. What is the evidence on self-assessment and calibration when using AI?

### Takeaway
Consistent evidence shows that AI use inflates confidence relative to actual competence:
- AI users overestimate their performance, and the usual Dunning–Kruger gradient flattens (Fernandes et al., two studies, N = 246 and N = 452).
- Students prefer LLMs and find them more helpful despite worse retention (Kreijkes et al.).
- LLM explanations raise *felt* learning (Kumar et al.).
- Confidence in AI predicts less critical-thinking effort (Lee et al.).
- Longer LLM explanations raise trust without improving accuracy (Steyvers et al.).

### Cited Findings

**Fernandes, D., Villa, S., Nicholls, S., Haavisto, O., Buschek, D., Schmidt, A., Kosch, T., Shen, C., & Welsch, R. (2026).** *AI makes you smarter but none the wiser: The disconnect between performance and metacognition.* Computers in Human Behavior, 175, 108779. https://doi.org/10.1016/j.chb.2025.108779 [PR]
- **Publication:** online Oct 2025, issue Feb 2026. Preprints: arXiv:2409.16708; SSRN 10.2139/ssrn.5212902.
- **Design:** two large studies.
  - Study 1: N = 246 participants solved 20 LSAT logical-reasoning problems with AI.
  - Study 2: N = 452, a replication.
- **Findings:**
  - Performance improved by about 3 points compared with a norm population, but participants **overestimated** their performance by about **4 points**.
  - "Higher AI literacy correlated with lower metacognitive accuracy."
  - "The Dunning-Kruger effect, usually observed in this task, ceased to exist with AI use." [Source](https://doi.org/10.1016/j.chb.2025.108779)
  - A monetary incentive did not correct the overestimation (press summary). [PRESS: PsyPost](https://www.psypost.org/users-of-generative-ai-struggle-to-accurately-assess-their-own-competence/)
- **Limitations:**
  - Adult online participants, not students.
  - A single reasoning task.
  - Comparison with a *norm population* in Study 1, not a randomised no-AI group.
- **Bears on:** (c) directly. Also (b): the product (score) and the self-judgment both drift from unaided ability.

**Steyvers, M., Tejeda, H., Kumar, A., Belem, C., Karny, S., Hu, X., Mayer, L. W., & Smyth, P. (2025).** *What large language models know and what people think they know.* Nature Machine Intelligence, 7(2), 221–231. https://doi.org/10.1038/s42256-024-00976-7 [PR]
- **Findings:**
  - Users "tend to overestimate the accuracy of LLM responses when provided with default explanations".
  - "Longer explanations increased user confidence, even when the extra length did not improve answer accuracy."
  - Aligning explanations with the model's confidence narrowed the calibration gap. [Source](https://doi.org/10.1038/s42256-024-00976-7)
- **Bears on:** (b), since a fluent, lengthy output persuades. Also (c).

**Kreijkes et al. (2026)** (see section 1)
- Students preferred the LLM and rated it more helpful, although LLM-only produced worse comprehension and retention than note-taking. [Source](https://doi.org/10.1016/j.compedu.2025.105514)
- **Bears on:** (c).

**Kumar et al. (2025)** (see section 4)
- LLM explanations "increased the amount people felt they learned and decreased the perceived difficulty of the test problems". [Source](https://api.semanticscholar.org/graph/v1/paper/DOI:10.2139/ssrn.4641653?fields=title,abstract)
- **Bears on:** (c). Here the perceived learning partly matched real gains, which is a nuance.

**Lee et al. (2025)** (see section 2)
- Higher confidence in GenAI was associated with less critical thinking; higher self-confidence with more. [Source](https://doi.org/10.1145/3706598.3713778)
- **Bears on:** (c), (d).

**Kosmyna et al. (2025)** (see section 2)
- The LLM group reported the lowest ownership and struggled to quote their own essays. [Source](https://arxiv.org/abs/2506.08872)
- [PREPRINT]. **Bears on:** (c).

**Fan et al. (2025)** (see section 2)
- "Metacognitive laziness": less self-regulatory monitoring with ChatGPT support. [Source](https://doi.org/10.1111/bjet.13544)
- **Bears on:** (c).

**Tankelevitch et al. (2024)** (see section 2)
- GenAI imposes high metacognitive monitoring and control demands. [Source](https://doi.org/10.1145/3613904.3642902)
- **Bears on:** (c), as theory.

**Autor et al. (2026), press framing**
- Coverage calls the junior result an "illusion of competence". This is a press framing, not a measured calibration outcome in the paper as verified here. [PRESS: Fortune](https://fortune.com/2026/10/10/david-autor-china-shock-nber-google-paper-illusion-of-competence-gen-z/)

### Inferences
- Claim (c) is well supported. The direction of the error is overconfidence: AI raises both performance and confidence, but confidence rises more, and low performers lose their usual signal that they are struggling (the flattened Dunning–Kruger effect).
- For assessment, students' self-assessments and reflections on AI-assisted work should not be taken as evidence of competence. Calibration has to be trained against unaided performance, for example by predicting a score and then sitting an unaided test.

**Cross-claim summary (for the memo writer)**

**(a) Without AI first, then with AI**
- *Strongest support:*
  - Autor et al. 2026 [WP]
  - Bastani et al. 2025 [PR]
  - Kumar et al. 2025 [PR]
  - Sinha & Kapur 2021 [PR]
  - Kreijkes et al. 2026 [PR]
  - Barcaui 2025 [PR]
  - Shen & Tamkin 2026 [PREPRINT]
- *Nuance or contradiction:*
  - Lira et al. 2025 [PREPRINT]: AI practice can transfer.
  - Kestin et al. 2025 [PR]: a scaffolded AI tutor beats active learning.
  - Kumar: explanation-first also helped.
  - The productive-failure boundary condition for domain-general skills.

**(b) The product says less about competence**
- *Strongest support:*
  - Scarfe et al. 2024 [PR]
  - Bastani et al. 2025 [PR]
  - Fan et al. 2025 [PR]
  - Rismanchian et al. 2026 [PREPRINT]
  - Dickey et al. 2026 [PREPRINT]
  - Deng et al. 2025's own caveat [PR]
  - Doshi & Hauser 2024 [PR]
  - Steyvers et al. 2025 [PR]
- *Nuance or contradiction:* Brynjolfsson et al. 2025 report some genuine learning among workers.

**(c) Students misjudge their AI-assisted performance**
- *Strongest support:*
  - Fernandes et al. 2026 [PR]
  - Kreijkes et al. 2026 [PR]
  - Steyvers et al. 2025 [PR]
  - Lee et al. 2025 [PR]
- *Nuance or contradiction:* in Kumar et al., the felt learning partly matched real gains.

**(d) Framing and judgment erode**
- *Strongest support:*
  - Stadler et al. 2024 [PR]
  - Dell'Acqua et al. 2026 [PR]
  - Lee et al. 2025 [PR]
  - Darvishi et al. 2024 [PR]
  - Autor et al. 2026 [WP]
  - Budzyń et al. 2025 [PR, by analogy]
- *Nuance or contradiction:*
  - Gerlich 2025 is only correlational.
  - Kosmyna 2025 is a preprint with an open critique.
  - No direct longitudinal measure of problem-framing ability exists.

### Gaps
- No calibration study was found with higher-education students on research or report tasks: predicted vs actual quality of an AI-assisted report, compared with an unaided one.
- It is unclear whether calibration training (e.g. predict, then unaided test) reduces AI-induced overconfidence. No intervention study was found.
- Fernandes et al. Study 1 used a norm-population comparison rather than a randomised no-AI control, so the "+3 points" figure should be described with that caveat.
