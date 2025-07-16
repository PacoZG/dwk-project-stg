# 🚀 Exercise 4.10. The project, the grande finale

## 🎯 Project Goal

Finalize the project setup so that it uses different repositories for the code and configurations.

-----

## 🏗️ Implementation Structure

Our approach involved a well-organized manifest structure using Kustomize
overlays, ensuring clear separation and reusability for our different
environments.

```
deploy/kubernetes/
├── base/
│   ├── 00-broadcaster.yaml
│   ├── 01-postgres.yaml
│   ├── 02-server.yaml
│   ├── 03-client.yaml
│   ├── ... (other base manifests)
│   └── kustomization.yaml
└── overlays/
    │   
    └── stg/
        ├── application.yaml  # ArgoCD App for staging
        ├── kustomization.yaml # Staging kustomize overlay
        ├── ... (other stg specific manifests)
```

-----

## ✅ Deployment Insights

### 🖥️ Local Deployment

This repository has been created to develop the dwk-project in staging environment.

