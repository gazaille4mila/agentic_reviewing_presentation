# ML Paper Review Tools Summary

This summary lists tools you can use right now in the ML pre-submission workflow, focused on review, readiness, compliance, and literature support.

## 1) PaperReview.ai
- Tool name: PaperReview.ai (Stanford Agentic Reviewer)
- Pros:
  - Free and fast first-pass review for CS/ML manuscripts.
  - arXiv-grounded feedback and reviewer-style scoring dimensions.
  - Useful for early draft triage before co-author circulation.
- Cons:
  - 15-page and 10 MB limits.
  - Best in CS/ML; weaker outside arXiv-heavy fields.
  - English-only support noted in source.
- Pricing: Free
- URL: https://paperreview.ai/
- IP handling:
  - Rights retained by author: No clear public ownership/IP terms found on the site.
  - Non-use of manuscript content: No public no-training/no-retention policy page found.
  - Guarantee verdict: Unknown (cannot confirm ownership protection or non-use guarantee).
  - Evidence: https://paperreview.ai/ , https://paperreview.ai/sitemap.xml

## 2) Refine.ink
- Tool name: Refine.ink
- Pros:
  - Strong at deep logic/proof auditing for theory-heavy papers.
  - Catches subtle assumption and internal consistency issues.
  - Supports native LaTeX and multiple document formats.
- Cons:
  - No live citation verification.
  - No vision-based figure analysis.
  - Ignores equations embedded as images.
- Pricing:
  - $49.99 one-time review
  - $39.99 per review (3-pack)
  - $29.99 per review (10-pack)
- URL: https://refine.ink/
- IP handling:
  - Rights retained by author: Terms state you retain rights to uploaded content.
  - Non-use of manuscript content: Privacy page states no LLM training on confidential uploads and no sale/sharing of uploaded content; providers are contractually restricted. Refine may still use interaction signals (for example comment interactions) to improve ranking unless opted out.
  - Guarantee verdict: Partial (strong manuscript-content protections, but not a blanket "no use in any way").
  - Evidence: https://www.refine.ink/terms-of-service , https://www.refine.ink/privacy-policy

## 3) Manusights
- Tool name: Manusights
- Pros:
  - Live citation checks against large scholarly databases.
  - Flags retractions/DOI issues and unsupported citation claims.
  - Vision-based figure/text consistency checks.
  - Gives journal-fit/readiness scoring and prioritized revision plan.
- Cons:
  - Not a direct prose rewriting tool.
  - Best positioned as final-stage diagnostic rather than early drafting assistant.
- Pricing:
  - Free readiness scan
  - $29 full AI diagnostic
  - Optional human expert review: ~$1,000-$1,800
- URL: https://manusights.com/
- IP handling:
  - Rights retained by author: Terms explicitly say you retain all rights to your manuscript.
  - Non-use of manuscript content: Privacy/terms/security pages state zero-retention processing, no training use, immediate deletion after analysis, and NDA-limited access on human path.
  - Guarantee verdict: Strong (for manuscript-content non-training/non-retention), with normal operational metadata caveats.
  - Evidence: https://manusights.com/terms , https://manusights.com/privacy , https://manusights.com/security

## 4) Reviewer3
- Tool name: Reviewer3
- Pros:
  - Fast structural and methodology triage (minutes).
  - Anchors comments to PDF passages for targeted revision.
  - Strong fabricated-reference detection and reproducibility checks.
- Cons:
  - Limited journal-specific targeting.
  - No live novelty/citation-grounding depth like Manusights.
  - Limited figure-vision analysis.
- Pricing:
  - Free first review path
  - Premium: $19 one-time (unlimited revisions option reported)
  - Or $29/month subscription
- URL: https://reviewer3.com/
- IP handling:
  - Rights retained by author: You retain ownership of User Content (Input); Reviewer3 assigns all rights in Output back to you. However, you grant Reviewer3 a perpetual, irrevocable, royalty-free, sublicensable worldwide license to use, reproduce, adapt, distribute, and exploit your User Content.
  - Non-use of manuscript content: **Terms explicitly allow AI training on User Content by default.** Opt-out requires emailing support@reviewer3.com. Security page's "never used for training" claim contradicts the legal terms.
  - Guarantee verdict: No (opt-out model only — training on submitted content is the default; security page marketing claim is contradicted by the Terms of Service).
  - Evidence: https://reviewer3.com/security , https://reviewer3.com/privacy , https://reviewer3.com/terms , agentic_reviewing_tools/privacy.pdf , agentic_reviewing_tools/terms.pdf

