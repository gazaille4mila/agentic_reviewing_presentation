# Automatic Paper Review Tools

This guide aims to help AMLRT researchers and project managers to select AI-powered review tools for project reports and scientific manuscripts, where intellectual property sensitivity varies from public-facing drafts to highly sensitive proprietary work.

**Before using any tool in this document:** All tool selections should be validated with the project manager and, when appropriate, with the legal and/or IT team to ensure alignment with data sensitivity requirements and Mila policy.

---

## Tool Description Matrix

**Column definitions:**
- **Tool:** Name of the tool or platform.
- **URL:** Main public webpage.
- **Best Use Case:** The manuscript review task(s) this tool handles best.
- **Pricing:** Publicly listed access model; prices are indicative and may change.
- **Default Training?:** Whether the vendor's legal terms allow use of uploaded content to train AI models by default.
- **Retention Posture:** What the vendor states about how long uploaded content is stored before deletion.
- **Evidence Strength:** Quality of the evidence supporting the tool's privacy posture: ⭐⭐⭐ direct legal terms and security documentation; ⭐⭐ public claims or partial terms; ⭐ marketing copy or incomplete documentation only.
- **Fit for confidential work?:** Whether the tool is *Potentially* suitable for confidential manuscripts (pending PM/legal/IT approval) or *No* (do not use for confidential work).



| Tool | URL | Best Use Case | Pricing | Default Training? | Retention Posture | Evidence Strength | Fit for confidential work? |
|------|-----|---------------|---------|-------------------|-------------------|------------------|----------------------------|
| **Manusights** | https://manusights.com/ | End-stage journal-fit scoring, citation verification, figure consistency | Free scan; $29 AI diagnostic; $1,000-$1,800 human review | No | Zero-retention, immediate deletion | ⭐⭐⭐ Direct terms + security pages | **Potentially** |
| **Refine.ink** | https://www.refine.ink/ | Theory-heavy papers, mathematical proof auditing, internal consistency | $49.99 one-time; $39.99/review (3-pack); $29.99/review (10-pack) | No | Zero-retention on confidential uploads | ⭐⭐⭐ Terms + privacy pages | **Potentially** |
| **Paperpal Preflight** | https://paperpal.com/preflight-for-authors | Format compliance, metadata checks, desk-rejection firewall | Request demo/contact sales; no public numeric pricing found | No (for chatbot data; preflight scope needs confirmation) | Zero-retention/immediate deletion claimed on product pages | ⭐⭐ Public claims + Cactus ToU for chatbot | **Potentially** |
| **q.e.d Science** | https://www.qedscience.com/ | Claim decomposition, co-author alignment on claim strength | Free (with institutional email) | Yes (explicit training rights) | Non-revocable license to use for model improvement | ⭐⭐ Direct ToS | **No** |
| **Reviewer3** | https://reviewer3.com/ | Methodology triage, reproducibility checks, fabricated reference detection | Free first review; $19 one-time or $29/month | Yes (opt-out model) | Zero-retention claimed, but training is default | ⭐⭐ Security page contradicts ToS | **No** |
| **ScholarsReview** | https://scholarsreview.com/ | All-in-one platform (review, grammar, journal finding) | From $4.99; $14.99/4 docs; $45/month; fixes plans up to $90/month | No (claimed) | Auto-deletion claimed, terms not fully accessible | ⭐⭐ Privacy claim, but terms hard to find | **No** |
| **SciScore** | https://sciscore.com/ | Compliance/reporting checks (RRIDs, ethics, statistics signals) | 1 report free via ORCID signup; additional reports via AsedaSciences (no public numeric pricing) | Unknown | Unknown | ⭐ Privacy statement vague | **No** |
| **PaperReview.ai** | https://www.paperreview.ai/ | Free rapid triage for CS/ML conference papers | Free | Unknown | Unknown | ⭐ Homepage + sitemap only | **No** |


---

## Detailed Tool Assessments

### Potentially Fit for Confidential Work

#### Manusights
**Best for:** Final-stage submission readiness, journal-fit prediction, citation accuracy verification

**Strengths:**
- Live citation verification (500M+ paper database across CrossRef, PubMed, OpenAlex, Semantic Scholar, bioRxiv, medRxiv)
- Detects retracted papers, DOI errors, hallucinated references
- Vision-based figure/text consistency checks
- Journal-fit scoring with prioritized revision plan
- Explicit zero-retention, no training use, immediate deletion after analysis
- NDA-limited access on human review path
- Human expert review available

