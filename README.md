# Polarion MCP Test Sandbox

This repository provides a preconfigured development environment for testing Polarion MCP tools with GitHub Copilot. Everything is set up so you can start using the tools right away.

## What's Included

- GitHub Copilot and Copilot Chat extensions preinstalled
- MCP server configuration ready to connect to your Polarion instance
- Development container setup for consistent environment

## Getting Started

### 1. Open in Codespaces

Click the "Code" button on this repository and select "Open with Codespaces" to create a new Codespace. The environment will build automatically with all extensions installed.

### 2. Start the MCP Server

Open the `.vscode` folder in the file explorer, then open `mcp.json`. You'll see a "Start" button or option to start the MCP server. Click it to connect to the Polarion server.

### 3. Start Using Copilot

Once the MCP server is running, you can use GitHub Copilot Chat to interact with your Polarion tools. The tools will be available in the chat interface.

## Troubleshooting

If the MCP server doesn't connect:

1. Make sure you've clicked "Start" in the `mcp.json` file
2. Verify the server is accessible from the Codespace (test with `curl` if needed)
3. Check the MCP Servers output panel for any error messages
4. Try restarting the MCP servers from the Command Palette: "MCP Servers: Restart all"

## Configuration Files

- `.vscode/mcp.json` - MCP server configuration (open this file and click Start)
- `.vscode/settings.json` - VS Code workspace settings
- `.devcontainer/devcontainer.json` - Development container setup

## Notes

This sandbox is designed for testing and demonstration purposes. Make sure your Polarion server is accessible from the Codespace network, and that you have the necessary permissions to connect to it.
