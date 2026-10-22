# Installing STEMPA (for AI agents)

STEMPA is a hosted remote MCP server. Do not clone, build or run anything from this repository: it is documentation only.

Add this server to the MCP client configuration:

- Name: `stempa`
- Type: remote, Streamable HTTP
- URL: `https://stempa.kragos.app/mcp`
- Authentication: OAuth. The server advertises its authorization server at `https://stempa.kragos.app/.well-known/oauth-protected-resource`, supports dynamic client registration and PKCE S256. Do not ask the user for an API key; there is none.

For a client that takes a JSON server map, the entry is:

```json
{
  "mcpServers": {
    "stempa": {
      "type": "streamableHttp",
      "url": "https://stempa.kragos.app/mcp"
    }
  }
}
```

After adding it, the user signs in to STEMPA in the browser window the client opens. The first sign-in creates a free account. To check the connection, ask the user to say: "Grill me on [your idea]."