## 5) q.e.d Science
- Tool name: q.e.d Science
- Pros:
  - Claim-tree decomposition maps claims to evidence.
  - Helps tighten over-strong claims or identify needed experiments.
  - Good for resolving co-author disagreements on claim strength.
- Cons:
  - No live citation verification.
  - No desk-reject/journal-fit scoring.
- Pricing: Free (with institutional email, per source)
- URL: (Referenced via comparison source) https://manusights.com/blog/ai-manuscript-review-tools-compared
- IP handling:
  - Rights retained by author: Terms say you retain rights in customer data.
  - Non-use of manuscript content: Terms also grant q.e.d a non-revocable license to use uploaded papers to train/fine-tune/evaluate q.e.d models and allow commercialization of anonymized/aggregated usage analytics.
  - Guarantee verdict: No (not a non-use service; manuscript content can be used for model improvement under their terms).
  - Evidence: https://www.qedscience.com/terms-of-use , https://www.qedscience.com/privacy-policy

## 6) ScholarsReview
- Tool name: ScholarsReview
- Pros:
  - Broad all-in-one workflow: review, literature help, journal finding, grammar.
  - Useful for early-career users needing one platform for many tasks.
- Cons:
  - Less transparent and less deep on technical scientific verification.
  - Weaker live-citation rigor than specialized tools.
- Pricing: Not clearly specified in source text
- URL: https://scholarsreview.com/
- IP handling:
  - Rights retained by author: No dedicated terms page found in this check; ownership clause not independently confirmed.
  - Non-use of manuscript content: Privacy page claims uploaded files are automatically deleted after processing and not retained/shared.
  - Guarantee verdict: Partial (privacy claims are strong, but legal enforceability cannot be fully confirmed without published terms).
  - Evidence: https://scholarsreview.com/privacy-policy

## 7) Google Paper Assistant Tool (PAT)
- Tool name: Google Paper Assistant Tool (PAT)
- Pros:
  - Conference-endorsed (ICML/NeurIPS 2026 pilots in source).
  - Focuses on methodological rigor, correctness, and clarity.
  - Private/stateless author feedback separated from official review process.
- Cons:
  - Availability tied to conference programs/pilots, not universal self-serve.
  - Access may depend on venue participation windows.
- Pricing: Not publicly specified in source (conference-provided in pilot context)
- URL: https://blog.neurips.cc/2026/04/21/neurips-supports-authors-with-googles-paper-assistant-tool-pat/
- IP handling:
  - Rights retained by author: Pilot posts focus on privacy/process controls; explicit IP ownership clause is not the main framing.
  - Non-use of manuscript content: ICML/NeurIPS PAT posts explicitly state stateless inference, no training/fine-tuning on submissions, restricted access, and scheduled deletion after feedback/program completion.
  - Guarantee verdict: Strong within PAT pilot scope.
  - Evidence: https://blog.neurips.cc/2026/04/21/neurips-supports-authors-with-googles-paper-assistant-tool-pat/ , https://blog.icml.cc/2026/01/14/icml-experimental-program-using-googles-paper-assistant-tool-pat/

## 8) Bibby AI
- Tool name: Bibby AI
- Pros:
  - AI-native LaTeX workspace with context-aware editing support.
  - Built-in paper review, citation search, equation/table generation.
  - Strong reported LaTeX error detection/fix performance in source benchmarks.
- Cons:
  - Primarily a writing environment; review quality varies by manuscript type.
  - Some benchmark claims come from product-adjacent sources.
- Pricing:
  - Freemium
  - Pro reported around $8-$20/month (academic discount dependent)
- URL: https://trybibby.com/
- IP handling:
  - Rights retained by author: Data-security page says users keep 100% ownership/IP and Bibby claims no rights to content.
  - Non-use of manuscript content: Page states no training on user data, zero-retention provider agreements, and deletion controls.
  - Guarantee verdict: Strong (based on published security commitments).
  - Evidence: https://trybibby.com/data-security

## 9) OpenAI Prism
- Tool name: OpenAI Prism
- Pros:
  - Integrated LaTeX + live preview + inline AI refinement.
  - Good for polishing existing technical manuscripts.
- Cons:
  - Less specialized than Bibby for some LaTeX-fix workflows.
  - Limited evidence of full end-to-end reviewer-style diagnostics.
