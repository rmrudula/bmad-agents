# BMAD Framework Setup

## Overview

This repository contains the BMAD framework setup configured with GitHub Copilot for agent-driven development workflows.

## Prerequisites

- Node.js
- npm / npx
- Git
- Visual Studio Code
- GitHub Copilot
- uv

## Dependency Purpose

### Node.js and npm

BMAD installation relies on the Node.js ecosystem.

Node.js provides the runtime required for the installation tooling, while npm/npx is used for package resolution and execution of the BMAD installer.

Verify the environment using:

```bash
node --version
npm --version

npx bmad-method install

uv
uv is used by BMAD build and automation workflows for Python-based tooling.

Verify the installation using:
uv --version

Repository Structure

bmad-agents/
├── .agents/skills/       # BMAD skills
├── .github/agents/       # GitHub Copilot agent definitions
├── _bmad/                # BMAD core modules and configuration
└── _bmad-output/         # Generated artifacts

GitHub Copilot Integration
BMAD generates Copilot-compatible agent definitions and skills under:

.github/agents
.agents/skills

These resources allow GitHub Copilot to discover and execute BMAD workflows within the repository context.

BMAD workflow guidance can be accessed through Copilot Chat using:

/bmad-help
