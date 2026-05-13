# ML Paper Review Tools Summary

This summary lists tools that automatically review or assess manuscripts (review-style feedback, readiness diagnostics, or compliance/risk checks).

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

## 8) SciScore
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

## 9) Paperpal Preflight
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

---

## Practical shortlist for your upcoming ML review
If your goal is pre-submission paper quality improvement (not just literature search), prioritize:
1. PaperReview.ai (quick/free first pass)
2. Reviewer3 (mid-draft structure/method checks)
3. Refine.ink (theory/proof-heavy audits)
4. Manusights (final readiness, citations, figures, desk-reject risk)
5. q.e.d Science (deep claim/evidence critique)
