# Project 6 - YouTube Video Q&A

## What I Built

Built a RAG application capable of answering questions about YouTube videos using transcripts.

---

## Architecture

YouTube URL
↓
Video ID
↓
Transcript
↓
Chunk
↓
Embeddings
↓
Similarity Search
↓
LLM

---

## Biggest Things I Learned

- Video ID is the canonical identifier.
- URLs can change while IDs remain stable.
- Transcripts become documents in a RAG pipeline.
- Retrieval works identically across different data sources.

---

## Mental Models

- RAG doesn't care whether text comes from PDFs, videos or websites.
- Every information source eventually becomes text.
- The retrieval pipeline stays the same.

---

## Biggest Mistakes

- Cached using the URL instead of the Video ID.
- Triggered old questions when changing videos.
- Didn't initially understand transcript structure.

---

## What I Can Build Now

- YouTube tutors
- Lecture assistants
- Podcast search
- Meeting transcript assistants