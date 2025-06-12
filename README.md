# k8s-gitops-test-demo
k8s-gitops-test-demo
📁 helm/
   └── api-tests/
       ├── templates/
       │   └── deployment.yaml         # Test runner pod definition
       └── values.yaml                # Runtime config for Rest Assured/JMeter tests
📁 .github/workflows/
   └── test-on-pr.yaml               # GitHub Actions workflow (PR → Helm → GitOps)
📁 manifests/
   └── namespace.yaml                # Dynamic namespace creation per PR
📁 scripts/
   └── generate-test-manifests.sh    # Automates manifest commits to GitOps repo
📄 README.md                          # Usage instructions



Tools Integrated:

    GitHub Actions (CI trigger)

    Helm (test chart deploy)

    ArgoCD/Flux (GitOps controller)

    Kubernetes (ephemeral namespace)

    Rest Assured or JMeter as test containers



Pull Request triggers GitHub Actions

Helm chart pushed to GitOps repo

ArgoCD applies it to Kubernetes

Test pod runs → logs results

Metrics go to dashboard (optional)





    
