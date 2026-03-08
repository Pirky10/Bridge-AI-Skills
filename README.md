# Bridge AI Skills

This repository contains the AI prompt skills and reference documentation for the [Bridge AI](https://github.com/Pirky10/Bridge) project, which connects AI assistants (like Claude, Cursor, and Windsurf) to the Unity Editor via the Model Context Protocol (MCP).

## Contents

The repository is structured to seamlessly sync with the Bridge AI Unity package. When using the Skill Sync feature in Unity, it pulls from this repository to ensure your AI always has the latest tools, schemas, and best practices.

* **.claude/**: Contains the core prompt instructions and settings tailored for Claude and other MCP clients.
* **unity-mcp-skill/**: Contains the main `SKILL.md` orchestrator guide.
  * **references/**: Detailed documentation for the AI to understand the Unity environment:
    * `tools-reference.md`: Complete schema and usage guide for all available tools.
    * `resources-reference.md`: Guide to all available Unity resources.
    * `workflows.md`: Common patterns and examples for accomplishing tasks in Unity.
    * `probuilder-guide.md`: Advanced guide for 3D modeling using the ProBuilder integration.

## How to used

This repository is primarily meant to be read by AI assistants. The Bridge AI Unity package will automatically download and sync these files to your local `.claude/skills/unity-mcp-skill` directory when you use the **Unity MCP Skill Install(Sync)** window in the Unity Editor.

If you are setting up manually or modifying instructions for your own project:
1. Ensure your MCP client is configured to load the Bridge AI server.
2. The AI will automatically read the `.claude/skills/unity-mcp-skill/SKILL.md` file to understand its capabilities.
