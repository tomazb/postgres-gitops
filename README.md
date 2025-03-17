# postgres-gitops
Simple Kubernetes deployment that uses the Red Hat PostgreSQL container image from the Red Hat container registry. Check https://catalog.redhat.com/software/containers/rhel9/postgresql-16/657b03866783e1b1fb87e142 to see possible environment variables you can use to customize it.

Check postgres-kustomize branch to see Kustomize support.

On OCP you will need something like this for ArgoCD to be able to deal with secrets:
oc label namespace workshop argocd.argoproj.io/managed-by=openshift-gitops

