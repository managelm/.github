<p align="center">
  <a href="https://www.managelm.com">
    <img src="https://www.managelm.com/assets/ManageLM.png" alt="ManageLM" height="60">
  </a>
</p>

<h3 align="center">Manage Linux & Windows servers with natural language</h3>

<p align="center">
  <a href="https://www.managelm.com">Website</a> &middot;
  <a href="https://app.managelm.com">Cloud Portal</a> &middot;
  <a href="https://app.managelm.com/doc/">Documentation</a> &middot;
  <a href="https://app.managelm.com/register">Sign Up Free</a>
</p>

---

ManageLM is an AI-powered platform for managing Linux and Windows servers using natural language. Install a lightweight agent on your servers, connect through the cloud portal or your favorite AI tool, and describe what you need — the agent handles the rest.

```
> install nginx, enable it, and open port 443
✓ packages: Installed nginx 1.26.2
✓ services: nginx is active and enabled
✓ firewall: HTTPS (443/tcp) opened
```

### How it works

```
AI Client ──────> ManageLM Portal ── WebSocket ──> Agent on Server
(Claude, ChatGPT,   (cloud control      (outbound      (local LLM,
 VS Code, Slack,      plane)              only)          32 skills)
 n8n, OpenClaw)
```

- **Agents** run on your servers with a local LLM — your data never leaves your infrastructure
- **Zero inbound ports** — agents connect outbound only, no SSH needed
- **32 built-in skills** — packages, services, firewall, Docker, databases, certificates, users, and more
- **4-layer security** — injection blocking, command allowlisting, destructive guards, kernel sandbox
- **Compliance frameworks** — CIS, HIPAA, ISO 27001, NIST CSF, NIS2, PCI DSS

### Repositories

| Repository | Description |
|---|---|
| [**linux-windows-agent**](https://github.com/managelm/linux-windows-agent) | Lightweight Python agent with local LLM, 32 skills, and multi-step planner |
| [**claude-extension**](https://github.com/managelm/claude-extension) | MCP extension for Claude Code and Claude Desktop |
| [**vscode-extension**](https://github.com/managelm/vscode-extension) | `@managelm` participant for VS Code Copilot Chat |
| [**openai-gpt**](https://github.com/managelm/openai-gpt) | Custom GPT for ChatGPT with OpenAI Actions |
| [**n8n-plugin**](https://github.com/managelm/n8n-plugin) | Community node for n8n — 51 actions and event triggers |
| [**slack-plugin**](https://github.com/managelm/slack-plugin) | Slack bot with real-time alerts and slash commands |
| [**openclaw-plugin**](https://github.com/managelm/openclaw-plugin) | Plugin for OpenClaw with 17 tools |
| [**custom-skills**](https://github.com/managelm/custom-skills) | Community-contributed skills for ManageLM agents |

### Get started

1. [Create a free account](https://app.managelm.com/register) (up to 10 agents)
2. Install the agent: `curl -fsSL https://app.managelm.com/install | bash`
3. Connect through [Claude](https://github.com/managelm/claude-extension), [VS Code](https://github.com/managelm/vscode-extension), [ChatGPT](https://github.com/managelm/openai-gpt), or the [portal](https://app.managelm.com)