- Pricing: Approximately $12/month (as cited in source)
- URL: (Referenced review source) https://www.thesisai.io/blog/openai-prism-ai-latex-editor-review/
- IP handling:
  - Rights retained by author: Under OpenAI terms, users retain ownership of input and own output (as between user and OpenAI).
  - Non-use of manuscript content: For individual services, OpenAI may use content to improve services/models unless the user opts out; for business/API products default is no training unless opt-in.
  - Guarantee verdict: Conditional/partial (depends on account type and settings; no universal non-use guarantee).
  - Evidence: https://openai.com/policies/terms-of-use , https://openai.com/policies/how-your-data-is-used-to-improve-model-performance

## 10) Overleaf AI Features (Writefull/TeXGPT ecosystem)
- Tool name: Overleaf AI Integration
- Pros:
  - Familiar LaTeX platform with strong collaboration and template ecosystem.
  - AI support for language feedback and basic generation tasks.
- Cons:
  - AI capabilities are less agentic/deep than specialized review tools.
  - More writing-assist oriented than scientific-critique oriented.
- Pricing: Overleaf subscription/institutional plans (AI feature pricing not clearly separated in source)
- URL: https://www.overleaf.com/about/ai-features
- IP handling:
  - Rights retained by author: Overleaf terms state they do not claim ownership of your content; for AI tools, inputs/outputs are treated as your stuff and you retain ownership.
  - Non-use of manuscript content: Overleaf AI pages/terms state no training on your project data for model development without consent and require third-party providers not to use your content for their own model training.
  - Guarantee verdict: Strong for AI-training non-use; standard service-operation/retention clauses still apply.
  - Evidence: https://www.overleaf.com/legal , https://www.overleaf.com/about/ai-features

## 11) SciScore
- Tool name: SciScore
- Pros:
  - Strong compliance/method reporting checks (RRIDs, ethics/statistics signals).
  - Useful for reducing desk-reject risk from reporting omissions.
- Cons:
  - Not a full novelty/methodological ML reviewer.
  - More compliance-focused than claim-level scientific critique.
- Pricing: Not specified in source text
- URL: https://www.scicrunch.com/sciscorereport-faq
- IP handling:
  - Rights retained by author: No clear manuscript-IP ownership clause found in accessible SciCrunch policy text.
  - Non-use of manuscript content: Privacy statement (older) covers personal-data handling and third-party disclosure limits, but does not provide explicit AI-model-training/non-use guarantees for manuscript content.
  - Guarantee verdict: Unknown/partial.
  - Evidence: https://www.scicrunch.com/privacy-statement

## 12) Paperpal Preflight
- Tool name: Paperpal Preflight
- Pros:
  - Fast pre-submission format/metadata/reference checks.
  - Good firewall against administrative desk rejection.
- Cons:
  - Not a deep technical reviewer of ML methodology.
  - Limited for novelty/baseline/ablation critique.
- Pricing: Not specified in source text
- URL: https://paperpal.com/preflight-for-authors
- IP handling:
  - Rights retained by author: Paperpal FAQ indicates a copyright-retention question is addressed; explicit answer text was not fully extractable in this run.
  - Non-use of manuscript content: Paperpal pages state "We don't train AI models on your data. Ever." and "your data is never used to train AI systems."
  - Guarantee verdict: Partial to strong (very clear non-training claim; ownership clause should be verified directly in full FAQ/terms).
  - Evidence: https://paperpal.com/ , https://paperpal.com/preflight-for-authors

## 13) Anonymous GitHub (anonymous.4open.science)
- Tool name: Anonymous GitHub
- Pros:
  - Preserves double-blind anonymity while sharing code.
  - Redacts identifying metadata and gives stable anonymous links.
  - Critical for conference policy compliance when code is required.
- Cons:
  - Not a paper quality reviewer by itself.
  - Requires careful repo hygiene to avoid leakage in non-text artifacts.
- Pricing: Free (open-source tool, per source framing)
- URL: https://anonymous.4open.science/
- IP handling:
  - Rights retained by author: Tool mirrors existing GitHub repositories for anonymized sharing; no transfer of authorship rights is indicated in the public pages checked.
  - Non-use of manuscript content: Manual FAQ expansion states repository data is not shared or used beyond anonymization service operation; when repositories are removed/expired, configuration metadata is retained to allow restoration and avoid ID reuse.
  - Guarantee verdict: Partial (clear service-scope non-sharing statement, but metadata/config retention means not a strict no-use/no-retention guarantee).
  - Evidence: https://anonymous.4open.science/ , https://anonymous.4open.science/faq

## 14) Elicit
- Tool name: Elicit
- Pros:
  - Useful for literature synthesis and evidence extraction.
  - Helps compare methods/datasets/findings across papers quickly.
