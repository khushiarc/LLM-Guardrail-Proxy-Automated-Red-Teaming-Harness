# LLM-Guardrail-Proxy-Automated-Red-Teaming-Harness
Built a dual-plane AI firewall &amp; CI/CD test harness to secure LLM apps. The Control Plane runs adversarial injection mutations against prompts via Pytest, blocking unsafe deployments using PostgreSQL quality gates. The Data Plane acts as an async FastAPI proxy, scanning runtime inputs for jailbreaks and scrubbing tokens to prevent PII leaks.

Project Overview: Adversarial Red-Teaming Gateway for LLMs
A dual-plane security infrastructure designed to harden LLM-powered applications against production-grade vulnerabilities (Prompt Injections, Privilege Escalations, and Multi-Tenant Data Leaks). The system splits responsibilities between an offensive Control Plane (CI/CD Quality Gate) that programmatically breaks prompts before deployment, and a defensive Data Plane (Runtime Proxy Middleware) that filters real-time token streams.

Key Architectural Features
Automated Red-Teaming Pipeline: Programmatically evaluates prompt templates against a localized database of mutated attack vectors (role-play overrides, indirect injections).

Deterministic Evaluation Rubrics: Leverages strict negative-constraint validation and exact-match filters to ensure the system never veers off the defined "Golden Path" of reliability.

Stateful Audit Logging: Powered by a relational database schema (PostgreSQL) tracking execution latency, total token allocation, and granular trace timelines for every interaction.
