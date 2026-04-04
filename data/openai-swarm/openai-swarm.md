## Overview

Swarm is a lightweight, experimental multi-agent framework from OpenAI designed for prototyping. It uses a routine-based model where agents are defined through prompts and function docstrings, relying on natural language routines and sequential handoffs.

## Architecture

- **Routine-Based Model**: Agents are defined through prompts and function docstrings
- **Sequential Handoffs**: Agents work sequentially, transferring tasks while maintaining shared context
- **No Formal Orchestration**: Does not have built-in orchestration or state models; relies on manually structured workflows

## Features

- **Natural Language Function Definitions**: Function behavior is inferred by the LLM through docstrings; Swarm identifies what a function does by reading its description
- **Python Tool Integration**: Uses Python tools for flexible workflows
- **Flexible but Less Precise**: No formal orchestration or state models make the setup flexible but less structured than alternatives
- **MCP Integration**: Benefits from OpenAI's native MCP support across its ecosystem; leverages infrastructure from ChatGPT and OpenAI Agents SDK
- **Stateless by Default**: Does not manage memory natively; developers can pass short-term memory through context_variables manually and optionally integrate external tools (e.g., mem0) for longer-term context

## Limitations

- **No Built-in Human-in-the-Loop**: Offers no native HITL support
- **No Native Memory Management**: Completely stateless; all memory must be handled externally
- **No Formal State Models**: Lacks the structured state machines or conversation loops of more robust frameworks
- **Experimental Status**: Designed primarily for prototyping rather than production deployments

## Best Use Cases

- Rapid prototyping of multi-agent systems
- Simple sequential workflows with clear handoff patterns
- Projects already in the OpenAI ecosystem leveraging native MCP support
- Lightweight agent experiments where flexibility is prioritized over structure