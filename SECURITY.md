# Security Policy

This file provides the default security policy for Knowledge Forge AI repositories that do not publish a repository-specific `SECURITY.md`. A repository-local security policy takes precedence over this organization default.

## Supported Versions

Knowledge Forge AI projects vary in maturity and release cadence. Unless a repository documents a different support policy, the current default branch is the only development line considered for security fixes. Historical commits, development snapshots, and older releases do not receive a blanket support commitment.

Maintainers may choose to backport a fix to a released version when appropriate, but such a backport is not implied by this default policy.

Consult the affected repository's README, release notes, tags, and any repository-local `SECURITY.md` for authoritative support information.

## Reporting a Vulnerability

**Do not report a suspected vulnerability through public issues, discussions, pull requests, or social media.**

For a public Knowledge Forge AI repository, use that repository's **Security** page and select **Report a vulnerability** when private vulnerability reporting is available.

If private vulnerability reporting is unavailable, contact the project steward privately at **lair001@gmail.com**. Send only the minimum information necessary to establish private contact initially; do not send credentials, secrets, unrelated personal information, customer data, or production data by email.

When it is safe to do so, a useful report includes:

- the affected repository, version, release, or commit;
- the affected component;
- the conditions required to reproduce the issue;
- the security impact and realistic attack preconditions;
- a minimal proof of concept or reproduction;
- whether the issue appears to affect published artifacts or downstream users; and
- a suggested mitigation, when known.

Please coordinate public disclosure with the maintainers until a remediation or disclosure decision has been made.

## What Reporters Can Expect

Maintainers will use a reasonable, evidence-driven process that may include:

- acknowledging receipt of the report;
- validating the issue and assessing severity and scope;
- requesting additional information when necessary;
- developing and validating a mitigation or fix;
- determining whether releases, advisories, or downstream notifications are appropriate;
- coordinating disclosure; and
- providing reporter credit when requested and appropriate.

Response and remediation timing depends on severity, affected components, available evidence, maintainer availability, and the maturity of the affected project. This policy does not promise a fixed response or remediation deadline.

## Scope

Security reports may cover, where applicable:

- project source code and default runtime behavior;
- release artifacts and packaging;
- dependency and build-chain behavior, including build-only tooling;
- installation, update, migration, and destructive lifecycle operations;
- authentication, authorization, privilege, or isolation boundaries;
- secret, credential, privacy, or unintended data exposure;
- injection, path traversal, arbitrary code or command execution;
- publication, provenance, signature, checksum, or artifact-integrity failures;
- unsafe handling of untrusted files, repositories, prompts, model/tool output, or other external inputs when a concrete security boundary is affected; and
- other defects with a plausible confidentiality, integrity, or availability impact.

Dependency findings remain in scope even when the affected dependency is used only during builds or packaging. Ordinary defects without a plausible security impact belong in the normal issue process.

## Disclosure and Good-Faith Boundaries

Test only systems, accounts, repositories, artifacts, and data that you own or are explicitly authorized to test.

Avoid privacy violations, service disruption, data destruction, persistence, credential access beyond what is necessary to demonstrate the issue, and lateral movement. Stop after establishing the minimum evidence needed to show the vulnerability and its impact.

Do not exploit a vulnerability for personal benefit, access data unrelated to the report, or intentionally degrade services. Allow maintainers a reasonable opportunity to investigate and remediate before public disclosure.

These boundaries describe the requested reporting process and do not create additional legal rights, warranties, safe-harbor commitments, or remediation obligations.
