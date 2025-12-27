# Global Governance Frameworks

**Research initiative developing crisis-resilient digital infrastructure and governance frameworks for democratic systems.**

---

## About This Initiative

Global Governance Frameworks (GGF) is a research and development initiative led by Björn Kenneth Holmström, systems architect and independent researcher based in Sweden. We develop open-source infrastructure and governance frameworks that enable communities, municipalities, and democratic organizations to maintain critical functions during crises while fostering human flourishing in peacetime.

**Organizational Status:** GGF is currently a research initiative, not a registered legal entity. We operate through open-source development, institutional partnerships, and grant funding. Formal organizational structure will be established as projects scale and funding is secured.

---

## Our Work: Two Interconnected Streams

### 🛡️ Crisis-Resilient Infrastructure (Sweden Focus)

**Developing offline-first, peer-to-peer systems for Swedish totalförsvar and municipal resilience.**

Modern societies are dangerously dependent on centralized, internet-reliant infrastructure. The November 2024 Baltic Sea cable cuts demonstrated this vulnerability. We build systems that work when the internet doesn't.

**Active Projects:**

#### [CivicBase](https://github.com/GlobalGovernanceFrameworks/CivicBase)
Offline-first P2P platform for Swedish municipal infrastructure.

**Technology:** libp2p, agent-centric data model, end-to-end encryption  
**Status:** Proof-of-concept with comprehensive test coverage  
**Applications:** TAK-405 (transit wellness), DPOP (democratic organizing), DiDiS (distributed identity)  
**Funding:** Vinnova grant application pending (2.5M SEK, 12 months)  
**Partnerships:** Upplands Väsby kommun, Civilförsvarsförbundet, MCF (in discussion)

**Why P2P, not blockchain?** 
- Blockchain requires internet for global consensus (fails during crisis)
- P2P enables local mesh networks that function offline
- Lower energy consumption, GDPR-compliant, faster transactions
- Proven technology (IPFS, Filecoin use libp2p globally)

#### Stuga (Neighborhood Coordination)
Local community resilience application built on CivicBase platform.

**Purpose:** Enable neighbors to coordinate resources and mutual aid during crises  
**Technology:** CivicBase + Bluetooth/Wi-Fi Direct mesh networking  
**Status:** Early development  
**Pilot:** Upplands Väsby (planned)  
**Partners:** Civilförsvarsförbundet Väsby (in discussion)

#### love-ledger** - Care economy tracking framework (conceptual + reference)  
Status: Research project  
Focus: Global care economy valorization  
Currency: Hearts (values care work and mutual aid)

## Repository Structure
```
GlobalGovernanceFrameworks/
├── CivicBase/              (Platform - infrastructure)
├── Stuga/                  (Application - Swedish crisis)
│   └── Uses: CivicBase + love-ledger concepts
├── love-ledger/            (Framework - care economy)
│   └── Can run on: CivicBase
└── governance-framework-site/  (Frameworks - global)
```

### 🌍 Governance Frameworks (Global Focus)

**Exploring patterns for planetary coordination, economic justice, and human development.**

Our governance frameworks are thought experiments and conceptual tools - not prescriptive solutions, but starting points for communities to adapt to their own contexts.

#### [Governance Frameworks Website](https://github.com/GlobalGovernanceFrameworks/governance-framework-site)
Repository of governance patterns and frameworks for planetary challenges.

**Key Explorations:**
- **Adaptive Universal Basic Income (AUBI):** Framework for economic security + purposeful engagement
- **Hearts & Leaves Currency:** Valuing care work and ecological stewardship
- **Bioregional Autonomous Zones:** Decentralized governance at ecosystem scale
- **Treaty for Our Only Home:** Legal frameworks for planetary coordination
- **Moral Operating System:** Rights framework for all beings

**Philosophy:** These are not a rigid system to implement, but a "mycelial network of possibilities" - patterns that can take root in different contexts, inspire new thinking, or serve as compost for entirely different solutions.

**Technologies:** SvelteKit, Tailwind CSS, Custom i18n (multilingual)  
**Status:** Active development, accepting contributions

