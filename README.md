# PrivaPals

**A browser-based privacy and internet safety education game for children ages 9–13.**

Developed in partnership with the [University of Michigan School of Information](https://www.si.umich.edu/) and [Privacy@Michigan](https://privacy.umich.edu/).

---

## About

PrivaPals is an interactive game designed to teach children about online privacy, data literacy, and digital surveillance through immersive, decision-based gameplay — not quizzes. Players make real choices and experience real consequences, building intuitive understanding of how personal data moves through digital systems.

The project targets a substantive gap in educational games for this age group. Every design decision is grounded in age-appropriate pedagogy (5th-grade reading level, Lauren's child development framework) and tested against the needs of real 9–13 year olds.

**Design philosophy:** decision → consequence → reflection. No account required. No data collected. COPPA-compliant.

---

## Current Prototypes

### 🏚️ Haunted Data Mansion
A first-person 3D maze game built in Three.js r128, themed after Disney's Haunted Mansion aesthetic. Players explore zones representing different data privacy threats, collect data scrolls, answer knowledge challenges, and navigate enemy encounters. Multi-level architecture with 90+ quiz questions and 15+ collectible data documents.

### 🍕 Privacy Pizza
A Papa's Pizzeria-style order management game with a 4-station gameplay loop. Players handle customer data requests, practice data minimization, and learn about consent — all through the metaphor of running a pizza shop.

---

## Getting Started

No install required. All prototypes are **single self-contained HTML files** — download and open in a browser.

```bash
git clone https://github.com/YOUR-ORG/privapals.git
cd privapals
```

Open any `.html` file directly in **Chrome or Firefox** as a `file:///` URL.

> ⚠️ Do not use VS Code's built-in preview. It sandboxes the file in an iframe and breaks browser APIs required for gameplay.

---

## Deployment

Files are designed for zero-friction deployment on school networks and Chromebooks:
- No server required
- No external dependencies (Three.js loaded via CDN)
- No accounts, logins, or data collection
- Hosted by UMich ITS at [link TBD]

---

## Performance Standards

All builds must maintain Chromebook compatibility:
- `MeshLambertMaterial` (not Phong or Standard)
- Shared geometries across repeated objects
- Single floor/ceiling planes per level
- Interior wall culling
- ≤ 8 active lights, ~300 draw calls

---

## Project Structure

```
/
├── haunted-data-mansion/       # HDM prototype (versioned)
│   └── hdm_v17.html
├── privacy-pizza/              # Privacy Pizza prototype
│   └── privacy_pizza.html
├── docs/                       # Design specs, learning objectives, COPPA plan
├── research/                   # Usability testing protocols and findings
└── README.md
```

---

## Educational Framework

**Learning objectives** (6 core):
1. Recognize how apps collect data without explicit consent
2. Understand the concept of a digital footprint
3. Identify phishing and social engineering tactics
4. Practice password hygiene and account security
5. Understand data sharing and third-party access
6. Develop habits of privacy-conscious decision-making

All content is written at a **5th-grade reading level** and reviewed by a child development specialist.

---

## Team

| Name | Role |
|------|------|
| Eric | Product & Engineering Lead |
| Sol | Faculty Advisor, UMich UMSI |
| Sarafina | UX Design |
| Grace | Content & Narrative |
| Lauren | Child Development & Education |
| UMich ITS | Hosting & Infrastructure |

---

## Contributing

This project is in active development. If you're a future intern or ITS team member picking this up — welcome. Start with `/docs` for design decisions and open questions, then review the latest prototype version before making changes.

All decisions, pivots, and known issues are logged in `/docs/decisions.md`.

---

## License

[TBD — confirm with UMich UMSI before public release]

---

*A Privacy@Michigan project · University of Michigan School of Information*
