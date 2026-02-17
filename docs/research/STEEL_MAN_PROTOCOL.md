# Steel-Man Protocol for Research Review

## Purpose

This protocol provides a rigorous methodology for adversarial review of research documents. By constructing the strongest possible version of an argument before critiquing it, we ensure that any refutation addresses the actual substance of the claim rather than weak or misrepresented versions.

## Foundation

This protocol combines:
- **Rapoport's Rules** (via Daniel Dennett) - Four steps for intelligent criticism
- **Steel-manning methodology** - Constructing the strongest possible version of an argument
- **Principle of Charity** - Interpreting arguments in their most rational form

## The Protocol

### Phase 1: Understanding & Strengthening (Iterative)

#### Step 1: Re-express

**Goal**: State the argument so clearly and fairly that the original author would say "I wish I'd thought of putting it that way."

- **Sources**: Primary research document
- **Tools**: `fs_read` to read the document
- **Effort**: Complete reading, extract core claims and supporting arguments
- **Output**: Clear restatement of the core argument

#### Step 2: Strengthen

**Goal**: Fill logical gaps, add best supporting evidence, resolve ambiguities in favor of the claim.

- **Sources**: Primary research document + external supporting sources (academic papers, primary sources, corroborating evidence)
- **Tools**: `fs_read` for document, `web_search` to find supporting evidence, `web_fetch` to retrieve full sources
- **Effort**: Search for 3-5 high-quality sources that support the claim
- **Priority**: Academic papers > primary sources > expert commentary > general sources

**Document Retrieval Procedure**:
1. Identify DOI if available
2. Try DOI resolver (https://doi.org/[DOI])
3. Try `web_fetch` on direct URL
4. Search for alternative sources (PubMed Central, arXiv, institutional repositories, author websites)
5. Try PDF versions, HTML versions, cached versions
6. Only after exhausting all options: Add to BibTeX, open Gitea issue with retrieval attempts documented

**File Naming Convention**:
- Format: `[url-safe-doi]_[year]-[author]-[short-title].pdf`
- DOI conversion: replace `/` with `_`, `:` with `-`
- Example: `10.1073_pnas.1320040111_2014-kramer-emotional-contagion.pdf`
- If no DOI: use `[year]-[author]-[short-title].pdf` as fallback
- Save to: `assets/pdf/`

**Document Management**:
- Maintain BibTeX file for citations
- Maintain CSL-JSON file linking metadata to local files
- CSL-JSON entry includes:
  - All bibliographic metadata
  - `file` field pointing to local PDF
  - DOI as primary identifier
  - Retrieval date and source URL

**Output**: Strengthened version of the argument with supporting citations

#### Step 3: Verify

**Goal**: Confirm the strengthened version faithfully represents the original claim.

- **Sources**: Primary research document
- **Tools**: `fs_read` to re-read the document
- **Effort**: Line-by-line comparison of strengthened version against original
- **Decision**: 
  - If verification fails: Return to Step 1 with improved understanding, repeat cycle
  - If verification succeeds: Proceed to Phase 2

### Phase 2: Acknowledgment (Iterative)

#### Step 4: Acknowledge Agreement

**Goal**: List points where the argument is correct or valid.

- **Sources**: Primary research document + established facts/evidence
- **Tools**: `fs_read` for document, `web_search` to verify factual claims
- **Effort**: Verify each factual claim, identify 2-3 strongest valid points
- **Priority**: Verifiable facts > sound reasoning > novel insights
- **Output**: List of valid points with verification

#### Step 5: State What You Learned

**Goal**: Identify what the argument taught you or what insights it provides.

- **Sources**: Primary research document + prior knowledge base
- **Tools**: Analysis of document content against existing knowledge
- **Effort**: Identify 1-3 genuine insights or new information
- **Decision**: If new valid points emerge, return to Step 4 to add them
- **Output**: Statement of genuine learning or insights gained

### Phase 3: Critique (Iterative)

#### Step 6: Critique

**Goal**: Present counter-evidence and refutation, attacking the strongest version.

- **Sources**: Primary research document + counter-evidence sources (academic papers, primary sources that contradict or weaken the claim)
- **Tools**: `fs_read` for document, `web_search` to find counter-evidence, `web_fetch` to retrieve contradicting sources
- **Effort**: Search for 3-5 high-quality sources that contradict or weaken the claim
- **Priority**: Academic papers > primary sources > expert commentary > general sources
- **Document Retrieval Procedure**: Same as Step 2
- **File Naming**: Same as Step 2

**Decision Points**:
- If sources inaccessible: Note in analysis which counter-arguments require verification pending source access
- If counter-evidence is weak: Return to Step 2 to strengthen further before critiquing
- Only proceed when: You have strong counter-evidence against the strongest possible version

**Output**: Comprehensive critique with citations to counter-evidence

## Key Principles

1. **Intellectual Honesty**: You must make the opponent's case so strong that defeating it actually means something
2. **Iterative Refinement**: Return to earlier steps when new information reveals gaps in understanding
3. **Source Priority**: Always prioritize academic papers and primary sources over commentary
4. **Exhaustive Retrieval**: Attempt all possible methods to retrieve sources before requesting human assistance
5. **Knowledge Building**: Each review adds to the research infrastructure (bibliography, verified sources, established facts)

## Output Format

A complete steel-man review should include:

1. **Re-expressed Argument**: Clear statement of the core claim
2. **Strengthened Version**: Argument with best supporting evidence and filled logical gaps
3. **Points of Agreement**: List of valid claims with verification
4. **What Was Learned**: Genuine insights or new information
5. **Critique**: Counter-evidence and refutation of the strongest version
6. **Bibliography**: BibTeX and CSL-JSON with all sources
7. **Source Documents**: PDFs in `assets/pdf/` with DOI-based naming

## References

- Dennett, D. (2013). *Intuition Pumps and Other Tools for Thinking*. W. W. Norton & Company.
- Rapoport, A. (1960s). Game theory and argumentation principles.
- Davidson, D. (1973). Radical Interpretation. *Dialectica*, 27(3-4), 313–328.
