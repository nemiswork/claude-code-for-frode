# Example 2: Research Assistant

> Time: ~15 minutes
> Goal: Use Claude Code for literature review, manuscript work, and grant writing

## Literature Search & Review

### Quick Literature Scan

```
Search the web for recent papers (2025-2026) on single-cell proteomics
in acute myeloid leukemia. Summarize the top 5 findings and identify
any gaps in the current research.
```

### Deep-Dive on a Topic

```
I'm writing a review section on mass spectrometry-based biomarker discovery
for neurodegenerative diseases. Give me a structured outline covering:
1. Current LC-MS/MS approaches
2. CSF vs blood-based biomarkers — pros and cons
3. Clinical translation challenges
4. Where the field is heading

Include key references I should cite.
```

### Compare Papers

Save two abstracts as text files, then:

```
Read abstract1.txt and abstract2.txt. Compare their methodological approaches,
identify contradictions, and tell me which has stronger evidence for their claims.
```

## Manuscript Assistance

### Draft a Methods Section

```
I ran a TMT-labeled quantitative proteomics experiment with the following setup:
- 10 CSF samples (5 Alzheimer's, 5 controls)
- TMT-10plex labeling
- High-pH reversed-phase fractionation (8 fractions)
- nanoLC-MS/MS on Orbitrap Eclipse
- MaxQuant 2.1 for database search (UniProt human, 1% FDR)
- Perseus for statistical analysis

Write a methods section suitable for a Journal of Proteome Research submission.
```

### Improve Writing

```
Read my draft in draft-introduction.txt. Improve the scientific writing:
- Tighten the logic flow
- Remove redundancy
- Strengthen the transitions
- Keep my voice — don't make it sound like AI wrote it
```

### Response to Reviewers

```
Here are the reviewer comments for our manuscript:

Reviewer 2, Comment 3: "The authors have not adequately addressed the
issue of missing values in their TMT dataset. With >30% missing values
in some channels, the imputation strategy needs stronger justification."

Draft a polite, evidence-based response. Reference our use of MinProb
imputation and cite the Lazar et al. 2016 paper that validates this
approach for MNAR data in proteomics.
```

## Grant Writing

### Structure a Grant

```
I'm applying for NFR FRIPRO funding for a project on:
"Clinical-grade proteomics platform for real-time biomarker monitoring
in neurodegenerative disease progression"

Budget: 12M NOK, 4 years
Team: 1 postdoc, 2 PhD students, 1 engineer

Create a structured project description following NFR's format:
1. Scientific background and objectives
2. Methodology and approach
3. Impact and relevance
4. Implementation plan and milestones
```

### Budget Justification

```
Write budget justification text for:
- 1x Orbitrap Astral mass spectrometer (8M NOK)
- Explain why this specific instrument is critical
- Compare to alternatives (Exploris, timsTOF)
- Justify in terms of clinical proteomics throughput
```

## What You Just Learned

- Claude can do real academic research assistance
- It knows proteomics terminology and workflows
- You can iterate on drafts without starting over
- It writes in proper scientific style
- It can structure complex documents (grants, reviews, responses)

> *Note: Always verify citations and facts. Claude is incredibly useful but occasionally hallucinates references. Think of it like a brilliant but sometimes overconfident PhD student — trust but verify.*
>
> *Unlike certain conspiracy theories, Claude's claims are at least checkable.*

**Next:** [03-data-analysis.md](03-data-analysis.md) — let Claude crunch your data.
