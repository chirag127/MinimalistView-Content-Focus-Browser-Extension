# Security Policy for MinimalistView-Content-Focus-Browser-Extension

As an Apex Technical Authority project, we maintain rigorous security standards aligned with **December 2025 best practices**. The security of the browsing experience is paramount, given this extension's deep interaction with web content.

## 1. Supported Versions

This repository strictly supports the latest stable version of the extension. Security updates will only be applied to the current mainline branch (`main`/`master`). Legacy versions are not supported or patched.

## 2. Reporting a Vulnerability

We encourage responsible disclosure. If you discover a security vulnerability, please follow these steps immediately:

1.  **Do not** open a public Issue. This exposes the vulnerability to malicious actors.
2.  **Privately disclose** the vulnerability to the maintainer using one of the following channels:
    *   **Recommended:** Email security disclosure to `security+minimalistview@[YourDomainHere].com` (Note: Replace `[YourDomainHere]` with a placeholder or actual contact if available, as this is an automated response).
    *   **Alternative:** Create a draft Security Advisory on GitHub (if repository settings permit private reporting).

### Disclosure Requirements
When reporting, please include:
*   A clear description of the vulnerability.
*   The affected file(s) and line numbers, if known.
*   Steps to reproduce the vulnerability (Proof of Concept).
*   Any suggested remediation, if you have one.

## 3. Vulnerability Handling Timeline

We adhere to a strict, fast-paced remediation timeline typical of Tier-1 engineering projects:

| Stage | Target Timeframe |
| :--- | :--- |
| **Acknowledgement** | Within 24 hours of receipt |
| **Triage & Verification** | Within 72 hours |
| **Patch Development** | Dependent on severity; Critical issues targeted for immediate hotfix |
| **Public Disclosure** | Only after the patch has been released to production channels (e.g., Chrome Web Store, Firefox Add-ons) and a reasonable embargo period (max 14 days) has passed. |

## 4. Security Audits and Tooling

This repository is architected using **Zero-Defect, High-Velocity** principles. We actively use static analysis tools to prevent common vulnerabilities:

*   **Static Analysis:** While the core extension logic is likely JavaScript/TypeScript (based on modern extension development), analysis tools appropriate for that ecosystem (e.g., ESLint/Biome custom rules targeting XSS, CSP violations, and sensitive data exposure) are enforced in the `ci.yml` workflow.
*   **Dependency Scanning:** Automated dependency checks (e.g., Dependabot, Snyk integration) are configured to monitor for known CVEs in third-party libraries.

**For reference, our CI pipeline validation is defined in:** [.github/workflows/ci.yml](https://github.com/chirag127/MinimalistView-Content-Focus-Browser-Extension/actions/workflows/ci.yml)

## 5. License and Legal

This project is released under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** License. Review the `LICENSE` file for full details regarding use and distribution.

--- 
*This policy is subject to updates reflecting the evolving threat landscape and Apex Authority standards.*