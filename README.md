# autogen-agent-framework

Conversational multi-agent patterns using Microsoft AutoGen for collaborative problem-solving.

## What this covers

- **Agent configurations** - AssistantAgent, UserProxyAgent, and GroupChat setups
- **Conversation patterns** - Two-agent dialogues, group chats, and nested conversations
- **Code execution** - Sandboxed code generation and execution within agent conversations
- **Function calling** - Agents that call external APIs and tools during conversations

## Stack

- Python 3.10+
- AutoGen (pyautogen)
- OpenAI, Anthropic
- Docker (for sandboxed execution)
- pytest, ruff

## Structure

```
agents/          # Agent configurations and system messages
conversations/   # Conversation flow definitions
functions/       # Callable functions exposed to agents
executors/       # Code execution sandboxes
tests/           # Conversation replay tests
examples/        # Demo conversations
```

## Setup

```bash
pip install -e .
cp .env.example .env
pytest
```

## License

MIT
