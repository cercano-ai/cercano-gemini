# Cercano — Gemini CLI Extension

Local-first AI co-processor for Gemini CLI. Offload research, summarization, extraction, and more to local models via Ollama.

## Prerequisites

- [Cercano](https://github.com/bryancostanich/Cercano) installed and on your PATH (`brew install bryancostanich/cercano/cercano`)
- [Ollama](https://ollama.com/) running with at least one model pulled

## Install

```bash
gemini extensions install https://github.com/bryancostanich/cercano-gemini
```

## Custom Commands

- `/research <topic>` — Research a topic using Cercano's local AI pipeline
- `/fetch <url>` — Fetch and extract text from a URL locally

## Configuration

Set a custom Ollama URL:

```bash
gemini extensions config cercano "Ollama URL" --value "http://my-server:11434"
```

## What It Does

Cercano runs inference locally via Ollama, keeping your data private and saving cloud tokens. See the [main Cercano repo](https://github.com/bryancostanich/Cercano) for full documentation.

## License

MIT
