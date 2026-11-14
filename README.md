# Awesome-Electronic-Signature-Software

# Top Electronic Signature Software Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Legally Binding E-Signatures, Audit Trails & Self-Hosted Signing Workflows*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Electronic Signature Software**. These tools help organizations send documents for legally binding signatures—covering envelope creation, field placement, signer authentication, audit trails, and the cryptographic sealing of completed PDFs.

**Examples** include DocuSign, Adobe Acrobat Sign, Dropbox Sign, PandaDoc, SignNow, OneSpan Sign, DocuSeal, Documenso, and OpenSign (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted e-signature workflows, open-source PDF signing engines, and community-driven document execution—ideal for developers embedding signing into their own products and organizations seeking data sovereignty over per-envelope SaaS pricing. The open-source landscape has matured significantly: **DocuSeal** leads with a WYSIWYG PDF editor and unlimited envelopes on the free Community Edition , **Documenso** offers a modern Next.js/TypeScript alternative with passkey signing , and **OpenSign** provides a Node.js/MongoDB option with detailed audit trails .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[DocuSign](https://www.docusign.com/)** | Industry-standard e-signature platform with envelopes, templates, and certificate of completion. **Per-user seat pricing with envelope caps** on lower tiers. Free developer sandbox available for API testing, but production requires a paid plan . | Personal: ~$10/month (1 user); Standard: ~$25/user/month (annual)  | **Free developer sandbox** (no credit card) for API testing; no permanent free tier for production . |
| **[Adobe Acrobat Sign](https://www.adobe.com/sign.html)** | E-signature bundled into Acrobat plans. **Per-license billing** with seat subscriptions. **Free Developer Edition with full REST API access and sandbox** for testing . Deep integration if your workflows are PDF-native. | Acrobat Standard with Sign: **$14.99/user/month**; Pro: $19.99/user/month  | **Free Developer Edition + sandbox** for API development; production requires paid Acrobat plan . |
| **[Dropbox Sign](https://sign.dropbox.com/)** | E-signature platform (formerly HelloSign) with **unlimited signature requests on paid plans**—no envelope caps. **Free tier: 3 signature requests per month**. Official SDKs for Python, Node, Java, C#, PHP, Ruby, Go . | Essentials: **$15/user/month** (annual, unlimited sends); Standard: $25/user/month (teams)  | **Free**: 3 signature requests/month; **Developer test mode** available for API testing . |
| **[PandaDoc](https://www.pandadoc.com/)** | Document workflow platform combining e-signature, proposals, and CPQ. Free eSign plan: **5 documents/month, 2 recipients/document**. | Free: **$0** (5 docs/month); Starter: $19/seat/month (annual)  | **Free**: 5 documents/month, 5 templates, limited API access . **14-day trial** . |
| **[SignNow](https://www.signnow.com/)** | E-signature platform with templates, role-based fields, and embedded signing. API supports template usage, invitation sending, and signed document download . | Entry: **~$8/user/month** (1 user)  | Free trial available; no permanent free tier . |
| **[OneSpan Sign](https://www.onespan.com/)** | Enterprise e-signature focused on **complex authentication and audit requirements**. Certificate-based signing, policy controls, and audit-oriented message handling. SaaS and on-premises deployment options available . | Quote-only (enterprise contract) | Free developer sandbox; trial via sales . |
| **[BoldSign](https://boldsign.com/)** | E-signature platform for **automated initiation via API**. Field auto-configuration and API-based audit record download for automated archival. Good for businesses wanting to trigger signing from business systems . | Quote-only (per-user or usage-based) | Free plan available; paid tiers for production . |

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
