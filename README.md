# argocd-yaml-to-helm

## prerequisites
- Kubernetes cluster (minikube or kind works)

## Setup
- Deploy ArgoCD on your cluster (feel free to choose deployment method)
- Apply the given application manifest (`application.yaml` in the root dir of the repo) to create an ArgoCD application

## Task - Migrate the application to deploy metrics server via helm chart.

## Details
- No downtime is allowed.
- Avoid pod restarts.
- The given manifest has an additional container arg in the deployment - `--kubelet-insecure-tls`. Make sure the deployment still has this arg, without editing `values.yaml` (or the templates) - Add it as application-level parameter/value.
