# Security AI Agent (Commercial)

Autonomous penetration-testing copilot that orchestrates 20+ Kali-grade tools with an LLM-driven decision engine, real-time logging, and professional reporting. Built for network security professionals who want aggressive coverage, repeatable methodology, and auditable results.

## Who This Is For
- Red teams and offensive security engineers
- MSSPs delivering repeatable web app and infrastructure assessments
- Defensive teams validating controls with controlled offensive runs

## Why Teams Use It
- **Full-stack coverage fast:** Seven-phase heuristic playbook runs recon, CMS checks, vuln scanning, fuzzing, exploitation attempts, and credential tests in minutes.
- **Tool resilience:** Binary-first, Python fallback implementations keep scans running even when some tools are missing on the host.
- **Operational clarity:** Live terminal-style UI, structured JSON audit logs, and Markdown reports with severity, PoC details, and remediation notes.
- **Safety and compliance:** PoC-only by default, hard timeouts, legal banners, and audit trails for every action.

## Key Capabilities
- 21-tool arsenal: nmap, nikto, nuclei, wpscan, wafw00f, feroxbuster-style dir fuzzing, wfuzz-style parameter fuzzing, sqlmap, hydra/ncrack/medusa credential testing, SSL/TLS checks, exploit DB lookups, and more.
- Heuristic sequencing: 7-phase flow (recon → CMS/stack → vuln scans → fuzzing → SSL/service analysis → credentials → deep discovery).
- Fallbacks: Python implementations for WAF detection, nuclei-style template checks, directory/parameter fuzzing, SSL checks, and subdomain discovery when binaries are absent.
- Reporting: Vulnerability markdown reports + JSON audit logs per target for compliance and reproducibility.
- Deployment: Works on Kali/Linux, CPU-only; supports air-gapped use with local LLM (Phi-2/Mistral via Ollama) when desired.

## Pilot Quickstart
- Request a pilot build (security@sirspyr0.com) and define scope/authorization.
- Provision a Kali/Linux host; ensure Python 3.12 and core tooling available (we supply fallbacks for missing binaries).
- Run the guided pilot against your staging or lab target; review live logs via the UI and the generated report/audit log.
- Tune timeouts, wordlists, and sequencing; move to production once satisfied.

## Sample Outputs
- Report: reports/sample_vulnerability_report_example.com.md
- Audit log: logs/sample_audit_example.com.json

## Engagement Model
1. **Discovery call:** Confirm scope, targets, and authorization. The agent is for authorized testing only.
2. **Pilot run:** We provide a guided pilot build; you execute against an agreed target while we monitor outcomes and tune timeouts/tool set.
3. **Rollout:** Move to your Kali or server environment; optional UI/dashboard enablement.
4. **Support:** Updates, tuning, and rulepacks under a commercial subscription.

## Licensing (Commercial)
- This public repository is a commercial offering with no rights to use, modify, or distribute the software without a paid license agreement.
- Evaluation builds are available under a time-limited evaluation addendum.
- For licensing and pilots, contact: security@sirspyr0.com

## Next Steps
- Request a pilot build and target scope review.
- Get a sample report and audit log package.
- Schedule a guided run on your staging or lab environment.

**Reminder:** Use only on systems you own or have explicit written authorization to test.
