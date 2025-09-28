<!-- Amicus POS README -->

<div align="center">

<h1>Amicus POS</h1>

<p>
Franchise-ready, multi-store, cloud-first Point of Sale — built with care in my spare time for a friend. ❤️
</p>

<p><em>Open source POS system designed for small franchises. Modular, API-first, offline-tolerant terminals with seamless sync.</em></p>

<p>
  <img alt="Open Source Love" src="https://img.shields.io/badge/Open%20Source-love-ff69b4?style=for-the-badge&logo=opensourceinitiative&logoColor=white" />
  <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen?style=for-the-badge&logo=github" />
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue?style=for-the-badge&logo=semver" />
  <img alt="Status" src="https://img.shields.io/badge/status-early%20work--in--progress-orange?style=for-the-badge" />
</p>

</div>

---

### Mission

Build a practical, reliable POS that helps small franchises run smoothly — simple to operate at the counter, safe and compliant under the hood, and easy to extend as needs grow.

### Goals

- Deliver a usable MVP for a single store, then scale to multi-store.
- Keep the system modular and API-first to avoid tight coupling.
- Design for offline tolerance at terminals with seamless sync.
- Bake in security, observability, and sensible defaults from day one.

### What is this project?

Amicus POS is an open, community-friendly POS aiming to support real storefront operations (catalog, checkout, receipts, basic inventory, simple reports) while staying franchise-ready for multi-tenant growth. It starts small, favors clarity over complexity, and iterates quickly.

### Status & Update Cadence

- Side project maintained in spare time; progress may vary week to week.
- I’ll post updates and ship changes on a daily/weekly cadence.
- Expect iterative commits, feature flags, and incremental docs as things evolve.

### High-Level Feature Outline (evolving)

- POS terminal experience (cart, scan, discounts, checkout)
- Catalog (products, variants, taxes/pricing)
- Basic inventory adjustments
- Receipts/printing integrations
- Roles/permissions for staff
- Simple reporting for daily/weekly summaries

Note: A deeper architecture and roadmap document exists separately and is not included here.

### Offline-Tolerant Terminals with Seamless Sync

One of Amicus POS's core design principles is ensuring that store operations can continue smoothly even when internet connectivity is unreliable or temporarily unavailable. Here's how this works:

**Offline-First Architecture**
- Terminal devices store essential data locally (product catalog, pricing, recent transactions)
- All critical POS operations (scanning, checkout, receipt printing) work without internet
- Local database maintains transaction history and inventory changes

**Intelligent Sync Strategy**
- **Background Sync**: When connected, terminals automatically sync with the cloud in the background
- **Conflict Resolution**: Smart algorithms handle conflicts when multiple terminals modify the same data
- **Incremental Updates**: Only changed data is synchronized, reducing bandwidth and sync time
- **Queue Management**: Failed syncs are queued and retried automatically when connectivity returns

**Business Continuity Benefits**
- **Zero Downtime**: Stores can operate normally during internet outages
- **Data Integrity**: No transaction loss, even during extended offline periods
- **Multi-Store Coordination**: Changes sync across all store locations when connectivity is restored
- **Real-Time When Possible**: Live updates when connected, seamless fallback when not

This approach ensures that franchise operations remain uninterrupted regardless of network conditions, while maintaining data consistency across all locations.

---

## Contributing

First off, thank you for considering contributing — PRs and feedback are welcome!

### How to Get Started

1) Fork this repository and create a feature branch.
2) Keep edits focused and atomic; write clear commit messages.
3) Add/update minimal docs for any user-facing change.
4) Open a Pull Request describing the motivation and testing steps.

### Contribution Guidelines

- Prefer small, composable changes. Avoid large refactors without discussion.
- Reuse existing utilities/schemas when possible; keep code minimal and readable.
- Add basic tests where reasonable and ensure no lint/build errors.
- Be mindful not to break existing flows; add guards and feature flags if needed.
- Use friendly language in issues/PRs; we’re building this together.

### Communication

- File issues for bugs/ideas. Include context, expected vs actual, and repro steps.
- Discussions are welcome for larger proposals before implementation.

### Code of Conduct

Be respectful, inclusive, and constructive. Harassment or disrespectful behavior isn’t tolerated.

---

## Getting Started (WIP)

Project setup instructions will be documented as components land. Typical steps will include:

- Clone the repo and install dependencies.
- Configure environment variables (development presets will be provided).
- Run the app locally and verify basic flows.

As the stack solidifies, this section will be updated with concrete commands and configuration examples.

---

## License

This project offers multiple licensing options. Choose the one that best fits your needs:

- **MIT License** - [LICENSE-MIT](LICENSE-MIT) - Most permissive, allows commercial use
- **Apache 2.0 License** - [LICENSE-APACHE](LICENSE-APACHE) - Includes patent protection
- **GPL 3.0 License** - [LICENSE-GPL](LICENSE-GPL) - Copyleft, requires source code sharing

<div>

<img alt="MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat&logo=opensourceinitiative&logoColor=white" />
<img alt="Apache-2.0" src="https://img.shields.io/badge/License-Apache--2.0-blue.svg?style=flat&logo=apache" />
<img alt="GPL-3.0" src="https://img.shields.io/badge/License-GPL--3.0-green.svg?style=flat&logo=gnu" />

</div>

---

## Maintainer & Contact

- Author: NN
- Version: 1.0.0
- Date (UTC): 2025-09-25 14:25:06

### GitHub

<a href="https://github.com/Nitin-Anil_Narang" target="_blank">
  <img alt="GitHub - Nitin-Anil_Narang" src="https://img.shields.io/badge/GitHub-@Nitin--Anil_Narang-181717?style=for-the-badge&logo=github" />
</a>

If you find this useful, consider starring the repo and sharing feedback. PRs welcome!