---

## The Connection: Local Resilience + Global Coordination

**Why both streams?**

1. **Crisis infrastructure** (CivicBase/Stuga) shows resilience is possible at municipal scale
2. **Governance frameworks** explore what becomes possible when basic security is established
3. Both challenge centralized control in favor of distributed, adaptive systems
4. Technical infrastructure enables governance experimentation; governance frameworks guide technical development

**Example synthesis:**
- CivicBase provides offline-capable infrastructure
- AUBI framework suggests economic models for communities using that infrastructure
- Stuga demonstrates local coordination that could scale bioregionally
- Hearts currency could run on CivicBase to value community care work

---

## Team & Contributors

### Core Team

**Björn Kenneth Holmström** - Founder & Lead Architect  
Independent researcher, systems architect  
Background: Civil engineering studies, mathematical optimization, distributed systems  
Location: Upplands Väsby, Sweden  
Contact: bjorn.kenneth.holmstrom@gmail.com

**Distributed Systems Consultant** - Position open (pending CivicBase funding)  
Expertise sought: libp2p/P2P architecture, offline-first systems, cryptography  
Funding: 800K SEK (12-month contract, Vinnova grant)

### Contributors

We welcome contributions to:
- Code (infrastructure, website)
- Frameworks (conceptual development, case studies)
- Translations (governance frameworks in multiple languages)
- Documentation (technical writing, policy analysis)
- Institutional partnerships (municipalities, civil defense, research institutions)

See individual repository CONTRIBUTING.md files for details.

---

## Active Institutional Dialogues

**Swedish Municipal & Civil Defense:**
- Upplands Väsby kommun (beredskapsamordnare) - Reference municipality for CivicBase pilot
- Civilförsvarsförbundet Väsby - Stuga community integration
- Myndigheten för civilt försvar (MCF) - Totalförsvar pilot funding
- Region Stockholm - TAK-405 transit wellness collaboration

**Research & Innovation:**
- Vinnova - Innovation grant application (CivicBase development)
- RISE Research Institutes - Potential distributed systems partnership
- KTH/Uppsala University - Academic collaboration (exploring)

**Civil Society:**
- Fjärilspartiet (Swedish political party) - Policy advocacy for crisis-resilient infrastructure (STR-506)
- Local FRG groups (Frivilliga resursgrupper) - Community resilience integration

*Note: These are ongoing conversations, not formal partnerships. We update as relationships solidify.*

---

## Funding Strategy

### Current Applications

**CivicBase Development (Vinnova)**
- Amount: 2.5M SEK
- Duration: 12 months
- Status: Pending institutional backing from Upplands Väsby
- Use: Platform development, distributed systems consultant, security audit, municipal integration

**MCF Totalförsvar Pilot**
- Amount: TBD (pilot funding scale)
- Focus: Stuga + CivicBase integration with FRG groups
- Status: Exploratory conversations

**TAK-405 External Funding (Region Stockholm)**
- Amount: 80% of project cost (MCF covers 20%)
- Focus: Hearts currency + transit wellness
- Status: Exploring integration with CivicBase platform

### Philosophy

We prioritize:
1. **Institutional partnerships first** (credibility, sustainability)
2. **Public funding** (aligns with public infrastructure mission)
3. **Open source always** (AGPL-3.0 for infrastructure ensures improvements stay public)
4. **No venture capital** (avoids profit-driven feature creep)

---

## Technical Approach

### Infrastructure Projects (CivicBase/Stuga)

**Architecture Principles:**
- **Offline-first:** Works without internet, syncs when available
- **Peer-to-peer:** No central server to fail or censor
- **Agent-centric:** Users own their data, not platforms
- **End-to-end encrypted:** AES-256-GCM, Ed25519 signatures
- **GDPR by design:** Data sovereignty built-in, not bolted-on

**Technology Stack:**
- **Networking:** libp2p (IPFS/Filecoin standard)
- **Database:** SQLite per-device, eventual consistency
- **Sync:** Vector clocks + last-write-wins conflict resolution
- **Security:** Defense in depth, professional audit planned (400K SEK)
- **Platforms:** JavaScript/TypeScript SDK, React Native mobile

