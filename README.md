# argocd-yaml-to-helm

## Task - Migrate the application to deploy metrics server via helm chart.

## Details
- No downtime is allowed.
- Avoid pod restarts.
- The given manifest has an additional container arg in the deployment - `--kubelet-insecure-tls`. Make sure the deployment still has this arg, without editing `values.yaml` (or the templates) - Add it as application-level parameter/value.
