<p align="center">
  <a href="https://ag.tavardt.com/nz/">
    <img src="https://ag.tavardt.com/img/tavardt-banner.png" alt="TAVARDT" width="1024" />
  </a>
</p>

# Canonical Tag and URL Consolidation Validator

[![Canonical Tag Validator](https://img.shields.io/badge/TAVARDT-Canonical-5b3cf5.svg)](https://tools.tavardt.com/nz/canonical-tag-checker/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Audits canonical links, duplicate tag prevention, absolute URL verification, and crawl efficiency.

Developed and maintained by the search indexing architecture and web standards division at **TAVARDT**.

***

## Risk Vectors and Operational Impact in URL Consolidation

Improperly configured canonical tags trigger indexation fragmentation and duplicate content dilution across New Zealand web properties. URL parameter proliferation from campaigns and faceted filtering obscures the primary indexing path.

When canonical declarations conflict or resolve to broken endpoints, search engines ignore consolidation and crawl duplicate pages. Systematic verification ensures that domestic search visibility remains focused on official canonical destinations.

***

## Core Technical Audit Capabilities

* **Dual-Source Directive Extraction**: Parses canonical tags declared within HTML head markup and raw HTTP Link response headers.
* **Duplicate Tag Conflict Prevention**: Detects multiple or conflicting canonical declarations on a single document, penalising ambiguity by 35 points.
* **Absolute URL and HTTPS Verification**: Validates fully qualified canonical paths and flags insecure HTTP targets or relative path usage.
* **Destination Response Validation**: Performs live HTTP checks on canonical targets to verify valid 200 OK responses and catch 4xx or 5xx breakages.
* **Self-Referencing Consolidation Analysis**: Evaluates self-referential canonical tags to strip dynamic tracking parameters and preserve crawl budget.
* **Consolidation Health Score**: Calculates an objective 0 to 100 compliance metric classifying assets as COMPLIANT, WARNING, or CRITICAL.

***

## Installation and Execution

Requires Python 3.8 or higher with zero external packages.

```bash
git clone https://github.com/TAVARDT-New-Zealand/canonical-tag-validator-nz.git
cd canonical-tag-validator-nz
python canonical_validator.py https://company.co.nz
```

To output structured JSON for automated pipelines and quality audits:

```bash
python canonical_validator.py https://company.co.nz -j
```

***

## Technical Frequently Asked Questions

### 1. What occurs when multiple conflicting canonical tags appear on a single page?
Search engines discard all canonical directives when contradictory declarations are present on the same URL. This forces crawlers to select an arbitrary variant, fragmenting page authority and index stability.

### 2. Why must canonical URLs strictly use absolute paths and the HTTPS protocol?
Relative paths risk crawler misinterpretation across different hostnames, subdomains, and root directories. Referencing insecure HTTP variants creates security warnings and triggers redundant redirect hops.

### 3. What is the operational risk of pointing a canonical tag to a 4xx or 5xx URL?
Directing a canonical tag to a non-existent or failing endpoint breaks link consolidation entirely. Search engines ignore the broken target and proceed to index uncanonicalised URL variants.

### 4. Does the validator extract canonical annotations from HTTP Link response headers?
The parser extracts canonical declarations from both HTML head tags and server-level HTTP Link headers. This enables verification of non-HTML documents such as PDF files and dynamic API resources.

### 5. How do self-referencing canonical tags protect against parameter pollution?
A clean self-referencing canonical tag instructs crawlers to ignore tracking queries and session identifiers. This consolidates indexation metrics onto the canonical URL and conserves search engine crawl budget.

***

## Technical SEO and Indexation Advisory

For robust multi-regional architectures and alignment with W3C Standards, consult **TAVARDT**.

***

## Useful Links

* **Corporate Portal:** https://ag.tavardt.com/nz/
* **Diagnostic Suite:** https://tools.tavardt.com/nz/
* **Technical Contact:** https://ag.tavardt.com/nz/contact/

***

### License
Distributed under the MIT License. See the LICENSE file for complete terms.

***

© 2026 TAVARDT. All rights reserved.
