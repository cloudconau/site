# ![](../images/speakers/headshots/MichaelFornaro.png){ width="200" } Michael Fornaro - Easygo

## Gitless GitOps with FluxCD

### Abstract
The GitOps model gave us traceable, declarative infrastructure. But relying on Git access from your clusters comes with downsides—network complexity, access control challenges, and audit gaps. This talk presents an evolved approach: keep Git as your truth, but push OCI-packaged artifacts to a registry where FluxCD can pull and reconcile securely.

You’ll learn how to:
- Build and package Kubernetes manifests into OCI images with tooling like flux push or oras
- Use image tags (e.g., latest, staging, stable) to decouple promotion from Git branching
- Sign artifacts using keyless signatures via Sigstore (cosign) to enforce trust and verify integrity
- Store and distribute SBOMs and VEX alongside manifests for audit-ready compliance
- Onboard teams or tenants with minimal friction—no need to give them Git access to the cluster

This architecture supports fine-grained control, eliminates the need for Git webhooks or polling, and aligns perfectly with security-first delivery practices. You'll leave with a practical, battle-tested method for running GitOps without direct Git dependencies at runtime.