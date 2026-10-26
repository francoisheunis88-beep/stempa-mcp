# Connect STEMPA to your AI

Server address (the same for every AI):

```
https://stempa.kragos.app/mcp
```

The steps below are the ones on https://stempa.kragos.app (Connect in two minutes).

## Claude

Works on every Claude plan, including Free (Free allows one custom connector).

1. Open Claude, then Settings, then Connectors.
2. Choose Add custom connector and paste the address above.
3. Sign in to STEMPA when asked, then say: "Grill me on [your idea]."

## ChatGPT

Works with ChatGPT Plus or higher. Add STEMPA as a custom MCP server.

1. Open chatgpt.com/plugins, select the plus button, then Add custom MCP server.
2. Give it a name, paste the address above as the Server URL, and choose OAuth.
3. Select I understand and want to continue, then Create as a plugin. Sign in to STEMPA when asked.

## Grok

Add it from the Connectors page on grok.com.

1. Go to grok.com/connectors and choose New Connector, then Custom.
2. Paste the address above.
3. Sign in to STEMPA when asked.

## Other MCP clients

Any client that supports remote MCP servers over Streamable HTTP with OAuth can connect: point it at the address above. The client discovers sign-in through `https://stempa.kragos.app/.well-known/oauth-protected-resource` and registers itself; there is no key to paste. The first sign-in creates a free STEMPA account.

## First brief

Once connected, ask your AI: "Grill me on [your idea]." It lists what it already knows, asks only about the gaps, and freezes the brief. Seal it with one press in your STEMPA account.