**Development Methodology:**
- Test-driven (comprehensive integration + offline scenario tests)
- Security-first (external audit before production)
- Iterative (pilot → regional → national)
- Open source (AGPL-3.0)

### Governance Frameworks

**Philosophy:**
- Conceptual exploration, not prescriptive blueprints
- Synthesis of developmental psychology, systems thinking, indigenous wisdom
- Emphasis on adaptation over adoption
- Recognition that comprehensive solutions often fail; distributed experimentation succeeds

**Approach:**
- Collaborative writing (GitHub-based)
- Multilingual from start (i18n built-in)
- Visual thinking (diagrams, interactive components)
- Real-world grounding (case studies, pilot implications)

---

## How We Work

### Open Source Principles

**Code:**
- All infrastructure code: AGPL-3.0 (copyleft ensures improvements stay public)
- Website code: MIT (permissive for maximum reuse)
- Frameworks: CC BY-SA 4.0 (attribution + share-alike)

**Why AGPL for infrastructure?**
- Prevents vendor lock-in (municipalities can't be held hostage)
- Network copyleft (running as service requires sharing modifications)
- Enables competitive support market (multiple vendors can offer services)
- Aligns with public infrastructure mission

**Development:**
- Public repositories (transparent from day one)
- GitHub Discussions (open technical and strategic conversations)
- Issue tracking (bugs, features, documentation needs)
- Security: Private disclosure for vulnerabilities (email first, public after patch)

### Communication

**For general inquiries:**  
globalgovernanceframeworks@gmail.com

**For technical questions:**  
GitHub Issues or Discussions in relevant repository

**For institutional partnerships:**  
bjorn.kenneth.holmstrom@gmail.com

**For crisis infrastructure pilots:**  
bjorn.kenneth.holmstrom@gmail.com

**Social:**
- LinkedIn: Björn Kenneth Holmström (personal updates, thought leadership)
- Twitter/X: @BKHolmstrom (occasional)
- WordPress: [bjornkennethholmstrom.wordpress.com](https://bjornkennethholmstrom.wordpress.com)

---

## Repositories

### Active Projects

**[CivicBase](https://github.com/GlobalGovernanceFrameworks/CivicBase)** - Offline-first municipal infrastructure  
**[governance-framework-site](https://github.com/GlobalGovernanceFrameworks/governance-framework-site)** - Frameworks website  
**Stuga** - Community resilience app (coming soon)

### Documentation & Resources

**[.github](https://github.com/GlobalGovernanceFrameworks/.github)** - Organization profile and guidelines (this file)

*More repositories will be added as projects develop.*

---

## Vision & Long-Term Direction

### 2025-2026: Proof of Concept
- CivicBase pilots in 2-3 Swedish municipalities
- Stuga integration with Civilförsvarsförbundet
- Governance frameworks website launch (multilingual)
- First institutional partnerships formalized

### 2027-2028: Regional Expansion
- 10-20 municipalities using CivicBase
- Regional mesh networks demonstrated
- National standards proposed (offline-first IT for totalförsvar)
- Academic partnerships (RISE, KTH)
- EU collaboration (digital sovereignty initiatives)

### 2029-2030: Systems Thinking at Scale
- Sweden recognized as leader in resilient infrastructure
- Governance frameworks adopted by communities globally (adapted to local contexts)
- GGF formalized as ideell förening or equivalent structure
- Export Swedish crisis infrastructure expertise
- Connect infrastructure resilience to governance frameworks (e.g., Hearts currency on CivicBase)

### Long-Term (2030+): Regenerative Coordination
- Bioregional implementation of governance frameworks
- Crisis infrastructure as standard for democratic systems globally
- Integration of care economies (Hearts) with resilient platforms
- Contribution to planetary coordination without centralized control

---

## What We're NOT

**We are not:**
- ❌ A startup seeking venture capital
- ❌ A consulting company selling proprietary solutions
- ❌ A political organization (though we support policy change)
- ❌ A comprehensive solution to all problems
- ❌ Claiming to have all the answers

**We are:**
- ✅ A research initiative exploring possibilities
- ✅ Open-source developers building public infrastructure
- ✅ Systems thinkers connecting local resilience to global coordination
- ✅ Honest about what we don't know
- ✅ Building tools, not prescribing outcomes

---

## Get Involved

### For Municipalities
Interested in piloting offline-first infrastructure? We're seeking reference municipalities for CivicBase testing.  
Contact: bjorn.kenneth.holmstrom@gmail.com

### For Developers
- Review [CivicBase](https://github.com/GlobalGovernanceFrameworks/CivicBase) codebase
- Open issues, suggest improvements
- Contribute code (see CONTRIBUTING.md)
- Help with testing (especially offline scenarios)

### For Researchers
- Governance frameworks collaboration
- Academic partnerships (distributed systems, crisis preparedness)
- Case study development

### For Civil Defense Organizations
- Stuga integration with FRG groups
- Offline coordination training
- Municipal preparedness integration

### For Translators
- Governance frameworks website (multilingual)
- Swedish ↔ English technical documentation

### For Funders
We're transparent about funding needs and uses. See individual repositories for grant applications and budgets.

---

## Frequently Asked Questions

**Q: Is Global Governance Frameworks a registered organization?**  
A: No, we're currently a research initiative. We'll formalize as ideell förening (non-profit association) when appropriate, likely upon securing significant funding.

**Q: Why offline-first instead of blockchain?**  
A: Blockchain requires internet for global consensus, making it useless during crises. P2P systems like libp2p work offline via mesh networks, use less energy, respect GDPR, and are faster. See [CivicBase Architecture](https://github.com/GlobalGovernanceFrameworks/CivicBase/blob/main/docs/CURRENT/ARCHITECTURE.md) for details.

**Q: How do governance frameworks relate to infrastructure?**  
A: Infrastructure enables governance experimentation (can't build AUBI without working systems), and frameworks guide infrastructure design (Hearts currency needs offline-capable platform). They're synergistic, not separate.

**Q: Is this related to Fjärilspartiet?**  
A: Björn Kenneth Holmström is founder of both. Fjärilspartiet (Swedish political party) advocates for policies like crisis-resilient infrastructure (see STR-506), but GGF is independent. We build tools; they advocate policy. Related but distinct.

**Q: Can we use your frameworks/code for our project?**  
A: Yes! Code is AGPL-3.0 (copyleft), frameworks are CC BY-SA 4.0 (attribution + share-alike). Adapt freely, share improvements.

**Q: How can we support this work?**  
A: Institutional partnerships > funding > code contributions > sharing the work. We need credible partners more than money right now.

---

## License Information

**Infrastructure Code (CivicBase, etc.):** AGPL-3.0  
- Why: Ensures public infrastructure improvements stay public
- Implication: Modifications must be shared, even when running as network service
- Benefit: Prevents vendor lock-in, enables competitive support market

**Website Code:** MIT  
- Why: Maximum reuse and adaptation
- Implication: Can be used commercially without sharing modifications

**Governance Frameworks:** CC BY-SA 4.0  
- Why: Encourages adaptation with attribution
- Implication: Must credit GGF and share derivatives under same license

See individual repositories for full license text.

---

## Acknowledgments

This initiative builds on ideas from:
- Distributed systems research (IPFS, libp2p, Holochain)
- Swedish totalförsvar doctrine (MCF 2024:1032)
- Indigenous governance systems and traditional ecological knowledge
- Developmental psychology (Spiral Dynamics, Kegan's stages)
- Regenerative economics (Kate Raworth, Charles Eisenstein)
- Democratic innovation (Audrey Tang's g0v, Taiwan's civic tech)

We stand on the shoulders of countless researchers, practitioners, and communities who've explored these questions before us.

---

**Global Governance Frameworks**  
*Building infrastructure for resilience. Exploring frameworks for flourishing.*

Last updated: 2025-12-27  
Contact: globalgovernanceframeworks@gmail.com
