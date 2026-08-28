# my-mcp-server

A small MCP server exposing my notes to Claude Desktop

## Features

- FastMCP style: decorators, zero boilerplate
- Three tools: add / get / list notes
- State persisted to a JSON file in the home dir
- Includes Claude Desktop config snippet

## Usage

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## Getting started

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   └── pull_request_template.md
├── docs/
│   ├── configuration.md
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── SECURITY.md
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT. Do whatever you want.
