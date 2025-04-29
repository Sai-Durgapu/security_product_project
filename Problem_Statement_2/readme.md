Kubernetes Security Scan

- Setup:
  - Used Minikube to create a local Kubernetes cluster.
  - Installed Kubescape to scan the cluster.
- Scan:
  - Ran: kubescape scan --format json --output k8s_findings.json
  - If no findings, deployed a test app (nginx) with: kubectl run nginx --image=nginx
- Output:
  - Saved scan results in: k8s_findings.json
  - Open this file to see security issues (e.g., RBAC or port problems).
