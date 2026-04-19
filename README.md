To install the add_tool MCP server, run the following command:

{
  "mcpServers": {
    "chess-stat-server": {      
      "command": "uvx",
      "args": [
        "--from",
        "git+https://github.com/eradesa/mcp-chess-stats.git",
        "chess"
      ]
    }
  }
}

- name: "git_chess_stat"
      command: "uvx"
      args: ["--from", "git+https://github.com/eradesa/mcp-chess-stats.git", "chess"]
      #env:
      #  FILE_IO_BASE_DIR: "/home/erangadesaram/Downloads"  # optional
      transport: "stdio"
This will fetch and set up the mcp-server from the specified GitHub repository.