# Awesome-Electronic-Signature-Software

## Top Electronic Signature Software Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Legally Binding E-Signatures, Audit Trails & Self-Hosted Signing Workflows*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Electronic Signature Software**. These tools help organizations send documents for legally binding signatures—covering envelope creation, field placement, signer authentication, audit trails, and the cryptographic sealing of completed PDFs.

**Examples** include DocuSign, Adobe Acrobat Sign, Dropbox Sign, PandaDoc, SignNow, OneSpan Sign, DocuSeal, Documenso, and OpenSign (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted e-signature workflows, open-source PDF signing engines, and community-driven document execution—ideal for developers embedding signing into their own products and organizations seeking data sovereignty over per-envelope SaaS pricing. The open-source landscape has matured significantly: **DocuSeal** leads with a WYSIWYG PDF editor and unlimited envelopes on the free Community Edition , **Documenso** offers a modern Next.js/TypeScript alternative with passkey signing , and **OpenSign** provides a Node.js/MongoDB option with detailed audit trails .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global electronic signature software market is estimated at approximately **$9 billion to $17 billion** and is projected to expand at a compound annual growth rate (CAGR) of over **25–35%** into the next decade. Structurally, the sector exhibits **moderate fragmentation with high concentration at the enterprise apex**: while legacy giants like DocuSign and Adobe command dominant brand recognition and enterprise volume, intense fragmentation exists underneath as hundreds of specialized vendors, regional compliance leaders (e.g., eIDAS/QES focused), and API-first alternatives compete across localized workflows and specific vertical niches.

## SaaS/Hosted Platforms

| Product | Company Size (Valuation / Revenue) | Description | Starting Tier Pricing | Free Tier / Trial Limits |
|---------|-----------------------------------|-------------|-----------------------|--------------------------|
| **[Adobe Acrobat Sign](https://www.adobe.com/sign.html)** | **~$93B Market Cap** (~$26B Revenue) | E-signature bundled into Acrobat plans. Deep integration for PDF-native document workflows and enterprise compliance. | **$14.99/user/month** (Acrobat Standard, billed annually) | **7-day free trial** (Acrobat Pro with Sign) / **30-day enterprise trial** (capped at 200 transactions) |
| **[DocuSign](https://www.docusign.com/)** | **~$15B Market Cap** (~$3.4B Revenue) | Industry-standard e-signature and agreement lifecycle platform with templates, routing, and certificates of completion. | **$10/month** (Personal plan, 1 user, billed annually) | **30-day free trial** (access to send up to ~100 test envelopes; forever-free account is receive-and-sign only with 0 sends) |
| **[Dropbox Sign](https://sign.dropbox.com/)** | **~$7.5B Market Cap** (~$2.5B Revenue, Dropbox) | E-signature platform (formerly HelloSign) featuring unlimited signature requests on paid tiers and developer-friendly SDKs. | **$15/user/month** (Essentials plan, billed annually) | **Free forever plan**: **3 signature requests/month** (or 30-day trial for team features) |
| **[signNow](https://www.signnow.com/)** | **~$1.25B Valuation** (~$200M Revenue, airSlate) | Intuitive e-signature platform with configurable signing roles, document generation, and embedded signing workflows. | **$8/user/month** (Business plan, billed annually) | **7-day free trial** (includes all standard features, up to 100 invites/user limit); no permanent free sending plan |
| **[PandaDoc](https://www.pandadoc.com/)** | **~$1.0B Valuation** (~$100M+ ARR) | All-in-one document automation combining proposals, quotes (CPQ), contract workflows, and digital signing. | **$19/user/month** (Starter plan, billed annually) | **Free forever plan**: **5 documents/month**, 5 templates, basic e-signatures (or 14-day trial of paid plans) |
| **[OneSpan Sign](https://www.onespan.com/)** | **~$780M Market Cap** (~$255M Revenue) | Enterprise digital signature platform tailored for high-security authentication, strict regulatory compliance, and audit trails. | **$20/user/month** (Professional plan, billed annually) | **30-day free trial** (full access up to standard envelope evaluation, no credit card required) |
| **[BoldSign](https://boldsign.com/)** | **~$50M–$75M Est. Revenue** (Syncfusion) | Modern e-signature software and developer API designed for automated initiation, customizable branding, and audit tracking. | **$5/user/month** (Growth plan, billed annually) | **Free forever plan**: **25 envelopes/month** (5 envelopes/mo for personal email addresses), 1 user, 2 templates |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[DocuSeal](https://github.com/docusealco/docuseal)** | [![Stars](https://img.shields.io/github/stars/docusealco/docuseal?style=social&color=white)](https://github.com/docusealco/docuseal/stargazers) | **The leading open-source DocuSign alternative with the most complete free edition.** AGPL-3.0, Ruby on Rails + PostgreSQL. **Free Community Edition: unlimited envelopes and seats**. WYSIWYG PDF form editor with **12 field types** (signature, date, file, checkbox, etc.), multiple signatories, automated email notifications, and **tamper-evident audit certificate**. **AI-powered field detection** (v2.3.0+) automatically identifies form fields in PDFs. Docker deployment (SQLite default, PostgreSQL/MySQL optional). Pro adds white-labeling, SSO/SAML, SMS verification, and embedded signing . **Best for teams wanting a mature, feature-complete self-hosted signing platform.** |
| **[Documenso](https://github.com/documenso/documenso)** | [![Stars](https://img.shields.io/github/stars/documenso/documenso?style=social&color=white)](https://github.com/documenso/documenso/stargazers) | **The modern TypeScript/Next.js e-signature platform—"Stripe for Signatures."** AGPL-3.0. **Free Community Edition includes core signing, templates, and API access**. Advanced multi-party signing order, **passkey signing authentication**, SHA-256 hash + audit log, and cryptographic PDF signing with optional timestamp authority (RFC 3161). **Full REST API with webhooks** for integration. Team collaboration with SSO. Docker/Kubernetes/Railway deployment . **Best for developer platforms wanting a modern stack with strong API and passkey support.** |
| **[OpenSign](https://github.com/OpenSignLabs/OpenSign)** | [![Stars](https://img.shields.io/github/stars/OpenSignLabs/OpenSign?style=social&color=white)](https://github.com/OpenSignLabs/OpenSign/stargazers) | **Node.js/MongoDB e-signature with full document lifecycle management.** AGPL-3.0 with specific directory exceptions (check LICENSE). **Cryptographic signing, detailed audit trails with IP tracking**, completion certificates, reusable templates, signing order, guest email verification codes, and REST API. Freemium model. Docker deployment with MongoDB, SMTP/Mailgun, and signature certificates . **Best for teams wanting a Node.js-based platform with customizable PDF generation templates.** |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Penpact](https://github.com/penpact/penpact)** | [![Stars](https://img.shields.io/github/stars/penpact/penpact?style=social&color=white)](https://github.com/penpact/penpact/stargazers) | **Developer-first open-source e-signature API for embedding signing in your own product.** AGPL-3.0. **Early development (v0.1.0)**—signing engine works end-to-end but API is not yet stable. Features: **in-document signing** with guided field flow, **AI field detection** (Claude/Gemini/GPT proposes fields), themeable React component, typed `@penpact/sdk` (TypeScript) + Python/Go/PHP clients, **append-only audit trail with IP/timestamps**, PAdES digital signature on sealed PDF, Certificate of Completion, templates with variable merge, bulk send via CSV, and HMAC-signed webhooks. **No per-seat billing**; free forever when self-hosted . **Best for developers embedding signing into a SaaS product—but not yet production-ready.** |

**Frameworks for building custom systems**: Choose **DocuSeal** for the most mature turnkey self-hosted e-signature platform with unlimited envelopes and AI field detection , **Documenso** for a TypeScript-native stack with passkey authentication and strong API , or **OpenSign** for a Node.js/MongoDB alternative with customizable templates . For embedding signing directly into your product, **Penpact** provides a developer-first API with AI field detection—but note it is **early-stage (v0.1.0)** and the API is not yet stable .

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- E-signature platforms handle legally binding agreements and signer PII; ensure compliance with ESIGN, UETA, eIDAS, and applicable data protection regulations. **Audit trails and certificate integrity are legally critical**—do not deploy open-source signing without validating the tamper-evidence of completed PDFs.
- **Open-source e-signature licensing is exclusively copyleft.** Every actively maintained project is AGPL-3.0 or similar—**no permissive (MIT/Apache) option exists**. If your organization restricts copyleft software, these projects may not be viable for embedding in proprietary products. **DocuSeal** is AGPL-3.0 with Pro paid tiers for API/embedding and white-labeling . **Documenso** is AGPL-3.0 . **OpenSign** is AGPL-3.0 **with directory exceptions**—review the LICENSE carefully before commercial use . **Penpact** is AGPL-3.0 and **v0.1.0 early development**—the README explicitly states it is not yet stable and the consent text is pending legal review . **Commercial platforms have differing pricing models**: DocuSign and Adobe use **per-seat subscriptions** (predictable for small teams, expensive for automated volume) . Dropbox Sign uses **signature-request volume** (API Essentials: $75/month for 50 requests) which scales with automation . **All major vendors offer free developer sandboxes but charge for production**—budget the production tier during architecture, not after prototyping .

---

**Made for developers, legal ops teams, and organizations building document signing infrastructure.**  
Let's make electronic signature software more open, verifiable, and accessible.
