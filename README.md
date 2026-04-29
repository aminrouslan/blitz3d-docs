# Blitz3D Docs in Markdown for LLM reference

## Links
Click [here](https://github.com/aminrouslan/blitz3d-docs) to visit the repository.
Or run `git clone https://github.com/aminrouslan/blitz3d-docs.git` in your terminal to clone the repository.

## What is this?
This is a conversion of the Blitz3D documentation from HTML to Markdown.
The project includes all 2D and 3D commands, the ASCII chart, and scancodes.

## Why was this made?

### Reason 1
This was made for use with Large Language Models (LLMs) such as ChatGPT or Claude to help you write real Blitz3D code.
A majority of LLMs know little to nothing about Blitz3D code, so they produce hallucinated (fake) code.

### Reason 2
The content of the original documentation is littered with HTML tags which unnecessarily increases the token count for LLMs.
That is why I converted the entire documentation from HTML to Markdown to reduce it.

## Optional FastMCP Server Script (Python)

1. Install the FastMCP package for Python by running `pip install fastmcp` in your terminal.

2. Copy the following Python script into Notepad and save as `server.py` in the same directory as the cloned repository:

```python
from fastmcp import FastMCP

mcp = FastMCP('Blitz3D Docs')

@mcp.tool()
def list_2d_commands() -> str:
    """Lists all 2D commands."""
    with open('command_list_2d.md') as file:
        return file.read()

@mcp.tool()
def list_3d_commands() -> str:
    """Lists all 3D commands."""
    with open('command_list_3d.md') as file:
        return file.read()

@mcp.tool()
def get_2d_command(command: str) -> str:
    """Returns the documentation for the specified 2D command."""
    try:
        with open(f'2d_commands/{command}.md') as file:
            return file.read()
    except FileNotFoundError:
        return 'Documentation not found.'

@mcp.tool()
def get_3d_command(command: str) -> str:
    """Returns the documentation for the specified 3D command."""
    try:
        with open(f'3d_commands/{command}.md') as file:
            return file.read()
    except FileNotFoundError:
        return 'Documentation not found.'

@mcp.tool()
def get_ascii_chart() -> str:
    """Returns an ASCII Chart for reference."""
    with open('ascii.md') as file:
        return file.read()
    
@mcp.tool()
def get_scancodes() -> str:
    """Returns scancodes for reference."""
    with open('scancodes.md') as file:
        return file.read()

if __name__ == '__main__':
    mcp.run()
```

3. Run with `fastmcp run server.py --transport http --host 0.0.0.0 --port 8000` in your terminal.

4. Done!
