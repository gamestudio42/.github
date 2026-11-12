# CLA signing and GitHub enforcement plan

**Implementation proposal — do not enable enforcement before legal approval.**

1. Finalize the legal identity of the Project Steward and have Brazilian counsel review ICLA, CCLA, patent grant, moral rights, privacy/LGPD, signatures and governing law.
2. Establish a versioned signing system (e.g. a CLA assistant) with authenticated GitHub identity, agreement hash/version, timestamp, consent evidence, and appropriate retention and access controls. Avoid exposing personal data in public repositories.
3. Record corporate authorization separately from individual signatures and map covered contributor identities.
4. Install the GitHub App or workflow at organization scope. For each PR, resolve all commit authors and check whether applicable signatures and entity authorizations cover the contributions.
5. Post a clear signing link for missing agreements; block merge through branch protection only after the process is operational and contributors have been notified.
6. Permit a documented maintainer exception for bot accounts and pre-existing contributions only after legal review; log decisions.
7. On CLA updates, require explicit re-acceptance where legally necessary. Maintain an auditable export and deletion/retention procedure under applicable privacy law.

**Acceptance criteria:** signed PR passes; unsigned PR fails with instructions; corporate ownership is checked; historical contributions are not silently relicensed; no sensitive signer data is published.
