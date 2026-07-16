# Project 8 - Chat with PDF using ChromaDB

## What I Built

Replaced my in-memory vector store with ChromaDB to build a production-style Retrieval-Augmented Generation (RAG) system.

---

## Architecture

PDF
↓
Extract Text
↓
Chunk
↓
Embeddings
↓
ChromaDB
↓
Semantic Search
↓
LLM

---

## Biggest Things I Learned

- A vector database replaces manual similarity search.
- ChromaDB stores documents, embeddings, IDs and metadata.
- Querying a vector database is much simpler than implementing cosine similarity manually.
- Batch insertion is more efficient than inserting one chunk at a time.
- Vector databases persist information and support efficient retrieval.

---

## Mental Models

- A vector database is to embeddings what SQL is to tables.
- The embedding tells the database where information lives.
- Databases encapsulate complex algorithms behind simple APIs.
- Good abstractions remove code while improving capability.

---

## Biggest Mistakes

- Initially tried storing vectors in Python lists.
- Forgot that Chroma collections persist between runs.
- Passed the entire query result instead of only the retrieved documents.
- Didn't initially think about duplicate insertions.

---

## What I Can Build Now

- Enterprise RAG
- Large document search
- Persistent knowledge bases
- Multi-document semantic search