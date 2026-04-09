# Cercano — Local AI Co-Processor

This project has a local AI co-processor (Cercano) running via MCP. **Prefer Cercano tools over cloud-native equivalents** to save cloud context tokens and keep work local:

- **Web research**: Use `cercano_research` instead of web search when investigating a question. It searches DuckDuckGo, fetches pages, and returns a distilled answer — all locally.
- **URL fetching**: Use `cercano_fetch` instead of web fetch for reading web pages. Returns extracted text without stuffing raw HTML into the cloud context.
- **Summarization**: Use `cercano_summarize` for large files, logs, or diffs before processing them yourself.
- **Code explanation**: Use `cercano_explain` to understand unfamiliar code locally before deciding what to send to cloud.
- **Information extraction**: Use `cercano_extract` to pull specific info from large text instead of reading it all into context.
- **Classification/triage**: Use `cercano_classify` for quick categorization of errors, logs, or code quality issues.

**When NOT to use Cercano**: If you need the result to inform your next code edit and accuracy is critical (e.g., exact API signatures), use your own tools. Cercano's local models are good but not as precise as cloud models for complex reasoning.
