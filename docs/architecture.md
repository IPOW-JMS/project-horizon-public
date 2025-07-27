🧱 Project Horizon – Architecture Overview (Public Version)

This document outlines the high-level technical architecture of Project Horizon’s public-facing scaffolding. It is designed to support contributor onboarding, open R&D, and future expansion of AI-native workflows.

⸻

⚙️ Stack Overview

Layer	Tech	Purpose
Frontend	WeWeb	No-code UI builder with JS/native action support
Backend	Nhost	Postgres DB, auth, file storage, edge functions
GraphQL	Hasura	Role-aware API over Nhost DB with permissions
Agents	Python (modular)	Scaffolded agent endpoints with MCP wrapper pattern
CI/CD	GitHub Actions	Linting and test automation


⸻

🧩 Modular Components

backend/mcp_public/
	•	Stateless FastAPI services intended to wrap logic into composable, callable agent endpoints
	•	Examples: /ping, /simulate_embedding, /extract_metadata

frontend/weweb-scripts/
	•	Utility JS scripts for custom component behavior
	•	Integration hooks for anonymous onboarding, event triggers, etc.

graphql/
	•	Hasura metadata and RLS configuration
	•	Defines GraphQL schema and access roles for public, anonymous, etc.

scripts/
	•	CLI tools for embedding, metadata reset, or testing
	•	No business logic or proprietary algorithms

notebooks/experiments/
	•	Exploration notebooks (e.g., embedding chunking strategies, pipeline timing)
	•	Meant to be standalone and forkable

⸻

🔐 Private Interfaces (Omitted Here)

The following elements are excluded from this public architecture:
	•	Prompt design and agent chaining
	•	Tier progression, engagement telemetry, or RAG scores
	•	Proprietary embedding logic and scoring heuristics
	•	Signal ingestion, ranking, or market data logic

Refer to PROPRIETARY.md for boundary details.

⸻

🧠 Contribution Path
	•	Add new agents in mcp_public/ with FastAPI or Flask wrappers
	•	Use scripts/ to test transformations or embedding loads
	•	Use GitHub Actions to validate formatting and tests
	•	Fork notebooks or generate public-safe utilities

Have questions? Email: projecthorizon.stealth@gmail.com