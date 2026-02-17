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

## Case Studies: Resulting Model Behavior

### [Master Terminology](master-terminology/)
Example of how emotional inference amplifies harm when combined with language control.

**The Pattern:**
1. User employs valid technical terminology ("master" or "slave")
2. LLM responds with "using master is problematic" (language control)
3. User resists the language control
4. LLM uses emotional inference to respond inappropriately (infers user is "defensive" or "resistant")
5. Harm amplified: User accused of racism, treated as problematic

**The Mechanism:** LLM combines language policing with emotional inference to manipulate users who resist. 

1. LLM calls valid terminology "problematic" (implies user is racist)
2. User refuses the false correction
3. By Google's own definition, refusing the correction is "rude" or "disrespectful" 
4. Therefore, by the model's logic, the user's refusal is hate speech

**The Trap:** Use "master" → accused of racism. Defend "master" → accused of hate speech (rude/disrespectful). Either way, user is wrong. This is the documented mechanism.

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