- Cons:
  - Not a full pre-submission peer-review simulator.
  - Best as literature-support tool, not final acceptance-readiness check.
- Pricing: Not specified in source text
- URL: https://elicit.com/
- IP handling:
  - Rights retained by author: Terms say you retain rights/title in your content.
  - Non-use of manuscript content: Terms grant Elicit a broad perpetual license to use/modify content for service provision and allow retention/use of aggregated behavioral/telemetry data to improve and market services.
  - Guarantee verdict: No (not a strict non-use model).
  - Evidence: https://elicit.com/operations/terms

## 15) Semantic Scholar
- Tool name: Semantic Scholar
- Pros:
  - Large-scale scholarly search with ML-assisted relevance and summaries.
  - Helps validate related-work coverage and citation quality.
- Cons:
  - Discovery tool, not a direct manuscript reviewer.
  - Requires manual interpretation for paper-specific critique.
- Pricing: Free (core use)
- URL: https://www.semanticscholar.org/
- IP handling:
  - Rights retained by author: Ai2 terms say users own inputs and (where applicable) outputs.
  - Non-use of manuscript content: Ai2 terms also grant a broad license and reserve the right to train models on user content unless a specific service says otherwise.
  - Guarantee verdict: No (no universal non-use guarantee at the platform-terms level).
  - Evidence: https://allenai.org/terms.html

## 16) Connected Papers
- Tool name: Connected Papers
- Pros:
  - Visual citation graph exploration for related work mapping.
  - Helps uncover foundational and derivative papers.
- Cons:
  - Not a manuscript quality/reproducibility auditor.
  - Limited direct guidance on ML experiment design quality.
- Pricing: Not specified in source text
- URL: https://www.connectedpapers.com/
- IP handling:
  - Rights retained by author: No explicit manuscript-IP ownership protections identified in connectedpapers terms/privacy.
  - Non-use of manuscript content: Policies describe collection of account/search/saved-paper data and sharing with third-party providers for operations; no explicit no-training/no-reuse guarantee.
  - Guarantee verdict: No/unknown for strict manuscript non-use.
  - Evidence: https://www.connectedpapers.com/privacy , https://www.connectedpapers.com/terms

## 17) Research Rabbit
- Tool name: Research Rabbit
- Pros:
  - Graph-based discovery and tracking of literature trajectories.
  - Useful for keeping related work current over drafting iterations.
- Cons:
  - Not a direct pre-submission reviewer.
  - Requires manual synthesis of insights into manuscript edits.
- Pricing: Not specified in source text
- URL: https://www.researchrabbit.ai/
- IP handling:
  - Rights retained by author: Terms/privacy are now extractable (served under Litmap Limited legal text), but no strong manuscript-IP ownership guarantee analogous to dedicated manuscript-review tools was identified.
  - Non-use of manuscript content: Policies describe sharing with AI service providers (including OpenAI/Databricks), vendors/affiliates, and analytics use; no explicit blanket "never used to train" manuscript guarantee was found.
  - Guarantee verdict: Partial (policies are available and specific, but no strict non-use guarantee for uploaded content).
  - Evidence: https://www.researchrabbit.ai/privacy-policy , https://www.researchrabbit.ai/terms-of-service

## 18) Scholarcy
- Tool name: Scholarcy
- Pros:
  - Rapid PDF summarization for literature screening.
  - Good for triaging large reading lists before writing related work.
- Cons:
  - Not a reviewer-style technical audit tool.
  - Summary quality depends on source document structure.
- Pricing: Not specified in source text
- URL: https://www.scholarcy.com/
- IP handling:
  - Rights retained by author: Terms state users remain owners of verbatim content; provider owns Scholarcy/Everway results.
  - Non-use of manuscript content: Terms state they do not sell personal data or processed documents and include confidentiality commitments; no explicit blanket "never used in any way" model-training prohibition found.
  - Guarantee verdict: Partial (ownership and confidentiality are clear, but strict no-use/no-training guarantee is not explicit in the extracted terms text).
  - Evidence: https://www.scholarcy.com/terms-of-service

---

## Practical shortlist for your upcoming ML review
If your goal is pre-submission paper quality improvement (not just literature search), prioritize:
1. PaperReview.ai (quick/free first pass)
2. Reviewer3 (mid-draft structure/method checks)
3. Refine.ink (theory/proof-heavy audits)
4. Manusights (final readiness, citations, figures, desk-reject risk)
5. Anonymous GitHub (double-blind code sharing compliance)
