# 🌍 NovaEco — The Open‑Source Operating System for a Circular Economy

NovaEco is an open‑source community building the **system‑of‑systems** needed to transition our planet to a sustainable, circular model.  
We engineer the interconnected **Horizontal Enablers** and **Vertical Sectors** that empower individuals, companies, and governments to collaborate transparently.

NovaEco is commercially supported by **[Circular Engineering Nova GmbH](https://circular.engineering/)**.

---

## 🚀 Key Entry Points

- 🌐 **Website & Docs:** [novaeco.tech](https://novaeco.tech) — Architecture, guides, and contributor documentation  
- 📊 **Central App:** [app.novaeco.tech](https://app.novaeco.tech) — Your “Mission Control” dashboard  
- 🔗 **API Gateway:** [api.novaeco.tech](https://api.novaeco.tech) — Unified REST API front door  
- 🔐 **Identity Service:** [auth.novaeco.tech](https://auth.novaeco.tech) — SSO & contributor passports  
- 💬 **Contact:** [contact@novaeco.tech](mailto:contact@novaeco.tech)

---

## 🏗️ Architecture Overview

NovaEco follows a **monorepo model** for atomic, coordinated development. Instead of scattering code across many small repos, each **Enabler** or **Sector** groups its API, App, Website, and Tests together.

### 1. Core Monorepo — [`ecosystem-core`](https://github.com/novaeco-tech/ecosystem-core)
The “heart” of the ecosystem, containing the tightly‑coupled central services:
- `/app` — Mission Control dashboard
- `/auth` — Identity & SSO provider  
- `/api` — Central API Gateway  
- `/website` — Public docs and landing site (Docusaurus)

### 2. Horizontal Enabler Monorepos
Cross‑cutting foundational services:
- **NovaHub** — innovation wizard, complex problem decomposition, orchestration.  
- **NovaFin** — tokens, staking, payments, revenue sharing, investment.
- **NovaTrade** — decentralized marketplace for goods, services, and assets.
- **NovaSapien** — shared artificial intelligence and ML models.  
- **NovaEnergy** — renewable energy production, distribution, and auditing.
- **NovaMaterial** — Digital Product Passports (DPPs), lifecycle tracking of raw/recycled materials. 
- **NovaMobility** — circular logistics and sustainable transport coordination.  
- **NovaInfra** — shared digital/physical infrastructure.  
- **NovaSkills** — education, skill‑sharing, labor coordination.
- **NovaPolicy** — governance, compliance, legal frameworks.
- **NovaBalance** — environmental auditing, proof of ecological impact.
- **NovaEquity** — social auditing, proof of fairness and social impact.

### 3. Vertical Sector Monorepos
Industry‑specific applications consuming Enablers:
- **NovaAgro** — sustainable agriculture, bio‑nutrients, post‑harvest processing.  
- **NovaWater** — water resource management, sustainable use, ecosystem restoration.
- **NovaBuild** — sustainable construction, circular building materials, built environment.
- **NovaTextile** — texlifecycle of textiles, sustainable sourcing, recycling, reuse.
- **NovaWaste** — waste‑to‑value streams, recycling, circular waste management.
- **NovaAir** — air quality monitoring, environmental credits.  
- **NovaHealth** — circular economy principles in healthcare and life sciences.
- **NovaPack** — reusable and circular packaging systems, deposit models, reverse logistics, inventory management.  
- **NovaTronix** — sustainable electronics and e‑waste management, modular design, repair, recycling, and material recovery.
- **NovaChem** — sustainable chemical processes, leasing models, and closed‑loop industrial chemistry.

### 4. Worker Repos
Decoupled, single‑purpose backend services (e.g., `novahub-worker-sync`, `novabalance-worker-impact-calculator`) for scalability and fault isolation.
They handle background jobs such as:
- Data ingestion and normalization
- Automated LCA calculations
- Compliance checks
- Logistics optimization

Workers are independent for scalability and fault isolation.

### 5. Product Repos
Flagship applications that consume multiple enablers and sectors:
- **DurasAGV** – autonomous logistics robots integrating AI and Agro.
- **Urban Mining Coordination** – orchestration app combining Build, Waste, and Mobility.
- **Reusable Packaging Systems** – products integrating Pack, Mobility, and Water.
- **City‑Wide Loop** – unified reusable cup system across entire cities.
- **Circular Hospital** – healthcare equipment leasing and reuse models.

### 6. Governance Repos
- **ecosystem‑qa** — tests the seams between Enablers and Sectors  
- **ecosystem‑releases** — CalVer‑tagged release manifests

---

## 🤝 Contributing

We welcome contributors of all kinds — code, docs, design, and governance.  
Start with our [Contribution Guide](CONTRIBUTING.md) and [Code of Conduct](CODE_OF_CONDUCT.md).

**Finding your way:**
1. Begin with [`ecosystem-core`](https://github.com/novaeco-tech/ecosystem-core) to understand the platform.  
2. Explore Enabler or Sector repos that match your interests.  
3. Check out product repos to see how everything comes together.  
4. Look at worker repos for backend microservices.

---

NovaEco is committed to openness, transparency, and collaboration. Together we can build the operating system for a truly circular economy.
