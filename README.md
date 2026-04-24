# The Token Maxer 5000 🔥

You've got a quota to hit and I'm here to help. This project will make every engineer in your company envious of your token usage.  Tokenshame as they say.

## Purpose
Hit emerald on your internal token usage leaderboards.

## How To Use It
It's a markdown file, if you don't know how to use this you might be cooked.

1. Drop CLAUDE.md in your project root:
bashcp CLAUDE.md /your/project/root/CLAUDE.md
Claude Code loads CLAUDE.md automatically at session start — no extra configuration needed.
2. Set effort level to high:
Create .claude/settings.json in your project:
json{
  "effortLevel": "high"
}
Or export it before starting a session:
bashexport CLAUDE_CODE_EFFORT_LEVEL=high
claude
3. Fill in the Project Context section at the bottom of CLAUDE.md:
markdown## Project Context

## Why This Exists
Why not.

## Token Usage Note
This spec intentionally increases token consumption. That's the point. Extended thinking (enabled by effortLevel: high) can run into tens of thousands of output tokens per request. The CLAUDE.md file itself is loaded into context at session start and costs tokens on every turn.
If you want to dial it back for a specific session, you can override effort level:
bashexport CLAUDE_CODE_EFFORT_LEVEL=medium
Or adjust the directives in CLAUDE.md — they're plain English, easy to tune.

License
MIT — use it, fork it, max your tokens.
