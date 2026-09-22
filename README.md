# Aagam Bandi

**LLM systems and data engineering.** B.Tech, IIT Roorkee. Previously ML/AI intern at Immverse AI, where I built multilingual RAG over Sanskrit scripture — Qdrant, Phi-4, query rewriting, and a validation agent that checked the retrieval instead of trusting it.

I work on the parts of AI systems that don't demo well — pipelines that fail loudly instead of quietly, retrieval that returns the right chunk, and the evaluation that tells you whether any of it actually helped.

---

### Projects

**[Automated Metadata Extractor](https://github.com/Aagam-Bandi/automated-metadata-extractor)** · `Gemini` `LangChain` `ChromaDB` `OCR`
Structured metadata from PDFs, DOCX and scanned documents. Selective per-page OCR, and a self-querying retrieval step where the document generates the questions used to find its own metadata. Ships with a rubric-based evaluation harness — exact match, Jaccard, and embedding similarity, scored per field.

**[Meeting Intelligence](https://github.com/Aagam-Bandi/meeting-intelligence)** · `Gemini` `LangChain` `ChromaDB` `asyncio`
Executive briefings and attributed action items from long transcripts, plus retrieval Q&A across them. Map-reduce summarisation with bounded concurrency and jittered retries. The eval harness measures decision coverage, owner attribution, and — the one that matters — whether the system correctly abstains on questions the transcript never covered.

**[Credit Default Risk Model](https://github.com/Aagam-Bandi/credit-default-risk)** · `XGBoost` `scikit-learn` `SMOTE`
Default prediction on 25k customers at a 19% base rate. AUC 0.79 after tuning, with isotonic calibration bringing max probability deviation from 0.34 to 0.035. Mostly an exercise in not being fooled: leak-free resampling, cost-sensitive thresholds, cross-validated confidence intervals.

**[Stock Sentiment Backtest](https://github.com/Aagam-Bandi/stock-sentiment-backtest)** · `NLTK` `pandas` `yfinance`
A post-mortem. This pipeline originally reported a Sharpe ratio of 1.25; the repo documents the three bugs that produced it — inverted trade accounting, a classifier trained on its own labels, and a join that silently discarded 95% of the data — and rebuilds it with the instrumentation that would have caught all three.

---

### Stack

**Languages** Python · SQL · C++
**LLM / AI** LangChain · Gemini · RAG architectures · ChromaDB · Qdrant · embedding models · async orchestration · prompt design · eval harness design
**Data** ClickHouse · MySQL · PostgreSQL · Elasticsearch · pandas · NumPy
**ML** scikit-learn · XGBoost · imbalanced-learn · feature engineering · calibration · cost-sensitive evaluation
**Other** Scrapy · Flask · Gradio · Mixpanel · pytest

---

### Open to

Contract work on LLM pipelines, document extraction, and evaluation infrastructure.

📧 aagambandi@gmail.com
