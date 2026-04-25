# Secure DevSecOps App

This repository demonstrates a complete GitHub-native DevSecOps pipeline with:

## Security Controls
- SAST (Semgrep)
- Dependency scanning (pip-audit)
- Secret scanning (Gitleaks)
- Container scanning (Trivy)

## Advanced Features
- SBOM generation (CycloneDX)
- Artifact storage for auditability
- Multi-job pipeline with enforced gating
- Trusted build promotion

## Pipeline Flow
1. Scan job runs all security checks
2. Build job executes only if scan succeeds
3. Container is scanned and SBOM generated
4. Artifacts are stored for traceability

## Artifacts Produced
- Dependency scan report
- Secret scan report
- Container vulnerability report
- SBOM (CycloneDX)
- Trusted build marker
