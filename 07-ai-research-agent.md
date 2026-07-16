# Project 7 - AI Research Agent

## What I Built

Built an AI agent using OpenAI Tool Calling.

---

## Architecture

User
↓
LLM
↓
Function Call
↓
Python
↓
Tool
↓
LLM
↓
Answer

---

## Biggest Things I Learned

- A tool is metadata describing a Python function.
- The model reasons.
- Python orchestrates.
- Tools execute.
- Arguments arrive as JSON strings.
- json.loads() converts them into dictionaries.
- previous_response_id continues the conversation.

---

## Biggest Mistakes

- Tried parsing strings.
- Mixed message history with Responses API.
- Forgot json.loads().

---

## What I Can Build Now

- Research Agent
- Weather Agent
- Calculator Agent
- Database Agent
- Multi-tool Agent