# gitops
A repo for storing plain kubernetes manifests to deploy to my homelab kubespray cluster.

I use the `homelab` branch as my plain manifests branch which ArgoCD points at for deployments.

The `main` branch is used for storing the helm charts and kustomize overlays that are relied on for generating plain manifests in `homelab` branch.

NOTE: The `homelab` branch should ONLY be touched by the CI pipeline. All changes should be made to the `main` branch to tricke into the `homelab` branch.
