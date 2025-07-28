# 🔌 Integrate XPack MCP Services into Your AI Product

XPack is an open MCP (Model-Context Protocol) marketplace that allows your AI product to connect with real-world tools and data via a simple config. This guide walks you through how to connect your AI application to XPack’s online MCP services in just a few minutes.

## ✨ Step-by-Step Integration Guide

### 1. Add XPack MCP Config to Your AI Product

In your product’s MCP config, add a new MCP service entry pointing to the XPack server:

```json
{
  "mcpServers": {
    "xpack-mcp-market": {
      "type": "sse",
      "url": "https://mcp.xpack.ai/v1/mcp?apikey={Your-XPack-API-Key}"
    }
  }
}
```

Replace `{Your-XPack-API-Key}` with your actual API key obtained from XPack.

---

### 2. Get Your XPack API Key

- Visit [https://xpack.ai](https://xpack.ai)  
- Register or log in  
- An API key will be automatically generated for your account  

You can find it on the dashboard. Copy the API key and paste it into your config.

---

### 3. Invoke XPack MCP Tools via Dialogue

Once the integration is complete, your AI agent can start calling tools from the XPack MCP marketplace using natural language.

For example, you can prompt your agent with:

> "Use the XPack MCP service to check the weather in New York and generate a 3D-style illustration based on it"

XPack will automatically handle the tool selection and execute the workflow using available MCPs.

---

## ✅ That’s it!

You’ve successfully connected your AI product to the world of real-time, real-world services via XPack’s MCP marketplace. Enjoy building!
