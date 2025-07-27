# 🚀 Project Horizon (Public Scaffold)

![CI](https://github.com/ipow-jms/project-horizon-public/actions/workflows/dev-checks.yml/badge.svg)

**A modular AI-native framework for exploring emerging private markets.**

Project Horizon is an experimental platform designed to support open research and development around intelligent systems, applied embeddings, and AI-native UI workflows. This public repo provides scaffolding and utilities to support extensions, integrations, and experimentation—while protecting the proprietary core logic and product vision.

---

## 🧠 What's Included

* 🔧 Developer scaffolding for modular backend services (MCP servers)
* 🧱 Example WeWeb automation hooks and Nhost-compatible functions
* ⚙️ Utility scripts for embedding pipelines and metadata reset
* 📐 Hasura metadata, RLS examples, and role-aware GraphQL setup
* 📁 Experiments and testbed notebooks for embedding workflows
* 🛠 CI workflows, issue templates, and onboarding support

---

## 🔐 What's Not Included

The proprietary core of Project Horizon is maintained in a private companion repo. It includes:

* Agentic workflows and prompt logic
* Engagement tracking and progression systems
* Proprietary datasets and embeddings
* Application-specific logic powering adaptive UX and signal modeling

See [`PROPRIETARY.md`](./PROPRIETARY.md) for more details.

---

## 🧩 Repo Structure

```
📁 .github/                  # Issue templates, workflows
📁 backend/mcp_public/       # Safe-to-share MCP server scaffolds
📁 docs/                    # Safe-to-share Architecture documents
📁 frontend/weweb-scripts/   # WeWeb embed scripts (non-proprietary)
📁 graphql/                  # Hasura metadata and RLS scaffolding
📁 notebooks/experiments/    # Experiment notebooks, non-sensitive
📁 scripts/                  # Embedding and utility scripts
```

---

## 📚 Project Docs

- [Architecture Overview](./docs/architecture.md)
- [Roadmap](./ROADMAP.md)
- [Security Policy](./SECURITY.md)
- [Contributing Guide](./CONTRIBUTING.md)
- [License Attribution](./LICENSES.md)

---

## 🛠 Getting Started

```bash
git clone https://github.com/YOUR_USERNAME/project-horizon-public.git
cd project-horizon-public
cp .env.example .env
```

You’ll need:

* Python 3.10+
* Optional: virtualenv or pyenv for isolation

Install dependencies (if using scripts):

```bash
pip install -r requirements.txt
```

You can explore safe-to-extend modules in:

- `backend/mcp_public/`
- `scripts/`
- `notebooks/experiments/`

Additional architectural context is available in [`architecture.md`](./architecture.md).

---

## 📜 License

This public repo is licensed under the MIT License. See `LICENSE` for details.
Attribution is required. Commercial use is allowed.

---

📬 Questions or interested in collaborating?

Reach us at: [projecthorizon.stealth@gmail.com](mailto:projecthorizon.stealth@gmail.com)
