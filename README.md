[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/MY-GITHUB-USERNAME/MY-REPO-NAME)

<!-- Edit the badge URL above: replace MY-GITHUB-USERNAME/MY-REPO-NAME with the actual owner/repo. -->

# Deep Agents 101

Instructor's demo notebook walks through building a journal agent with the `deepagents` harness.

## What's in this repo

- `deep_agents_101_journal_agent.ipynb`: the instructor's demo notebook. Builds one journal agent, one step at a time.
- `deep_agents_101_template.ipynb`: a blank version of the same steps, with no persona or use case baked in. Use it as a starting point for your own agent.
- `images/`: screenshots and diagrams referenced in the notebooks.
- `pyproject.toml`, `uv.lock`: dependency manifest for `uv`.

## Getting Started

Click **Open in GitHub Codespaces** above and wait for the Codespace to build. Dependencies install automatically via [uv](https://docs.astral.sh/uv/); open `deep_agents_101_journal_agent.ipynb` and start running cells.

The devcontainer uses Python 3.12, runs `uv sync` on first launch, and configures VS Code to use the `.venv` interpreter.

## Workshop outline

0. **Setup**: connect a model.
1. **Invoke the agent**: call `create_deep_agent` and send it a message.
2. **System prompt**: give the agent a persona with `system_prompt`.
3. **Custom tool**: write a `@tool` function and hand it to the agent.
4. **Optional, human-in-the-loop**: gate a tool call with `interrupt_on` so a human can approve, edit, or reject it before it runs.

Not covered today, but in the full LangChain Academy Deep Agents course: subagent delegation, backends (filesystem/store/composite), skills, memory across sessions, sandboxes, and deployment.
