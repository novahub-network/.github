## Welcome to the Nova Ecosystem\!

We are an open-source community building the **open-source operating system for a circular economy.**

Our mission is to engineer the interconnected **Horizontal Enablers** (like finance and AI) and **Vertical Sectors** (like materials and agriculture) needed to transition our planet to a sustainable, circular model. The Nova Ecosystem is stewarded by the (future) non-profit **Nova Foundation gGmbH** and commercially supported by **[Circular Engineering Nova GmbH](https://circular.engineering/)**.

  * 🌐 **Ecosystem Hub:** [**nova-ecosystem.org**](https://nova-ecosystem.org) (The main "user manual")
  * 🚀 **Central App:** [**app.nova-ecosystem.org**](https://app.nova-ecosystem.org) (Your "Mission Control" dashboard)
  * 📚 **Documentation:** [**nova-ecosystem.org/docs**](https://nova-ecosystem.org/docs) (Architecture, Guides, & API Docs)
  * 💬 **Email Us:** [**contact@nova-ecosystem.org**](mailto:contact@nova-ecosystem.org)

-----

### 🏗️ Our Architecture

Our architecture is a "monorepo" model designed for atomic, coordinated development. Instead of many small repos for each app/api/website, each **Horizontal Enabler's** or **Vertical Sector's** core components are grouped into a single repository.

#### 1\. The Core Monorepo: `ecosystem-core`

This is the "heart" of the ecosystem. It's a monorepo containing all the tightly-coupled central services:

  * `/api`: The central API Gateway.
  * `/app`: The "Mission Control" dashboard.
  * `/auth`: The unified "passport" (SSO/Identity) service.
  * `/website`: The Docusaurus site for `nova-ecosystem.org` and all high-level docs.

#### 2\. Horizontal Enabler Monorepos (e.g., `hub`, `finance`, `ai`)

One monorepo for each cross-cutting, foundational service. This allows a single, atomic pull request to update the API, App, and Website for a new feature.

  * **Example (`hub` repo):**
        \* `/api`: Code for the `hub-api` artifact.
        \* `/app`: Code for the `hub-app` artifact.
        \* `/website`: Code for the `hub-website` artifact.
        \* `/tests`: **Intra-Enabler tests** (testing `/api` and `/app` *together*).

#### 3\. Vertical Sector Monorepos (e.g., `agro`, `water`, `build`)

One monorepo for each industry-specific application. These **Sectors** *consume* the services from the **Enablers**.

  * **Example (`agro` repo):**
        \* `/api`: Code for the `agro-api` artifact.
        \* `/app`: Code for the `agro-app` artifact.
        \* `/website`: Code for the `agro-website` artifact.
        \* `/tests`: **Intra-Sector tests** (testing `/api` and `/app` *together*).

#### 4\. Decoupled Worker Repos (e.g., `hub-worker-sync`)

These are specialized, single-purpose backend services (like data importers or background jobs) that are developed and deployed independently from the core **Enablers** and **Sectors** for better scalability and fault isolation.

#### 5\. Central Governance Repos

  * **`ecosystem-qa`:** This repo tests the "seams" *between* repositories (e.g., tests `hub` \<-\> `finance` (Enabler-to-Enabler), or `hub` \<-\> `agro` (Enabler-to-Sector)).
  * **`ecosystem-releases`:** Hosts the CalVer-tagged `release-manifest.json` files that define each stable ecosystem release.

#### 6\. Product Repos (e.g., `durasagv`)

Standalone "flagship" product monorepos that *consume* services from multiple **Enablers** (e.g., `ai`) and **Sectors** (e.g., `agro`).

-----

### 🚀 How to Get Involved

We welcome contributors of all kinds—from code and documentation to design and policy standards. The best place to start is our main [Contribution Guide](https://www.google.com/search?q=../CONTRIBUTING.md).

#### Finding Your Way

Our new monorepo structure makes it easy to find what you're looking for:

1.  **Start at the Core:** The **`ecosystem-core`** repo is the best place to understand the central platform.
2.  **Browse the Enablers & Sectors:** Pick a **Horizontal Enabler** (e.g., **`hub`**, **`balance`**) or a **Vertical Sector** (e.g., **`agro`**) that matches your interests. You can find the API, App, and Website all in one place.
3.  **Explore Products:** Check out our product repos (like **`durasagv`**) to see how the ecosystem comes together.
4.  **Find Backend Tasks:** Browse the **`worker-`** repositories for decoupled, single-purpose microservice tasks.

-----

We are committed to fostering an open and welcoming environment. Please read our [Code of Conduct](https://www.google.com/search?q=../CODE_OF_CONDUCT.md) before participating.