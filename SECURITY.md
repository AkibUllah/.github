# Security policy

## Reporting a vulnerability

Please **do not** open a public issue for security problems.

Use GitHub's private vulnerability reporting on the affected repository (**Security** tab → **Report a vulnerability**). Include:

- the affected repository and commit or version,
- steps to reproduce or a proof of concept,
- the impact you expect.

You'll get an acknowledgement within 3 working days and a status update within 10. Once a fix is released, you're welcome to be credited in the release notes.

## Scope

These are portfolio and reference projects. Payment, KYC and messaging integrations ship with **sandbox or stub adapters only** and must not be pointed at production credentials without your own review. Reports about the stubs themselves being non-functional are not vulnerabilities; reports about the core services (authentication, signature verification, tenant isolation, SQL guarding, rate limiting and similar) very much are.
