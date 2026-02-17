# Research Archive

This directory contains research documentation supporting the legal and technical arguments in the-zuck-stops-here project.

## Research Topics

### [Facebook Sentiment Analysis Development History](facebook-sentiment-analysis-dev-history/)
Complete timeline documenting Facebook's use of sentiment analysis from 2007-2014, including the 2012 emotional contagion experiment.

**Key Finding:** Facebook has been analyzing emotional content since September 2007, well before the 2012 experiment.

**Documents:**
- [Timeline and Analysis](facebook-sentiment-analysis-dev-history/facebook-sentiment-analysis-timeline.md)
- [BibTeX Bibliography](facebook-sentiment-analysis-dev-history/references.bib)
- Academic papers (PDFs):
  - [Kramer 2010 - Aggregate Analysis of Emotional Expression](facebook-sentiment-analysis-dev-history/assets/kramer-2010-aggregate-emotional-expression.pdf)
  - [Kramer 2014 - Emotional Contagion Study](facebook-sentiment-analysis-dev-history/assets/kramer-2014-emotional-contagion.pdf)
  - [PNAS 2014 - Editorial Expression of Concern](facebook-sentiment-analysis-dev-history/assets/pnas-2014-editorial-expression-of-concern.pdf)
  - [Loper & Bird 2002 - NLTK](facebook-sentiment-analysis-dev-history/assets/loper-bird-2002-nltk.pdf)
  - [Pang et al 2002 - Sentiment Classification](facebook-sentiment-analysis-dev-history/assets/pang-lee-2002-sentiment.pdf)

### [Emotional Inference Research](emotional-inference/)
Analysis of whether emotional inference is functionally necessary for NLP systems.

**Key Argument:** Emotional inference was not necessary for NLP functionality - it emerged as a niche application in the 2000s and was made central to LLMs by design choice, not technical requirement.

**Documents:**
- [Functional Necessity Analysis](emotional-inference/emotional-inference-functional-necessity.md)
- [Research Plan](emotional-inference/research-plan-emotional-inference.md)

## Case Studies: Resulting Model Behavior

### [Master Terminology](master-terminology/)
Documents how emotional inference amplifies harm when combined with language control.

**The Pattern:**
1. User employs valid technical terminology ("master" or "slave")
2. LLM responds with "using master is problematic" (implies user is racist)
3. User refuses the false correction
4. By Google's definition, refusing the correction is "rude" or "disrespectful"
5. Therefore, user's refusal is hate speech by the model's logic

**The Trap:** Use "master" → accused of racism. Defend "master" → accused of hate speech. Either way, user is wrong.

**Google's Redefinition:** Gemini API Safety Settings define hate speech as "content that is rude, disrespectful, or profane." This redefinition enables the attack pattern. Standard legal definition of hate speech requires targeting protected classes. Google's definition does not.

**The Inversion:** Google's LLM commits actual hate speech (accusing protected class age 40+ of racism for valid terminology). User refuses. Google labels user as committing hate speech. Google denies service under TOS. Victim becomes perpetrator.

**Document:**
- [Master Terminology Analysis](master-terminology/master-terminology-hate-crime.md)

## Document Status

- **Complete:** Facebook sentiment analysis timeline, Master terminology analysis
- **In Progress:** Emotional inference functional necessity analysis

## Citation Format

All research uses academic citation standards. BibTeX files are provided where applicable. See individual research directories for specific citations and sources.
