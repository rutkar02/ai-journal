# Project 3 - AI Chatbot

## What I Built

Built a conversational chatbot using the OpenAI Responses API and Streamlit.

---

## Architecture

User
↓
LLM
↓
Response

---

## Biggest Things I Learned

- Messages maintain conversation history.
- Roles have different responsibilities.
- Streamlit reruns the script after every interaction.
- Session State preserves memory.

---

## Mental Models

- Conversation history is the chatbot's memory.
- The LLM is stateless unless we provide previous context.
- Session State acts like RAM for a Streamlit app.

---

## Biggest Mistakes

- Lost conversation history because of Streamlit reruns.
- Confused local variables with session state.

---

## What I Can Build Now

- AI chatbots
- Customer support assistants
- FAQ bots
- Personal AI assistants