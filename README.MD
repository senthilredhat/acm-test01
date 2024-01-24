# Attempt to replicate GitOps Standard layout [https://github.com/redhat-cop/gitops-standards-repo-template]

## Installation
1. Checkout the repository [https://github.com/senthilredhat/acm-test01.git] to local
2. Install App of App manifests uwing following commands
    `
    cd acm-test01
    oc apply -k ./app-of-app-manifest/
    `
3. This should install two applications to clusters based on label `env=stage` or `env=production`

## Folder Structure

### applications
This folder contains placement and subscriptions for individual application

### clusters
Folder contains deployment customizations per cluster

### Components
Original manifests for individual application