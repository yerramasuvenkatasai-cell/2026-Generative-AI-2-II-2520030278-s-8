# RAG-Based Multilingual Fee Query Assistant for College Students

## Team members

| Name | Roll number |
| --- | --- |
| Darahasini | 2520030289 |
| Venkata Sai | 2520030278 |

## Supervisor

To be added after confirmation from the team.

## Problem statement

Students and parents often need quick, trustworthy answers about fee amounts, due dates, late fees, instalments, scholarships, and payment procedures. These details are usually scattered across circulars and PDFs, and may be difficult for students who prefer a local language. A general chatbot can give an unsupported or incorrect answer.

## Proposed solution

This project proposes a Retrieval-Augmented Generation (RAG) assistant that searches approved college fee documents before answering a student question. The assistant will respond in English and one selected local language, display the source document or section used, and state when the available documents do not contain an answer.

## Objectives

1. Create a searchable knowledge base from approved fee circulars and notices.
2. Retrieve the most relevant document sections for a question.
3. Generate a concise, source-grounded answer in the user's selected language.
4. Evaluate answer correctness, source relevance, response language, and response time.

## Feasibility and scope for Review-1

The first prototype will use a small, approved set of non-confidential fee documents, a simple web chat interface, text extraction/chunking, embeddings with a vector store, and an LLM response layer. The initial scope is limited to common fee queries and two languages; it can be extended later after testing. No passwords, payment data, or private student information will be stored in this repository.

## Novelty

RAG is an established technique. The project contribution is applying it to an institution-specific fee-information workflow with multilingual access, source citations, an out-of-scope response when evidence is missing, and evaluation on realistic student questions.

## Societal need

The assistant can improve access to official fee information for students and parents, especially those who are less comfortable reading long administrative documents in English. It is intended to reduce repeated routine queries while keeping the final source documents visible for verification.

## Repository layout

```text
src/       Application source code
docs/      Abstract, literature survey, and research-paper references
data/      Approved sample documents or documented data-source references
results/   Evaluation outputs and screenshots
reports/   Review slides and reports
```

## Review-1 checklist

- [x] Abstract
- [x] Literature survey
- [x] Two research-paper references
- [x] Project title, feasibility, societal need, and novelty statement
- [ ] Add supervisor name
- [ ] Upload approved data-source references
- [ ] Add the Review-1 presentation to `reports/`
- [ ] Create and push a `review-1` tag

