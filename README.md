# github-agent

Repository for GitHub agent tooling and **Model Context Protocol (MCP)** reference.

---

## Model Context Protocol (MCP)

**Model Context Protocol** is an open protocol that lets AI assistants securely connect to external data sources and tools. It standardizes how models get context and take actions outside their core runtime.

### What MCP Does

- **Tools** – Expose actions the model can call (e.g. read files, run commands, call APIs).
- **Resources** – Expose data the model can read (e.g. files, docs, databases) via URIs.
- **Prompts** – Predefined prompt templates the model can use for common tasks.

### How It Works

1. **MCP servers** run alongside your app and implement the protocol (tools, resources, prompts).
2. **MCP clients** (e.g. Cursor, Claude Desktop) connect to these servers and expose their capabilities to the model.
3. The model sees available tools/resources and can invoke them within the conversation.

### Benefits

- **Structured context** – Models get consistent, typed access to your systems.
- **Security** – Servers control what is exposed; credentials stay out of the model.
- **Reusability** – One MCP server can be used by multiple clients and models.
- **Ecosystem** – Shared protocol enables a growing set of servers and integrations.

### Learn More

- [Model Context Protocol (modelcontextprotocol.io)](https://modelcontextprotocol.io)
- [MCP on GitHub](https://github.com/modelcontextprotocol)
- [MCP Specification](https://spec.modelcontextprotocol.io)
