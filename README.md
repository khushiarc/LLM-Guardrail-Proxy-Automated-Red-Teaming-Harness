# LLM-Guardrail-Proxy-Automated-Red-Teaming-Harness
Built a dual-plane AI firewall &amp; CI/CD test harness to secure LLM apps. The Control Plane runs adversarial injection mutations against prompts via Pytest, blocking unsafe deployments using PostgreSQL quality gates. The Data Plane acts as an async FastAPI proxy, scanning runtime inputs for jailbreaks and scrubbing tokens to prevent PII leaks.