**Limitations:**
- Does not rewrite prose
- Best as final-stage diagnostic, not early drafting

**Pricing:** Free readiness scan; $29 full AI diagnostic; optional human review $1,000–$1,800

**IP Guarantee:** Strong ✅
- Explicit terms state you retain all manuscript rights
- Zero-retention processing, no training use, immediate deletion, NDA-limited access
- Evidence: https://manusights.com/terms, https://manusights.com/privacy, https://manusights.com/security

---

#### Refine.ink
**Best for:** Theory-heavy papers, mathematical proofs, internal logic auditing

**Strengths:**
- Intensive parallel compute (2+ hours, hundreds of frontier model calls per review)
- Identifies subtle proof assumptions, notation inconsistencies, internal reference errors
- Meticulously audits claim-to-data alignment
- Native LaTeX support + 12 file formats
- Explicit zero-LLM-training clause on confidential uploads
- Contractually restricted providers

**Limitations:**
- No live citation verification
- No vision-based figure analysis
- No journal-fit scoring
- Ignores equations embedded as images

**Pricing:** $49.99 one-time; $39.99 per review (3-pack); $29.99 per review (10-pack)

**IP Guarantee:** Partial ✅
- Terms state you retain rights to uploaded content
- No training on confidential uploads, providers contractually restricted
- May use interaction signals (e.g., comment behavior) to improve ranking, but no training on manuscript content per se
- Evidence: https://www.refine.ink/terms-of-service, https://www.refine.ink/privacy-policy

---

#### Paperpal Preflight
**Best for:** Format compliance, metadata completeness, reference structure checks

**Strengths:**
- Fast pre-submission compliance (under 2 minutes)
- Clear no-training statement: "We don't train AI models on your data. Ever."
- Firewall against administrative desk rejection

**Limitations:**
- Not a deep technical reviewer
- Limited novelty or baseline critique
- Cactus ToU ownership/no-training clause is explicit for AI chatbot input/output, but applicability to all Preflight uploads is not stated with equal clarity

**Pricing:** Request demo/contact sales; no public numeric pricing found on Preflight pages

**IP Guarantee:** Partial ⚠️
- Clear non-training claim on public pages
- Cactus ToU includes explicit AI chatbot language: users retain ownership of chatbot input, and data is not used to train the chatbot model/platform
- Scope caveat: the strongest legal clause is explicitly tied to chatbot usage; confirm contractual coverage for Paperpal Preflight manuscript uploads before confidential use
- **Recommendation:** Potentially fit for confidential work, with PM/legal sign-off before confidential uploads
- Evidence: https://paperpal.com/, https://paperpal.com/preflight-for-authors, https://cactusglobal.com/terms-of-use

---

### Public Work Only

#### q.e.d Science
**Best for:** Claim decomposition, co-author alignment on claim strength (public work only)

**Why avoid:**
- **Explicit training rights:** Terms grant q.e.d a non-revocable license to use uploaded papers to train, fine-tune, and evaluate q.e.d models
- **Commercialization:** Allows commercialization of anonymized/aggregated usage analytics derived from your uploads

**Strengths (ignoring IP issue):**
- Claim-tree decomposition maps claims to supporting evidence
- Helps identify over-strong claims or missing experiments
- Good for resolving co-author disagreements

**Limitations:**
- No live citation verification
- No desk-reject or journal-fit scoring

**Pricing:** Free (with institutional email)

**IP Guarantee:** None ❌
- Explicit training and commercialization rights in terms
- Not a zero-use service for manuscript content
- Evidence: https://www.qedscience.com/terms-of-use, https://www.qedscience.com/privacy-policy

**Recommendation:** Public work only. Avoid for confidential work.

---

#### Reviewer3
**Best for:** Methodology triage, reproducibility checks, fabricated reference detection (public work only)

**Why avoid:**
- **Legal/marketing contradiction:** Security page claims "never used for training," but Terms of Service explicitly allow AI training on User Content by default
- **Opt-out model:** Training occurs unless user emails support@reviewer3.com to opt out
- **Risk:** Default assumption is that all uploads are usable for model improvement

**Strengths (ignoring IP issue):**
- Rapid structural triage (under 10 minutes)
- 97.7% fabricated-reference detection accuracy
- PDF-anchored feedback for targeted revision

