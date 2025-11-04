# MCP: Build Rich-Context AI Apps with Anthropic

This repo covers how to use the **Model Context Protocol (MCP)** to build applications that connect LLMs to external tools, data sources, and prompt-resources in a standardized way.

---

## What You’ll Learn

- The purpose and architecture of the Model Context Protocol (MCP), how it enables AI apps to integrate with external tools/data without bespoke integrations.
- How to build an MCP-compatible server exposing tools, prompt templates, and resources (e.g., local files, web scraping, data repositories).
- How to build an MCP client inside an AI application (chatbot or agent) that connects to MCP servers and uses their capabilities.
- How to deploy and configure MCP servers and clients, including connecting to reference servers (e.g., filesystem, fetch) and integrating with applications like Claude Desktop.
- Best practices for building rich-context AI applications that scale and avoid fragmented tool integrations.

---

## Setup Instructions

1. **Clone the repository**
2. **Install dependencies**

   ```bash
   pip install fastmcp mcp-sdk python-dotnet (or other SDKs as needed)
   ```

   _(Ensure you check the `requirements.txt` or code comments for precise packages.)_

3. **Run the examples**

   - Open notebooks and run sequentially.
   - To experiment with the server/client patterns:

     ```bash
     python create_mcp_server.py
     python create_mcp_client.py
     ```

   - Explore connecting to reference servers or external tools via the MCP protocol.

---

## How to Get Started

- Start with the **“Introduction to MCP”** notebook which covers the background and architecture of MCP.
- Then move to the **“Server Setup”** notebook/script to build your own MCP server exposing tools/resources.
- Next, open the **“Client Setup”** notebook/script to connect an AI application to your server.
- Finally, use the **“Deployment & Integration”** examples to connect multiple servers, configure clients like Claude Desktop, and deploy your system remotely.
- You’re encouraged to **customize**: add new tools, data sources, or connect to other MCP-compatible servers.

---

## Why This Matters

As AI systems become more ubiquitous, the ability to seamlessly integrate models with tools and data sources is critical. MCP provides a **standard protocol** for doing so — reducing integration complexity, promoting reuse, and enabling richer AI applications. This course and repo give you the practical skills to build next-generation AI systems that truly connect with the world.

---
