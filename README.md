# code-map-mcp
Python MCP

Key Features:

Scans your workspace for Python, JavaScript, and TypeScript files
Extracts all functions, classes, and methods with their locations
Provides powerful search to find functions by name or parameters
Tracks file paths and line numbers for easy navigation
5 Tools Available:

scan_workspace - Build/update the code map from your workspace
search_functions - Find functions by name or parameters
get_file_map - View all code elements in a specific file
list_all_functions - Browse all tracked functions/classes
track_file - Manually add a new file to the map
To use it:

Install with pip install -e code-map-mcp or use uvx
Add to your MCP config at 

mcp.json
:
{
  "mcpServers": {
    "code-map": {
      "command": "python",
      "args": ["/absolute/path/to/code-map-mcp/server.py"],
      "disabled": false,
      "autoApprove": ["scan_workspace", "search_functions"]
    }
  }
}

The server will help you quickly locate any function you need as you generate code through specs or vibecoding. Just scan your workspace periodically to keep the map updated!