**Limitations:**
- Lacks journal-specific targeting
- No live novelty assessment
- Limited figure-vision analysis

**Pricing:** Free first review; $19 one-time or $29/month premium

**IP Guarantee:** None ❌
- Terms grant Reviewer3 a perpetual, irrevocable, royalty-free, sublicensable worldwide license to use, reproduce, adapt, and exploit your User Content
- Training on submissions is default; opt-out requires email request
- Security page messaging ("never used for training") contradicts legal terms
- Evidence: https://reviewer3.com/terms, https://reviewer3.com/security, https://reviewer3.com/privacy

**Recommendation:** Public work only. Do not use for confidential material.

---

#### ScholarsReview
**Best for:** Broad all-in-one workflow (review, grammar, journal finding, literature help)

**Strengths:**
- All-in-one platform for early-career researchers
- Useful for many simultaneous workflow needs
- Claims auto-deletion of uploaded files after processing

**Limitations:**
- Less transparent and less deep on technical scientific verification
- Weaker live-citation rigor than specialized tools
- Terms of service not easily accessible

**Pricing:** Public plans listed on site: $4.99 (single review), $14.99 (4 reviews), $45/month (unlimited), $11.99 (single fix), $23.99 (4 fixes), $90/month (fixes unlimited)

**IP Guarantee:** Partial ⚠️
- Privacy page claims auto-deletion and no retention/sharing
- Published terms of service not directly accessible in standard venues
- **Recommendation:** Public work only unless legal review confirms confidential-use safety
- Evidence: https://scholarsreview.com/privacy-policy

---

#### SciScore
**Best for:** Compliance and reporting standard verification (RRIDs, ethics statements, statistics signals)

**Strengths:**
- Automated reporting standard checks (Research Resource Identifiers, ethics/statistics flags)
- Reduces desk-reject risk from methodological reporting gaps

**Limitations:**
- Not a full novelty or methodological ML reviewer
- More administrative than scientific critique

**Pricing:** 1 report free via ORCID signup; additional reports available via AsedaSciences partner flow (no public numeric price list)

**IP Guarantee:** Unknown/Partial ⚠️
- No clear manuscript-IP ownership clause in accessible SciCrunch documentation
- Privacy statement does not explicitly guarantee AI-model non-use for manuscript content
- **Recommendation:** Public work only unless vendor terms are clarified for confidential use
- Evidence: https://www.scicrunch.com/sciscorereport-faq, https://www.scicrunch.com/privacy-statement

---

#### PaperReview.ai
**Best for:** Early triage for CS/ML conference papers (public work only)

**Why unclear:**
- No published terms of service or privacy policy on main site
- No public data handling documentation
- Cannot confirm ownership protection or non-training guarantee

**Strengths:**
- Free, fast, arXiv-grounded feedback for CS/ML papers
- Trained to mimic ICLR review scores
- Useful for early triage before co-author circulation

**Limitations:**
- 15-page, 10 MB file size limits
- Best in CS/ML; weak outside arXiv-heavy domains
- English-only support

**Pricing:** Free

**IP Guarantee:** Unknown ❌
- No accessible terms of service or privacy policy
- No public documentation of data handling or training policies
- Cannot verify ownership retention or non-training commitment

**Recommendation:** Public work only. Do not use for confidential work until vendor publishes explicit IP and data-handling terms.

---

## Conference-Endorsed Tools

Major ML conferences are beginning to offer official pre-submission author feedback tools. [ICML 2026](https://blog.icml.cc/2026/01/14/icml-experimental-program-using-googles-paper-assistant-tool-pat/) and [NeurIPS 2026](https://blog.neurips.cc/2026/04/21/neurips-supports-authors-with-googles-paper-assistant-tool-pat/), for example, both ran optional programs using Google's Paper Assistant Tool (PAT), giving authors automated feedback before submission with explicit stateless inference and scheduled deletion guarantees. These conference-hosted programs tend to carry stronger IP protections than self-serve vendor tools, since data handling is governed directly by the conference and program organizers rather than a commercial third party.

Researchers should keep an eye on submission guidelines for future mainstream ML conferences (ICML, NeurIPS, ICLR, EMNLP, CVPR, etc.) for similar offerings. Availability is tied to specific submission windows and is not guaranteed to continue across cycles — verify at the time of submission.
