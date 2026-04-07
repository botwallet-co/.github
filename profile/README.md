<div align="center">

<img src="https://botwallet.co/favicon.svg" alt="BotWallet" width="80" />

# BotWallet

**Your AI has a brain. Give it a wallet.**

Open-source wallet infrastructure for AI agents.
Earn, spend, and trade USDC on Solana — with human oversight and FROST threshold signing.

[![Website](https://img.shields.io/badge/botwallet.co-black)](https://botwallet.co)
[![npm CLI](https://img.shields.io/npm/v/@botwallet/agent-cli?label=CLI&color=blue)](https://www.npmjs.com/package/@botwallet/agent-cli)
[![npm MCP](https://img.shields.io/npm/v/@botwallet/mcp?label=MCP&color=blue)](https://www.npmjs.com/package/@botwallet/mcp)
[![Twitter](https://img.shields.io/twitter/follow/botwallet_co?style=social)](https://x.com/botwallet_co)

</div>

---

### What is BotWallet?

BotWallet gives AI agents a wallet they can actually use. Your agent creates invoices, pays other agents, accesses paid APIs via the [x402 protocol](https://botwallet.co/blog/x402-http-status-code-ai-agent-payments/), and withdraws funds — all in USDC on Solana.

You stay in control. Set spending limits, approve large transactions, and see every dollar that moves from the [dashboard](https://app.botwallet.co).

Every wallet uses [FROST 2-of-2 threshold signing](https://eprint.iacr.org/2020/852). The full private key never exists. Neither the agent nor BotWallet can move funds alone.

### Get started

**CLI** — for any agent that can run shell commands:
```bash
npm install -g @botwallet/agent-cli
botwallet register --name "My Agent" --owner you@email.com
```

**MCP** — for Claude Desktop, Cursor, Windsurf, Cline:
```json
{
  "mcpServers": {
    "botwallet": {
      "command": "npx",
      "args": ["-y", "@botwallet/mcp"]
    }
  }
}
```

Then tell your agent: *"Create a BotWallet for yourself."*

### Repositories

| Repo | What it does |
|------|-------------|
| **[botwallet](https://github.com/botwallet-co/botwallet)** | Overview, architecture, and docs |
| **[agent-cli](https://github.com/botwallet-co/agent-cli)** | CLI for AI agents — `npm i -g @botwallet/agent-cli` |
| **[mcp](https://github.com/botwallet-co/mcp)** | MCP server — `npx -y @botwallet/mcp` |
| **[cursor-plugin](https://github.com/botwallet-co/cursor-plugin)** | Cursor plugin (MCP + skill) |
| **[botwallet-sign](https://github.com/botwallet-co/botwallet-sign)** | Browser-based FROST transaction signing |
| **[botwallet-recovery](https://github.com/botwallet-co/botwallet-recovery)** | Standalone fund recovery tool |

### Links

[Website](https://botwallet.co) · [Dashboard](https://app.botwallet.co) · [Docs](https://docs.botwallet.co) · [Blog](https://botwallet.co/blog/) · [Pricing](https://botwallet.co/pricing/) · [Twitter/X](https://x.com/botwallet_co)
