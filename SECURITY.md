# Security policy

## Reporting a vulnerability

Email [security@arthur.place](mailto:security@arthur.place). Do not open a public issue or pull request with exploit details or credentials.

Include the affected repository and version, reproduction steps, expected impact and any relevant configuration or logs with secrets removed. For remote connections, describe which machine an attacker would need access to. A minimal proof of concept is helpful; do not test against systems or data you do not own or have permission to assess.

Reports are reviewed by maintainers. Response and fix times depend on severity and availability; there is no guaranteed response window. Please coordinate public disclosure after a fix or mitigation is available, and mention any disclosure deadline in your report.

## Scope

This policy covers devlanes-run repositories unless a repository has its own security policy. Report issues such as unintended network exposure, unauthorized access to the daemon, privilege escalation, credential disclosure or failures in TLS and remote connection handling.

A lane separates a development stack's ports, hostnames and data. It is not a security sandbox for untrusted code. Processes run with the permissions of the user or container running them. Reports should identify a security boundary that can be crossed, rather than assume lanes provide process isolation.

## Supported versions

Security fixes target the latest release and the default branch. Older versions do not have a backport guarantee. Individual repositories may document a different support policy.

For non-security questions, contact [devlanes@arthur.place](mailto:devlanes@arthur.place) or open an issue in the relevant repository.
