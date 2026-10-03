# Project plan: MCP Config Doctor

## Brief

**Type:** Local-first developer tool

**Audience:** Developers configuring local AI agents.

**Problem:** Inspect MCP server configuration for risky commands, exposed credentials and permissive launch flags before you run it.

## Experience flow

1. Read the scope and privacy boundary before entering data.
2. Load the fictional sample or paste authorized input.
3. Run the local analysis and inspect each rule or calculation.
4. Copy or download a draft only when the user chooses.

## Core capabilities

- Parse common mcpServers JSON layouts
- Flag shell launchers, mutable packages and permissive flags
- Check environment key names without echoing values
- Export a concise, reviewable audit

## Key design decision

Keep the application self-contained and explain what is heuristic, human-reviewed or user-configured. Never imply that a demo replaces a production control.

## Boundaries

This is a static configuration review, not a sandbox or a guarantee of safety. It does not launch servers, contact MCP endpoints or send configuration anywhere.

## Learning goals

- Keep input handling, analysis and rendering in clear small functions.
- Make empty, invalid and successful states visible and accessible.
- Use semantic HTML, labelled fields, keyboard focus and responsive CSS.
- Document assumptions, local data handling and limitations.

## Next iteration

Add user research and domain-specific validation rules, then document those rules with examples before expanding scope.
