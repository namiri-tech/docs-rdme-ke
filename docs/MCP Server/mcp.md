---
title: MCP
excerpt: 'MCP: Model Context Protocol'
hidden: false
---
The DigiTax Kenya API Hub Model Context Protocol (MCP) server enables AI-powered code editors like Cursor and Windsurf, plus general-purpose tools like Claude Desktop, to interact directly with your DigiTax Kenya API Hub API and documentation.

## What is MCP?

Model Context Protocol (MCP) is an open standard that allows AI applications to securely access external data sources and tools. The DigiTax Kenya API Hub MCP server provides AI agents with:

* **Direct API access** to DigiTax Kenya API Hub functionality
* **Documentation search** capabilities
* **Real-time data** from your DigiTax Kenya API Hub account
* **Code generation** assistance for DigiTax Kenya API Hub integrations

## DigiTax Kenya API Hub MCP Server Setup

DigiTax Kenya API Hub hosts a remote MCP server at `https://ke.docs.digitax.tech/mcp`. Configure your AI development tools to connect to this server. If your APIs require authentication, you can pass in headers via query parameters or however headers are configured in your MCP client.

<Tabs>
  <Tab title="Cursor">
    **Add to `~/.cursor/mcp.json`:**

    ```json
    {
      "mcpServers": {
        "dgtx-ke": {
          "url": "https://ke.docs.digitax.tech/mcp"
        }
      }
    }
    ```
  </Tab>

  <Tab title="Windsurf">
    **Add to `~/.codeium/windsurf/mcp_config.json`:**

    ```json
    {
      "mcpServers": {
        "dgtx-ke": {
          "url": "https://ke.docs.digitax.tech/mcp"
        }
      }
    }
    ```
  </Tab>

  <Tab title="Claude Desktop">
    Claude Desktop connects to remote MCP servers through the Connectors UI, not via `claude_desktop_config.json`.

    1. Open **Claude Desktop** and go to **Settings → Connectors**.
    2. Click **Add custom connector**.
    3. Enter a name (e.g. `DigiTax Kenya`) and the URL:
       ```
       https://ke.docs.digitax.tech/mcp
       ```
    4. Save. To use it in a conversation, click **+** → **Add connectors** and enable **DigiTax Kenya**.

  </Tab>
</Tabs>

## Testing Your MCP Setup

Once configured, you can test your MCP server connection:

1. **Open your AI editor** (Cursor, Windsurf, Claude Desktop, etc.)
2. **Start a new chat** with the AI assistant
3. **Ask about DigiTax Kenya API Hub** - try questions like:
   * "How do I create an eTIMS sale with DigiTax Kenya?"
   * "Which fields are mandatory when creating an item, and how do I pick its item classification code?"
   * "How do I issue a credit note against an existing sale?"
   * "How do I get a callback when a sale has synced with eTIMS?"

The AI should now have access to your DigiTax Kenya API Hub account data and documentation through the MCP server.

## Authentication

The DigiTax Kenya MCP server reads live data from your account. Pass your API key as a request header:

```text
X-API-Key: <your-api-key>
```

See [Prerequisites of using the API](doc:start-using-the-api#prerequisites) for how to obtain your key and configure it in your MCP client.
