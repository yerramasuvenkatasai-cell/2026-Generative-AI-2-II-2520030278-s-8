# Research Papers

The following two papers are the primary references for Review-1. Their official public pages are linked below. Downloaded copies should only be added when their license or the course instruction permits it.

## Paper 1 — Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks

- **Authors:** Patrick Lewis, Ethan Perez, Aleksandra Piktus, et al.
- **Year:** 2020
- **Link:** https://arxiv.org/abs/2005.11401
- **Relevance:** Introduces the RAG approach of combining a language generator with retrieved external knowledge. It supports the core pipeline for retrieving official fee-document sections before answering a query.

## Paper 2 — Multilingual Retrieval-Augmented Generation for Knowledge-Intensive Question Answering Task

- **Authors:** Leonardo Ranaldi, Barry Haddow, and Alexandra Birch
- **Year:** 2026
- **Link:** https://aclanthology.org/2026.findings-eacl.35/
- **Relevance:** Studies RAG for multilingual question answering and compares multilingual retrieval strategies. It supports the need to evaluate language correctness and source consistency in a two-language fee assistant.

## How these papers inform the project

Paper 1 provides the RAG architecture: retrieve evidence, then generate an answer. Paper 2 provides guidance for multilingual use: test whether the answer is in the requested language and whether the retrieved content still supports the response. These findings lead to three project rules: use only approved source documents, display source references, and decline to answer when evidence is insufficient.

