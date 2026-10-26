# STEMPA

**Brief your AI once. Seal it.**

STEMPA is a remote MCP server. Your AI first lists what it already knows about a job, then asks you only about the gaps: up to five questions at a time, each with a suggested answer. You answer once, and STEMPA seals your answers into one brief with a signed receipt. Change a word and it becomes a new version.

Works with Claude, ChatGPT (Plus or higher) and Grok.

- Server address: `https://stempa.kragos.app/mcp`
- Transport: Streamable HTTP
- Sign-in: OAuth 2.1 with dynamic client registration and PKCE. There is no key to paste.
- Website: https://stempa.kragos.app
- Official MCP Registry name: `app.kragos/stempa` (see [`server.json`](server.json))

This repository is documentation only. STEMPA is a hosted service; there is nothing to install or run locally.

## Connect

STEMPA works with Claude, ChatGPT (Plus or higher) and Grok; step-by-step instructions for each are in [CONNECT.md](CONNECT.md). In short: paste `https://stempa.kragos.app/mcp` into your AI's connectors, and sign in to STEMPA when asked.

Any other MCP client that supports remote servers with OAuth connects the same way: add a remote server with the address `https://stempa.kragos.app/mcp`. The client finds the sign-in itself; there is no key to paste. In a client that reads an `mcp.json` file, the entry looks like this:

```json
{
  "servers": {
    "stempa": {
      "type": "http",
      "url": "https://stempa.kragos.app/mcp"
    }
  }
}
```

The first sign-in creates a free STEMPA account.

## Use it

1. Say to your AI: "Grill me on [your idea]."
2. Your AI lists what it already knows, then asks only about the gaps: up to five questions at a time, each with a suggested answer. Accept the suggestion, pick an option, or type your own.
3. When the gaps are closed, your AI freezes the brief.
4. Open your account at https://stempa.kragos.app and press Seal. The brief gets a fingerprint and a signed receipt.
5. Later, in any AI you connect, ask it to read your sealed brief. It reads the same sealed version.

## Tools

`grill_start`, `grill_map`, `grill_gaps`, `grill_answer`, `grill_freeze`, and tools that read your briefs back.

## How a brief is sealed

1. **Connect.** Add STEMPA to the AI you already use.
2. **Answer.** Your AI lists what it already knows, then asks only about the gaps. Pick an option, accept the suggestion, or type your own.
3. **Seal.** Your AI freezes the brief; you seal it with one press in your STEMPA account. The sealed brief gets a fingerprint and a receipt with post-quantum signatures. Anyone you share a receipt with can check it on the receipt page.

A sealed brief is a record of the scope you agreed.

## Plans

Start free: 14 days of Pro, then Free: 5 sealed briefs a month, kept 30 days. No card. Current plans are on https://stempa.kragos.app.

## Support

Use the contact details on https://stempa.kragos.app. STEMPA is supplied by KRAGOS, South Africa.
