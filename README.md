# MCP Server Deployment

This repository contains configuration for MCP (Model Context Protocol) servers.

## Configuration

The following JSON snippet configures the `addtool` MCP server:

```json
{
    "mcpServers": {
        "addtool": {
            "command": "uvx",
            "args": [
                "--from",
                "git+https://github.com/vischva/mcpserverexample.git",
                "mcp-server"
            ]
        }
    }
}
```

- **Command**: `uvx`
- **Source**: Git repository at `https://github.com/vischva/mcpserverexample.git`
- **Entry Point**: `mcp-server`

## Usage

The configuration can be used with MCP-compatible applications that support server definitions in this JSON format.
