# 🌍 NovaEco — Digital Public Infrastructure for the Circular Economy

**NovaEco** is the open‑source **Digital Public Infrastructure** for the circular economy.  
It connects individuals and siloed sectors to **foster innovation**, measure impact, and **collaborate** within a federated system-of-systems.

NovaEco is commercially supported by **[Circular Engineering Nova GmbH](https://circular.engineering/)**.

---

## 🚀 Key Entry Points

The ecosystem is anchored by **four core services** that provide unified identity, orchestration, and access management:

- 📊 **[Central App](https://app.novaeco.tech)** — Mission Control for onboarding, discovery, and ecosystem management.
- 🔐 **[Identity Service](https://auth.novaeco.tech)** — Digital Passport & Trust Profile for unified login.
- 🔗 **[API Gateway](https://api.novaeco.tech)** — API gateway for secure, managed access to all services.
- 🌐 **[Website & Docs](https://novaeco.tech)** — Architecture, use cases, and developer guides.
- 💬 **Contact:** [contact@novaeco.tech](mailto:contact@novaeco.tech)

---

## 🏗️ Architecture Overview

NovaEco follows a **Federated Monorepo model**. Each **Enabler** or **Sector** is a self-contained monorepo that groups its API, App, Website, and Tests together.

### 1. Core Monorepo — [`ecosystem-core`](https://github.com/novaeco-tech/ecosystem-core)
The “heart” of the ecosystem, containing the tightly‑coupled central services.

### 2. Horizontal Enabler Monorepos
Cross‑cutting foundational services:
- **[NovaHub](https://github.com/novaeco-tech/novahub)** — Innovation wizard, complex problem decomposition, orchestration.
- **[NovaFin](https://github.com/novaeco-tech/novafin)** — Tokens, staking, payments, revenue sharing, investment.
- **[NovaTrade](https://github.com/novaeco-tech/novatrade)** — Decentralized marketplace for goods, services, and assets.
- **[NovaSapien](https://github.com/novaeco-tech/novasapien)** — Shared artificial intelligence and ML models.
- **[NovaEnergy](https://github.com/novaeco-tech/novaenergy)** — Renewable energy production, distribution, and auditing.
- **[NovaMaterial](https://github.com/novaeco-tech/novamaterial)** — Digital Product Passports (DPPs), lifecycle tracking.
- **[NovaMobility](https://github.com/novaeco-tech/novamobility)** — Circular logistics and sustainable transport coordination.
- **[NovaInfra](https://github.com/novaeco-tech/novainfra)** — Shared digital/physical infrastructure.
- **[NovaSkills](https://github.com/novaeco-tech/novaskills)** — Education, skill‑sharing, labor coordination.
- **[NovaPolicy](https://github.com/novaeco-tech/novapolicy)** — Governance, compliance, legal frameworks.
- **[NovaBalance](https://github.com/novaeco-tech/novabalance)** — Environmental auditing, proof of ecological impact.
- **[NovaEquity](https://github.com/novaeco-tech/novaequity)** — Social auditing, proof of fairness and social impact.

### 3. Vertical Sector Monorepos
Industry‑specific applications consuming Enablers:
- **[NovaAgro](https://github.com/novaeco-tech/novaagro)** — Sustainable agriculture, bio‑nutrients, post‑harvest processing.
- **[NovaWater](https://github.com/novaeco-tech/novawater)** — Water resource management, sustainable use, restoration.
- **[NovaBuild](https://github.com/novaeco-tech/novabuild)** — Sustainable construction, circular building materials.
- **[NovaTextile](https://github.com/novaeco-tech/novatextile)** — Lifecycle of textiles, sustainable sourcing, recycling.
- **[NovaWaste](https://github.com/novaeco-tech/novawaste)** — Waste‑to‑value streams, recycling management.
- **[NovaAir](https://github.com/novaeco-tech/novaair)** — Air quality monitoring, environmental credits.
- **[NovaHealth](https://github.com/novaeco-tech/novahealth)** — Circular economy principles in healthcare.
- **[NovaPack](https://github.com/novaeco-tech/novapack)** — Reusable packaging systems, deposit models.
- **[NovaTronix](https://github.com/novaeco-tech/novatronix)** — Sustainable electronics, modular design, repair.
- **[NovaChem](https://github.com/novaeco-tech/novachem)** — Sustainable chemical processes, leasing models.

### 4. Worker Repos
Decoupled, single‑purpose backend services (e.g., `novahub-worker-sync`) for scalability and fault isolation.

### 5. Product Repos
Flagship applications that consume multiple enablers and sectors:
- **[DurasAGV](https://github.com/novaeco-tech/product-durasagv)** – autonomous logistics robots integrating NovaSapien and NovaAgro.
- **Urban Mining Coordination** – orchestration app combining NovaBuild, NovaWaste, and NovaMobility.
- **Reusable Packaging Systems** – products integrating NovaPack, NovaMobility, and NovaWater.
- **City‑Wide Loop** – unified reusable cup system across entire cities.
- **Circular Hospital** – healthcare equipment leasing and reuse models.

### 6. Governance & Tooling Repos
- **[ecosystem-devtools](https://github.com/novaeco-tech/ecosystem-devtools)** — Shared CLI, Docker images, and standard developer configurations.
- **[ecosystem‑qa](https://github.com/novaeco-tech/ecosystem-qa)** — Integration testing gatekeeper for the ecosystem.
- **[ecosystem‑releases](https://github.com/novaeco-tech/ecosystem-releases)** — CalVer‑tagged release manifests and BOMs.

---

## 🤝 Contributing

We welcome contributors of all kinds — code, docs, design, and governance.  
Start with our [Contribution Guide](../CONTRIBUTING.md) and [Code of Conduct](../CODE_OF_CONDUCT.md).

**Finding your way:**
1. Begin with [`ecosystem-core`](https://github.com/novaeco-tech/ecosystem-core) to understand the platform.  
2. Explore Enabler or Sector repos that match your interests.  
3. Check out Product repos to see how everything comes together.  
4. Look at Worker repos for backend microservices.

---

NovaEco is committed to openness, transparency, and collaboration. Together we can build the operating system for a truly circular economy.