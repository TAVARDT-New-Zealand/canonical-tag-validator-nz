# Canonical Tag and URL Consolidation Validator

[![Canonical Tag Validator](https://img.shields.io/badge/TAVARDT-Canonical-5b3cf5.svg)](https://tools.tavardt.com/nz/canonical-tag-checker/)
[![Jurisdiction](https://img.shields.io/badge/Jurisdiction-New%20Zealand-00C853.svg)](https://ag.tavardt.com/nz/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Audits canonical links, duplicate tag prevention, absolute URL verification, and crawl budget protection.

Developed and maintained by the digital systems and crawl optimization division of **[TAVARDT New Zealand](https://ag.tavardt.com/nz/)**.

---

## Canonical Tag Audit Capabilities

* **Canonical Directive Inspection**: Audits `<link rel="canonical">` tags in HTML head sections and HTTP Link headers.
* **Duplicate Tag Prevention**: Detects conflicting or multiple canonical tags declared on a single document.
* **Absolute URL Verification**: Ensures canonical directives use absolute paths with secure HTTPS protocols.
* **Destination Response Verification**: Verifies that the canonical target URL returns an HTTP 200 OK status code.
* **Consolidation Health Score**: Quantitative 0 to 100 health score with prioritized technical remediation steps.

---

## Installation and Execution

Requires Python 3.8 or higher.

```bash
git clone https://github.com/TAVARDT-New-Zealand/canonical-tag-validator-nz.git
cd canonical-tag-validator-nz
python canonical_validator.py https://company.co.nz
```

To output results in structured JSON format:

```bash
python canonical_validator.py https://company.co.nz --json
```

---

## Comprehensive Web Diagnostic

For full web verification and deep URL consolidation audits:

* **[Official Canonical Tag Checker Tool](https://tools.tavardt.com/nz/canonical-tag-checker/)**
* **[TAVARDT New Zealand Enterprise Portal](https://ag.tavardt.com/nz/)**

---

## Technical SEO and Indexation Advisory

For platforms operating across New Zealand under W3C Standards and NZ Digital Government Guidelines, contact **[TAVARDT New Zealand](https://ag.tavardt.com/nz/contact/)**.
