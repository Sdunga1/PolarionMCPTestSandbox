# Polarion MCP Test Sandbox

This repository provides a preconfigured development environment for testing Polarion MCP tools with GitHub Copilot. Everything is set up so you can start using the tools right away.

## What's Included

- GitHub Copilot and Copilot Chat extensions preinstalled
- MCP server configuration ready to connect to your Polarion instance
- Development container setup for consistent environment

## Getting Started

### 1. Open in Codespaces

Click the "Code" button on this repository and select "Open with Codespaces" to create a new Codespace. The environment will build automatically with all extensions installed.

### 2. Configure Your Polarion Server URL

Create a `.env` file in the workspace root with your Polarion MCP server URL:

```
MCP_SERVER_URL=http://your-polarion-server.com:8080/sse
```

You can use `.env.example` as a template. The `.env` file is gitignored, so your server URL won't be committed to the repository.

### 3. Reload the Window

After creating your `.env` file, reload the VS Code window:

- Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
- Type "Developer: Reload Window" and press Enter

### 4. Start Using Copilot

Once the window reloads, the MCP server should connect automatically. You can now use GitHub Copilot Chat to interact with your Polarion tools. The tools will be available in the chat interface.

## Troubleshooting

If the MCP server doesn't connect:

1. Check that your `.env` file exists and contains `MCP_SERVER_URL` with a valid URL
2. Verify the server is accessible from the Codespace (test with `curl` if needed)
3. Check the MCP Servers output panel for any error messages
4. Try restarting the MCP servers from the Command Palette: "MCP Servers: Restart all"

## Configuration Files

- `.vscode/mcp.json` - MCP server configuration (reads from environment variable)
- `.vscode/settings.json` - VS Code workspace settings
- `.devcontainer/devcontainer.json` - Development container setup
- `.env.example` - Template for your environment variables

## Notes

This sandbox is designed for testing and demonstration purposes. Make sure your Polarion server is accessible from the Codespace network, and that you have the necessary permissions to connect to it.
