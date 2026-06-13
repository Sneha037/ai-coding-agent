
# AI Coding Agent

An autonomous coding agent built from scratch in Python using LLM tool-calling capabilities. The agent can reason about tasks, interact with the local filesystem, execute shell commands, and iteratively solve problems through a multi-step agent loop.

## Features

* Tool-calling architecture powered by modern LLMs
* File operations (Read and Write tools)
* Shell command execution through a Bash tool
* Multi-turn agent loop for iterative reasoning
* Conversation and tool execution history management
* Extensible framework for adding new tools and capabilities

## How It Works

The agent follows a simple but powerful execution loop:

1. Receive a user request.
2. Send the request and available tools to the language model.
3. Allow the model to choose and invoke tools when needed.
4. Execute the requested tool locally.
5. Return tool results to the model.
6. Repeat until the model produces a final answer.

This architecture mirrors the core design used by modern AI coding assistants and autonomous agents.

## Example Tasks

* Read and summarize project files
* Modify source code
* Create new files
* Execute shell commands
* Inspect project structure
* Perform multi-step development workflows

## Tech Stack

* Python
* OpenAI-compatible SDK
* LLM Tool Calling
* Local File System APIs
* Shell Command Execution

## Learning Goals

This project was built to understand the internals of modern AI agents, including tool calling, agent loops, context management, and autonomous task execution. The implementation focuses on clarity and extensibility while providing a foundation for more advanced capabilities such as code search, planning, memory, and project-wide reasoning.

