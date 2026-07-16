# Project 5 - Multi PDF RAG

## What I Built

Extended my PDF chatbot to support multiple uploaded documents simultaneously.

---

## Architecture

Multiple PDFs
↓
Extract Text
↓
Chunk
↓
Embeddings
↓
Combined Retrieval
↓
LLM

---

## Biggest Things I Learned

- Data structures become increasingly important.
- Metadata improves retrieval.
- Caching saves unnecessary computation.

---

## Mental Models

- Every chunk belongs to a document.
- Metadata provides context beyond the text itself.
- Scaling usually means better organization, not more code.

---

## Biggest Mistakes

- Initially processed PDFs twice.
- Didn't preserve document identity.

---

## What I Can Build Now

- Enterprise knowledge search
- Company documentation assistants
- Multi-document research tools