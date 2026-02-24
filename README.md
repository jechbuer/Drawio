# Draw.io Diagrams

This repository contains draw.io diagrams created with AI assistance.

## Using draw.io Without Claude Code

### Option 1: Claude.ai Projects (Easiest - No Install/MCP)

For users without Claude Code, the easiest method is **Claude.ai Projects**:

1. Go to https://claude.ai
2. Create a new Project
3. Add this system prompt to the Project instructions:

```
When the user asks for a diagram, generate a draw.io URL using Python code execution.
Create the mxGraphModel XML, encode it, and provide a clickable draw.io link.
The link will open directly in draw.io web app with the full diagram embedded.
```

4. Then simply prompt:  
   **"Describe & generate draw.io diagram for [your idea here]"**

Claude will output a clickable, editable link that opens in draw.io web app with the full XML embedded.

### Option 2: Hosted Inline (MCP Apps)

If your Claude.ai supports MCP Apps:

1. Add `https://mcp.draw.io/mcp` as a remote MCP server
2. Then prompt normally for diagrams
3. Diagrams will render inline in the chat

### Option 3: draw.io Desktop + Claude Code

For local development with full export capabilities:

1. Install [draw.io Desktop](https://github.com/jgraph/drawio-desktop/releases)
2. Use Claude Code with the draw.io skill
3. Export to PNG/SVG/PDF with embedded XML

## Files in this Repo

| File | Description |
|------|-------------|
| `user-login-erp-bc-sync.drawio` | User login flow with ERP Business Central sync (with branches) |
| `user-login-erp-sync.drawio` | Linear version of the login flow |

## Opening Diagrams

1. Go to https://app.diagrams.net
2. File → Open From → Device
3. Select the `.drawio` file
4. Edit and save

## Resources

- [draw.io](https://www.draw.io) - Free online diagram editor
- [draw.io Desktop](https://github.com/jgraph/drawio-desktop) - Desktop application
- [drawio-mcp on GitHub](https://github.com/jgraph/drawio-mcp) - Official MCP integration
