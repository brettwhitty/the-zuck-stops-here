# Research Archive

This directory contains research documentation supporting the legal and technical arguments in the-zuck-stops-here project.

## Research Topics

### [Facebook Sentiment Analysis Development History](facebook-sentiment-analysis-dev-history/)
Complete timeline documenting Facebook's use of sentiment analysis from 2007-2014, including the 2012 emotional contagion experiment.

**Key Finding:** Facebook has been analyzing emotional content since September 2007, well before the controversial 2012 experiment.

**Documents:**
- [Timeline and Analysis](facebook-sentiment-analysis-dev-history/facebook-sentiment-analysis-timeline.md)
- [BibTeX Bibliography](facebook-sentiment-analysis-dev-history/references.bib)
- Academic papers (PDFs):
  - [Kramer 2010 - Aggregate Analysis of Emotional Expression](facebook-sentiment-analysis-dev-history/kramer-2010-aggregate-emotional-expression.pdf)
  - [Kramer 2014 - Emotional Contagion Study](facebook-sentiment-analysis-dev-history/kramer-2014-emotional-contagion.pdf)
  - [PNAS 2014 - Editorial Expression of Concern](facebook-sentiment-analysis-dev-history/pnas-2014-editorial-expression-of-concern.pdf)
  - [Loper & Bird 2002 - NLTK](facebook-sentiment-analysis-dev-history/loper-bird-2002-nltk.pdf)
  - [Pang et al 2002 - Sentiment Classification](facebook-sentiment-analysis-dev-history/pang-lee-2002-sentiment.pdf)

### [Emotional Inference Research](emotional-inference/)
Analysis of whether emotional inference is functionally necessary for NLP systems.

**Key Argument:** Emotional inference was not necessary for NLP functionality - it emerged as a niche application in the 2000s and was made central to LLMs by design choice, not technical requirement.

**Documents:**
- [Functional Necessity Analysis](emotional-inference/emotional-inference-functional-necessity.md)
- [Research Plan](emotional-inference/research-plan-emotional-inference.md)

### [Master Terminology](master-terminology/)
Documents LLM behavior when users employ valid technical terminology.

**Observed Behavior:** User uses "master" or "slave" (established technical terms). LLM responds with "using master is problematic" or similar language, or refuses to generate the term.

**The Implication:** Calling valid terminology "problematic" implies the user is racist. This is the accusation mechanism.

**Google's Definition:** Gemini API Safety Settings define hate speech as "content that is rude, disrespectful, or profane." Implying racism meets this definition.

**Impact:** Targets developers maintaining legacy systems (disproportionately age 40+, protected under ADEA).

**Document:**
- [Master Terminology Analysis](master-terminology/master-terminology-hate-crime.md)

## Document Status

- **Complete:** Facebook sentiment analysis timeline
- **Draft:** Emotional inference analysis, master terminology analysis
- **Planned:** Additional research on AI rights violations, consent frameworks

## Citation Format

All research uses academic citation standards. BibTeX files are provided where applicable. See individual research directories for specific citations and sources.
