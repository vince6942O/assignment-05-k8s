# Assignment-05: K8s - Deployment, Service, ConfigMap, Secret

Orchestration of a **Web Application** on Azure Kubernetes Service.

## Justification

### 1. Deployment (`Deployment`)
Managing lifecycle and scaling and providing self-healing by restarting crashed containers to maintain state.

### 2. Service (`Service`)
* **WebApp (LoadBalancer):** Exposes frontend via public External IP.
* **MongoDB (ClusterIP):** Restricts database access to internal cluster traffic only.

### 3. ConfigMap (`ConfigMap`)
Decouples configuration (Database URL) from the container image, allowing updates without rebuilding.

### 4. Secret (`Secret`)
Injects sensitive credentials (user/pass) as environment variables at runtime, preventing hardcoded secrets.
