# Changelog

All notable changes to the **TIBCO BWCE Jenkins Git Parameter Global Configuration & Multi-Cluster SSOT** repository will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-09-03

### Summary
Initial production-ready release of the centralized configuration SSOT repository for `jenkins-git-parameter-bwce`. Reviewed, audited, and hardened using **Gemini 3.8 Flash**.

This repository manages multi-cluster topologies, environment definitions (`dev`, `staging`, `prod`), TIBCO BWCE application catalogs, Helm values overlays, and External Secrets Operator (ESO) HashiCorp Vault mappings for OpenShift 4.20+ clusters.

---

### 🚀 Added
- **Centralized BWCE Topologies**:
  - Registered declarative cluster topology manifests (`clusters/ocp-dev-cluster.yaml`, `clusters/ocp-staging-cluster.yaml`, `clusters/ocp-prod-cluster.yaml`).
- **Environment Overlays**:
  - Fully externalized configuration parameters and Datadog APM settings across DEV, STAGING, and PROD environments.
- **Enterprise Release Tags**:
  - Pinned stable Git release tags consumed dynamically by the Jenkins Git Parameter dropdown UI for TIBCO BWCE microservices.
