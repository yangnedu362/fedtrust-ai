# FedTrust.ai

A single-page academic research portal led by Prof. Yang Li, Northeast Electric Power University.

Live site: https://fedtrust.ai/

## Maintain

- Edit `index.html` for research text, citations, links and contact information.
- Edit `style.css` for presentation. No build tool, JavaScript, remote fonts, analytics or package dependencies are required.
- Serve locally with `python3 -m http.server 8000` and open http://localhost:8000/.
- Deployment uses the existing GitHub Pages configuration. Preserve `CNAME` (`fedtrust.ai`) and domain DNS records.
- Existing anchors `#research`, `#projects`, `#publications`, `#team` and `#contact` remain valid. `#projects` maps to the conceptual framework; `#team` maps to the academic lead.
- Check desktop and mobile layouts, keyboard navigation, links and citation metadata after edits. Update sitemap lastmod when publishing substantive changes.

## Content provenance (verified 2026-09-22)

Affiliation and academic email: https://meyangli.com/ and the author affiliation in https://arxiv.org/html/2508.18318v1.

Publisher-deposited Crossref metadata was checked for full author order, title, journal, volume, issue, pages/article number and journal publication year:

| Article | DOI | Technical source |
| --- | --- | --- |
| ZTFed-MAS2S (2026) | 10.1109/TII.2025.3609075 | https://arxiv.org/abs/2508.18318 |
| F-MADRL (2024) | 10.1109/TNNLS.2022.3232630 | https://pubmed.ncbi.nlm.nih.gov/37018258/ (article abstract) |
| FedDRL forecasting (2023) | 10.1016/j.apenergy.2022.120291 | https://arxiv.org/abs/2211.02674 |
| Secure federated FDIA detection (2022) | 10.1109/TSG.2022.3204796 | https://arxiv.org/abs/2209.00778 |

Use https://api.crossref.org/works/{DOI} to recheck publisher metadata. DOI year strings are not necessarily the journal volume year. All four are published journal articles; arXiv links are separately labelled author preprints.

The framework is an editorial synthesis, not an implemented platform. Future resilience questions are explicitly separated from evaluated tasks. Data locality, encryption, differential privacy and attack robustness are not presented as equivalent guarantees. No field deployment, end-to-end resilience performance, formal institutional status or IEEE endorsement is claimed.

No verified paper-specific public code or benchmark was identified during this release; the Resources section is therefore omitted. Do not label third-party forks as original research outputs.

The personal site and Task Force site are separate projects and were not changed. The Task Force public URL returned HTTP 403 in this execution environment; its institutional boundary follows the owner's explicit brief.

## Hosting baseline

Before changes on 2026-09-22: fedtrust.ai returned HTTPS 200 with the repository's original index. Public DNS reported A `185.199.108.153`; www CNAME `yangnedu362.github.io`. Apex MX and TXT queries returned no answers. No DNS, CNAME, email or Pages configuration changes were made. These observations describe the test environment, not worldwide or mainland-China reachability.
