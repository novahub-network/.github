## Welcome to the Nova Ecosystem!

We are an open-source community building the **open-source operating system for a circular economy.**

Our mission is to engineer the interconnected pillars—from finance and AI to materials and agriculture—needed to transition our planet to a sustainable, circular model. The Nova Ecosystem is stewarded by the (future) non-profit **Nova Foundation gGmbH** and commercially supported by **[Circular Engineering Nova GmbH](https://circular.engineering/)**.

* 🌐 **Ecosystem Hub:** [**nova-ecosystem.org**](https://nova-ecosystem.org) (The main "user manual")
* 🚀 **Central App:** [**app.nova-ecosystem.org**](https://app.nova-ecosystem.org) (Your "Mission Control" dashboard)
* 📚 **Documentation:** [**nova-ecosystem.org/docs**](https://nova-ecosystem.org/docs) (Architecture, Guides, & API Docs)
* 💬 **Email Us:** [**contact@nova-ecosystem.org**](mailto:contact@nova-ecosystem.org)

---

### 🏗️ Our Architecture

Our architecture is a "monorepo" model designed for atomic, coordinated development. Instead of many small repos for each app/api/website, each pillar's core components are grouped into a single repository.

#### 1. The Core Monorepo: `ecosystem-core`
This is the "heart" of the ecosystem. It's a monorepo containing all the tightly-coupled central services:
* `/api`: The central API Gateway.
* `/app`: The "Mission Control" dashboard.
* `/auth`: The unified "passport" (SSO/Identity) service.
* `/website`: The Docusaurus site for `nova-ecosystem.org` and all high-level docs.

#### 2. Pillar Monorepos (e.g., `hub`, `finance`, `agro`)
One monorepo for each pillar's core product. This allows a single, atomic pull request to update the API, App, and Website for a new feature.
* **Example (`hub` repo):**
    * `/api`: Code for the `hub-api` artifact.
    * `/app`: Code for the `hub-app` artifact.
    * `/website`: Code for the `hub-website` artifact.
    * `/tests`: **Intra-pillar tests** (testing `/api` and `/app` *together*).

#### 3. Decoupled Worker Repos (e.g., `hub-worker-sync`)
These are specialized, single-purpose backend services (like data importers or background jobs) that are developed and deployed independently from the core pillars for better scalability and fault isolation.

#### 4. Central Governance Repos
* **`ecosystem-qa`:** This repo tests the "seams" *between* repositories (e.g., tests `hub` <-> `finance`, or `hub` <-> `hub-worker-sync`).
* **`ecosystem-releases`:** Hosts the CalVer-tagged `release-manifest.json` files that define each stable ecosystem release.

#### 5. Product Repos (e.g., `durasagv`)
Standalone "flagship" product monorepos that *consume* services from multiple pillars (e.g., `ai` and `agro`).

---

### 🚀 How to Get Involved

We welcome contributors of all kinds—from code and documentation to design and policy standards. The best place to start is our main [Contribution Guide](../CONTRIBUTING.md).

#### Finding Your Way
Our new monorepo structure makes it easy to find what you're looking for:

1.  **Start at the Core:** The **`ecosystem-core`** repo is the best place to understand the central platform.
2.  **Browse the Pillars:** Pick a **Pillar Monorepo** (e.g., **`hub`**, **`agro`**, **`balance`**) that matches your interests. You can find the API, App, and Website all in one place.
3.  **Explore Products:** Check out our product repos (like **`durasagv`**) to see how the ecosystem comes together.
4.  **Find Backend Tasks:** Browse the **`worker-`** repositories for decoupled, single-purpose microservice tasks.

---
We are committed to fostering an open and welcoming environment. Please read our [Code of Conduct](../CODE_OF_CONDUCT.md) before participating.
