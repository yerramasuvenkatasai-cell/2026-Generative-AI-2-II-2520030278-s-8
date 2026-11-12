# Literature Survey

## 1. Background

Large language models can answer questions fluently, but may generate unsupported statements when they lack reliable context. Retrieval-Augmented Generation (RAG) addresses this by retrieving relevant text from an external knowledge collection before generating an answer. For a fee-information assistant, this makes official circulars and notices the evidence base instead of relying only on a model's stored knowledge.

## 2. Retrieval-Augmented Generation

Lewis et al. (2020) introduced RAG models that combine a generator with a retrieved non-parametric knowledge source. The work motivates the main design of this project: retrieve relevant document passages first, then use the retrieved evidence to formulate an answer. The project will require that the generated answer is based only on the retrieved approved fee documents.

## 3. Multilingual RAG

Ranaldi, Haddow, and Birch (2026) investigate RAG for multilingual knowledge-intensive question answering. Their study highlights that multilingual retrieval and answer generation require deliberate evaluation because translations and cross-language contexts can introduce inconsistency. In this project, the initial prototype will use two languages and test both response language correctness and whether the cited source supports the answer.

## 4. Research gap and proposed contribution

Existing RAG research largely evaluates broad open-domain question answering. The proposed system focuses on a narrow administrative domain: official college fee information. Its practical contribution is to provide multilingual access, show sources, avoid answering when evidence is absent, and test the system with realistic student fee queries. The project does not claim that RAG itself is novel; its novelty is the transparent, institution-focused application and evaluation.

## 5. Proposed methodology

1. Collect only approved, non-confidential fee notices and circulars.
2. Extract text and divide it into meaningful sections with document and page metadata.
3. Create multilingual embeddings and store the sections in a vector database.
4. Retrieve the most relevant sections for each user question.
5. Prompt a language model to answer only from the retrieved evidence and return source references.
6. Evaluate retrieval relevance, answer correctness, citation coverage, language correctness, and response time.

## References

1. Lewis, P., Perez, E., Piktus, A., et al. (2020). *Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks.* arXiv:2005.11401. https://arxiv.org/abs/2005.11401
2. Ranaldi, L., Haddow, B., & Birch, A. (2026). *Multilingual Retrieval-Augmented Generation for Knowledge-Intensive Question Answering Task.* Findings of EACL 2026, 697–716. https://aclanthology.org/2026.findings-eacl.35/

