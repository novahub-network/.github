## Welcome to the Nova Ecosystem!

We are an open-source community building the **open-source operating system for a circular economy.**

Our mission is to engineer the interconnected pillars—from finance and AI to materials and agriculture—needed to transition our planet to a sustainable, circular model. The Nova Ecosystem is stewarded by [Circular Engineering Nova GmbH](https://circular.engineering/).

* 🌐 **Ecosystem Hub:** [**nova-ecosystem.org**](https://nova-ecosystem.org) (The main "user manual" for the ecosystem)
* 🚀 **Central App:** [**app.nova-ecosystem.org**](https://app.nova-ecosystem.org) (Your "Mission Control" dashboard)
* 📚 **Documentation:** [**nova-ecosystem.org/docs**](https://nova-ecosystem.org/docs) (Architecture & Guides)
* 💬 **Email Us:** [**contact@nova-ecosystem.org**](mailto:contact@nova-ecosystem.org)

---

### 🏗️ Our Architecture

Our ecosystem is a **"Hub-and-Spoke"** model. The repositories in this organization are grouped into four main categories, all identifiable by their prefixes.

#### 1. Core Ecosystem Services (Prefix: `ecosystem-`)
This is the "Hub" or "meta-pillar" that runs the entire system. It provides the central services that all other pillars consume.

* **`ecosystem-website`:** The main informational "user manual" and documentation.
* **`ecosystem-auth`:** The unified "passport" (SSO, KYC, auth) for all users.
* **`ecosystem-app`:** The central "Mission Control" dashboard for profile management.
* **`ecosystem-api`:** The central API Gateway (the "front door" for all services).
* **`ecosystem-qa`:** Cross-pillar testing, QA, and E2E test suites.
* **`ecosystem-operations`:** Central DevOps, IaC, and deployment pipelines.

#### 2. Enabler Pillars (Prefix: `pillar-*` topic)
The horizontal "OS" providing the core infrastructure and capabilities for the economy.

* **`hub-` (Novahub):** The collaboration engine for projects and partners.
* **`finance-` (Novafinance):** The capital engine for green loans, bonds, and ESG finance.
* **`markets-` (Novatrade):** The trading backbone for circular commodities.
* **`ai-` (Novasapien):** The intelligence layer (AI, IoT, digital twins).
* **`energy-` (Novaelectron):** The power grid for renewable energy and smart grids.
* **`material-` (Novamaterial):** The R&D lab for sustainable materials and recycling tech.
* **`mobility-` (Novamobility):** The logistics network for EV fleets and reverse logistics.
* **`infra-` (Novainfra):** The physical backbone for circular industrial parks.
* **`skills-` (Novaskills):** The human capital engine for training and "circular job" certifications.
* **`balance-` (Novabalance):** The environmental auditor (the "E" in ESG).
* **`equity-` (Novaequity):** The social auditor (the "S" in ESG).
* **`policy-` (Novapolicy):** The "rulebook" setting standards for governance and compliance (the "G" in ESG).

#### 3. Sector Pillars (Prefix: `sector-*` topic)
The vertical "applications" where the enablers are applied to specific industries.

* **`agro-` (Novaagro):** Regenerative agriculture and food systems.
* **`water-` (Novawater):** Water purification, recycling, and smart irrigation.
* **`build-` (Novabuild):** Circular construction and smart buildings.
* **`textile-` (Novatextile):** Fiber-to-fiber recycling and circular fashion.
* **`waste-` (Novawaste):** Resource recovery, e-waste mining, and waste-to-value.
* **`air-` (Novaair):** Air quality monitoring, pollution control, and carbon capture.
* **`health-` (Novahealth):** Circular healthcare and preventative wellness.

#### 4. Products (Prefix: `product-*` topic)
These are standalone "flagship" products that *consume* services from multiple pillars and sectors.

* **Example: `durasagv-`** (An autonomous agricultural vehicle that uses the `ai-` pillar and the `agro-` sector).

---

### 🚀 How to Get Involved

We welcome contributors of all kinds—from code and documentation to design and policy standards. The best place to start is our main [Contribution Guide](../CONTRIBUTING.md).

#### Finding Your Way
With over 40 repositories, here's how to find what you're looking for:

1.  **Start at the Core:** Our `ecosystem-website` and `ecosystem-app` repos are the best places to understand the core system.
2.  **Browse the Pillars:** See which pillar or sector above interests you most.
3.  **Explore Products:** Check out our `durasagv-` repos to see how the ecosystem comes together.
4.  **Filter by Topic:** We use topics like `pillar-hub`, `sector-agro`, `product`, and `help-wanted` to organize work.

---
We are committed to fostering an open and welcoming environment. Please read our [Code of Conduct](../CODE_OF_CONDUCT.md) before participating.
