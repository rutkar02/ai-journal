# Project 10 - My First MCP Server & Client

## What I Built

Built an MCP server exposing a calculator tool and a Python MCP client capable of:

- Starting the server
- Establishing an MCP session
- Initializing the protocol
- Discovering available tools
- Calling a tool
- Receiving the result

---

## Architecture

Python Client
        │
        ▼
STDIO Transport
        │
        ▼
MCP Server
        │
        ▼
Python Tool

---

## Biggest Things I Learned

- MCP standardizes communication between AI clients and tools.
- FastMCP automatically generates tool schemas using Python introspection.
- Clients don't need hardcoded tool definitions.
- Tool discovery happens dynamically through `list_tools()`.
- Tool execution happens through `call_tool()`.
- The protocol begins with an initialization handshake.

---

## Biggest Realization

MCP does not replace Tool Calling.

It replaces manually distributing tool definitions.

Previously:

tools = [...]

Now:

tools = await session.list_tools()

The LLM receives exactly the same information.

Only the source of that information changed.

---

## Mental Model

Tool Calling answers:

"How does an AI use a tool?"

MCP answers:

"How does an AI discover tools?"

Together they form a complete system.

---

## Engineering Lesson

Frameworks evolve.

Architectures remain.

Even though the SDK API differed from my expectations, the overall flow never changed:

Connect

↓

Initialize

↓

Discover

↓

Execute

Understanding the architecture made adapting to the SDK straightforward.