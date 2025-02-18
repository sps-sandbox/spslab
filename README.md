
# SPS Sandbox

## Purpose:
To quickly demonstrate use cases that are not available in Democenter and been time-consuming for custom setups (with CSC).

## Out of Scope:
Any performance tests on storage arrays.

In the initial phase, Phase I use cases are delivered. Phase II use cases will be delivered by March 2025.

## Setup

| Phase I                                   | Phase II                                         |
|-------------------------------------------|--------------------------------------------------|
| PowerFlex 4.6 x 2 (PF01 & PF02)           | SUSE Rancher                                     |
| PowerStore 4 x 2 (PowerStore-1 & PowerStore-2) | Ansible / Ansible Modules (Dell Storage)        |
| PowerScale                                | Terraform / Terraform Providers (Dell Storage)   |
| Openshift (2 clusters, v4.17)             | Cloud Native / Stateful Applications / Database (MSSQL, MongoDB) |
| Dell CSI drivers for PowerFlex & PowerStore | GitLab / GitHub                                |
| Dell CSM Replication modules for PowerFlex & PowerStore | Ansible Lint / SonarQube                       |
| Dell CSM Auth module for PowerFlex        | ArgoCD / FluxCD                                  |
| Dell CSM Resiliency module for PowerFlex & PowerStore | Jenkins                                      |

## Use Cases:

| Use Case                        | Storage               | Scope                                                                                                                                       |
|----------------------------------|-----------------------|---------------------------------------------------------------------------------------------------------------------------------------------|
| **Phase I**                      |                       |                                                                                                                                             |
| 1. General Management Capability | PowerFlex             | Demonstrate general management capability, including replication through PowerFlex Manager 4.6.                                              |
| 2. General Management Capability | PowerStore            | Demonstrate general management capability, including replication through PowerStore Manager 4 (Block only).                                   |
| 3. Container Workloads on OpenShift | PowerStore & PowerFlex | Provisioning of Persistent Volumes on PowerStore and PowerFlex using Dell CSI drivers.  <br> - Showcase volume lifecycle <br> - Showcase snapshot creation <br> - Create PVC from snapshots. <br> **Extension** (needs additional effort): <br> - Can be shown on upstream Kubernetes <br> - PowerScale provisioning can be shown. |
| 4. Resiliency for Container Workloads on OpenShift | PowerFlex, PowerStore | Showcase node resiliency on OpenShift clusters using the CSM Resiliency module on PowerFlex and PowerStore. <br> - Shutdown node <br> - Shutdown network. |
| 5. Stateful Application Replication Capability | PowerFlex, PowerStore | Showcase replication capability on PowerFlex (async) and PowerStore (sync & async) with CSM replication module on OpenShift. <br> - Failover application/pod to target <br> - Reprotect workload at target <br> - Failover back to source. <br> **Extension** (needs additional configuration effort): <br> 1. Can be shown on upstream Kubernetes. |
| 6. Role-Based Access Control for Storage with OpenShift | PowerFlex             | Showcase CSM Authorization capability on PowerFlex. <br> - Define storage quota at cluster level (OpenShift) <br> - Restrict storage admin credentials to OpenShift admin. <br> **Extension** (needs additional configuration effort): <br> 1. Can be shown on PowerScale <br> 2. Other supported Kubernetes distributions. |
| **Phase II**                     |                       |                                                                                                                                             |
| 7. Application Mobility (Container Workloads) | PowerStore            | Showcase application mobility across the same or different Kubernetes clusters with PowerStore.                                               |
| 9. Infrastructure Provisioning   | PowerFlex, PowerStore | Showcase IaC. Covers: <br> 1. Build/Modify code with Visual Studio Code (integration with Git) <br> 2. Source code management <br> 3. Continuous integration (integration with Ansible lint/SonarQube) <br> 4. Continuous Deployment (integration with deployment tools - cloud-init, Ansible modules for PowerStore/PowerFlex). |
| 10. GitOps with Dell Storage     | PowerFlex             |                                                                                                                                             |
